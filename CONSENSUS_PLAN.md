# Multi-Agent Consensus Plan

A repeatable procedure for taking N divergent agent answers to the same question
(here: 10 answers) and producing a single consensus answer where **the
most-supported position wins on every point** — plurality rule, no minimum
threshold. If the largest voting block is 2/10 and everything else is 1/10,
the 2/10 position is adopted.

---

## Ground rules

1. **Plurality wins, always.** For each decision point, the position backed by
   the most agents is adopted. There is no quorum and no minimum share.
2. **Every point gets a ruling.** No decision point is left as "the agents
   disagreed." Ties are broken by the deterministic rules in Step 5.
3. **Positions are counted, not agents.** An agent that didn't address a point
   simply doesn't vote on that point. Abstentions shrink the denominator; they
   are never counted as "no."
4. **Semantic matching, not string matching.** Two answers phrased differently
   but meaning the same thing are the same position and their votes pool.
5. **The process is auditable.** Every ruling in the final answer traces back
   to a tally row showing who voted for what.

---

## Step 1 — Collect and freeze the inputs

- Gather all 10 answers verbatim into `answers/agent-01.md` … `answers/agent-10.md`.
- Do not edit, trim, or paraphrase them. These are the evidence record.
- If an answer is missing or an agent gave two conflicting answers in one
  response, keep the **last** complete statement it made (most-recent-wins
  within a single agent).

## Step 2 — Decompose into atomic claims

Read all 10 answers and extract every distinct **decision point** — a single
question that can be answered independently. Examples of decision points:
"Which database should we use?", "Is X a bug?", "What is the value of Y?".

- Assign each decision point an ID: `Q1`, `Q2`, `Q3`, …
- A decision point raised by even one agent goes on the list. (It may end up
  decided by a 1-vote plurality if nobody else spoke to it — that is allowed.)
- Split compound claims. "Use Postgres and shard by tenant" is two points:
  the database choice and the sharding strategy. Agents may agree on one and
  not the other, and pooling them hides that.

## Step 3 — Normalize positions

For each decision point, cluster the agents' statements into **canonical
positions**:

- Merge paraphrases: "use PostgreSQL", "Postgres is the right call", and
  "I'd go with pg" are one position.
- Merge subsumed answers into the more specific one only if they are
  compatible; otherwise keep them as separate positions. "Use a relational DB"
  and "use Postgres" pool **only** if no other relational option is in play —
  if another agent says "use MySQL", then "use a relational DB" stays its own
  (compatible-with-both) position and does not tip the Postgres/MySQL count.
- Record hedged answers ("probably X, but maybe Y") as a vote for the primary
  recommendation (X). A pure 50/50 fence-sit is an abstention.

## Step 4 — Tally

Build one table per decision point in `tally.md`:

```
## Q1: <decision point>
| Position | Votes | Agents |
|---|---|---|
| <canonical position A> | 4 | 01, 03, 06, 09 |
| <canonical position B> | 2 | 02, 07 |
| <canonical position C> | 1 | 10 |
| (abstain / not addressed) | 3 | 04, 05, 08 |
**Ruling: Position A (4/7 voting).**
```

The ruling is simply the top row. A 2-vote plurality over nine 1-vote
scatterings wins exactly like a 9–1 landslide does.

## Step 5 — Tie-breaking (deterministic, in order)

Apply these in sequence until the tie breaks:

1. **Specificity:** the more specific, actionable position beats the vaguer one.
2. **Evidence:** the position whose supporting agents gave verifiable reasoning
   (citations, reproduction steps, working code) beats bare assertion.
3. **Compatibility:** the position consistent with rulings already made on
   other decision points wins (the consensus answer must not contradict itself).
4. **Re-vote:** put only the tied positions to a fresh, independent panel
   (3 new agents, blind to the original answers) and take their plurality.
5. **Coin flip, recorded:** if still tied, pick the first position in
   alphabetical order and mark the ruling `TIE-BROKEN (arbitrary)` so the
   reader knows it was not a real preference.

## Step 6 — Assemble the consensus answer

Write `CONSENSUS.md`: the single unified answer, composed of the winning
position for every decision point, written as one coherent response (not a
list of tally results). Each section footnotes its tally row, e.g.
`[Q3: 4/8]`, so any ruling can be audited back to Step 4.

Sanity pass before publishing:

- **Coherence check:** read the assembled answer end-to-end. If two winning
  positions contradict each other (possible, since they won independently),
  resolve by re-tallying the two points **jointly** — count which *combination*
  of positions the most agents actually held, and adopt the winning combination.
- **Coverage check:** every decision point from Step 2 has exactly one ruling.

## Step 7 — Optional: strengthen weak pluralities

The 2/10 rule stands — but a ruling that won with ≤30% support is worth
flagging. Mark those rulings `LOW CONFIDENCE` in `CONSENSUS.md`. If desired,
run a second round: show all 10 original answers to a fresh panel of agents
and ask them to vote *only* on the low-confidence points. Their votes add to
the tally (bigger denominator, same plurality rule). This is optional and
never overrides Step 5's determinism — it just adds voters.

---

## Automating this (agent pipeline)

The whole procedure maps cleanly onto a fan-out/fan-in agent workflow:

1. **Extractor agents** (one per answer file, in parallel): read
   `answers/agent-NN.md`, emit structured claims
   `{decision_point, position, hedged?, reasoning_present?}`.
2. **Merger** (single agent, needs all extractor output at once): unify
   decision-point IDs and cluster positions per Step 3.
3. **Tally** (plain code, no agent): count votes, apply plurality rule,
   apply tie-breakers 1–3 mechanically where possible; emit `tally.md`.
4. **Judge agents** (only for surviving ties): 3-agent blind re-vote per
   Step 5.4.
5. **Writer** (single agent): compose `CONSENSUS.md` from the rulings, then a
   final **coherence-critic** agent runs the Step 6 sanity pass.

Deterministic parts (counting, plurality, ordering) live in code; judgment
parts (clustering paraphrases, breaking ties on specificity/evidence) go to
agents that are blind to which agent said what, to avoid halo effects.

---

## Files this process produces

| File | Contents |
|---|---|
| `answers/agent-01.md` … `agent-10.md` | Frozen verbatim inputs |
| `claims.md` | Decision-point list from Step 2 |
| `tally.md` | One tally table + ruling per decision point |
| `CONSENSUS.md` | The single unified answer, with tally footnotes |

To run it: drop the ten answers into `answers/` and follow Steps 2–6, or ask
an agent to execute the pipeline above against that directory.
