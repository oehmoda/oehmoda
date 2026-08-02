# Consensus Plan — Founder Governance & Equity (oehmoda/oehmoda)

A concrete procedure for merging the independent governance/equity plans in this
repository into one consensus design where **the most-supported position wins on
every decision point** — plurality rule, no minimum threshold. If the largest
voting block is 2 plans and everything else is a 1-plan scattering, the 2-plan
position is adopted.

The subject matter, common to every plan: governance and equity design for a
~1-year-old Massachusetts LLC with 5 founders (some inactive), ~10 unpaid
employees, and a part-time Yale professor promised "a decent share."

---

## 1. The voters — actual inventory of this repo

The canonical aggregation lives on the **`all-plans`** branch under
`plans/plan-N/`. Cross-checking every branch gives this roster:

| Voter | Where to read it | Docs available | Notes |
|---|---|---|---|
| plan-1 | `all-plans:plans/plan-1/` | one-pager, implementation plan, merit formula, OA, references, research/ | Same content as the repo's default branch |
| plan-2 | `all-plans:plans/plan-2/` | design, one-pager, OA, references | |
| plan-3 | `all-plans:plans/plan-3/` | design, one-pager, OA, references | Exists only on `all-plans` (no own branch survives) |
| plan-4 | `all-plans:plans/plan-4/` | design, one-pager | **No operating agreement** — votes only on points its docs address |
| plan-5a | `all-plans:plans/plan-5/` | design, one-pager, OA, references, NOTE | Session `j5kmc7` |
| plan-5b | `all-plans:plans/plan5/` | design, one-pager, OA, references | Session `jx79r1` — an independent second run of plan 5 |
| plan-7 | `all-plans:plans/plan-7/` | design, one-pager, OA, references | |
| plan-9 | `all-plans:plans/plan-9/` | design, one-pager, OA, references | |
| plan-10 | `all-plans:plans/plan-10/` **+** branch `claude/llc-governance-equity-design-10j7h7` | OA on `all-plans`; design, one-pager, references only on its claude branch | Migration to `all-plans` was incomplete — read the claude branch for the full plan |

**That is 9 voters.** Plans 6 and 8 do not exist anywhere in the repo — the
denominator is 9, not 10, and no ruling should pretend otherwise.

Special cases, decided now so tallying is mechanical:

- **plan-5a and plan-5b both vote.** They were independent sessions answering
  the same brief; that is exactly what a voter is. The copy of 5b quarantined
  inside `plans/plan-5/_preexisting-unverified/` is a duplicate of `plans/plan5/`
  and must **not** be counted a second time.
- **`plan-review` (branch `plan-review`, also `plans/plan-review/` on
  `all-plans`) is not a voter.** It read and judged the other plans, so it is
  not independent. It is used in exactly one place: tie-breaking (§5, rule 2),
  where its assessments count as evidence quality signals.
- **Provenance files (`plan-N-provenance.md`) never vote.** They describe
  process, not positions.

### Within-plan precedence

When a single plan's documents disagree with each other, the position is taken
from, in order: **operating agreement → design doc → one-pager**. The OA is the
binding text a plan actually committed to; the one-pager is marketing for it.
(For plan-1 the "merit formula and rate table" ranks with its OA; for plan-4,
which has no OA, the design doc is authoritative.)

### Reading the inputs

Read everything from git without checking branches out, e.g.:

```bash
git show origin/all-plans:plans/plan-7/plan-7-operating-agreement.md
git show origin/claude/llc-governance-equity-design-10j7h7:plan-10-design.md
```

Note on the `all-plans` README isolation rules ("never read another team's
directory"): those rules bind the *plan teams* during authoring. This consensus
exercise is the repo owner's cross-plan aggregation step and necessarily reads
all plans; it writes only to the consensus branch
(`claude/multi-agent-consensus-j7lzgr`), never into any `plans/plan-*/`
directory and never to `all-plans` itself.

---

## 2. Decision points — seeded from the plans' shared structure

Every plan answers the same brief, so the decision points are largely known in
advance. The tally must cover at least these, with IDs fixed here:

**Equity architecture**
- **Q1** Equity model: fixed split vs. dynamic contribution ledger vs. hybrid (founder reserve + contribution pool)
- **Q2** Founder reserve: total % and per-founder %
- **Q3** Contribution pool: size, and formula (rate source, time multiplier, cash multiplier, any quality factor)
- **Q4** Year-1 retroactive settlement: method for crediting the undocumented first year
- **Q5** Vesting: schedule, cliff, and any activity condition (e.g. vest only in months actually worked)
- **Q6** Ledger freeze: trigger (first financing / conversion / breakeven) and what it converts into
- **Q7** Employee equity: instrument (profits interests vs. options), benchmarks, pool size after freeze

**People**
- **Q8** Inactive founders: keep earned / forfeit unearned / buyout (offered or forced) / board rights
- **Q9** The professor: % range, instrument, vesting, written-agreement terms, Yale IP handling

**Governance**
- **Q10** Board: size, composition, how seated (appointed vs. elected), independent seat or not
- **Q11** CEO: single vs. co-CEOs; selection and removal mechanics
- **Q12** Voting thresholds: reserved matters and required majorities; any unanimity anywhere
- **Q13** Disputes: ladder (mediation/arbitration/expert determination), shotgun clause or not

**Legal & entity**
- **Q14** Entity path: stay MA LLC now? Delaware C-corp conversion — when and how pre-authorized
- **Q15** Wage Act remediation: sequencing and scope (this appears in every plan skimmed so far; the tally records *how*, not *whether*)
- **Q16** Tax execution: 83(b)s, valuation timing, profits-interest mechanics

Step 2 of execution is to read all nine plans and **extend** this list with any
decision point at least one plan raises that isn't captured above (each gets the
next free ID). Split compound positions: "25% reserve vesting monthly" is Q2
(the 25%) and Q5 (the vesting) — plans may agree on one and not the other.

---

## 3. Normalize positions

For each decision point, cluster the nine plans' statements into canonical
positions before counting:

- Merge paraphrases: "4-year vest, 1-year cliff" and "48-month schedule with
  12-month cliff" are one position.
- Numeric answers cluster by **material equivalence**, not exact match: 65% and
  75% contribution pools are different positions; "0.5–1.5%" and "≈1%" for the
  professor are the same position. When in doubt, keep positions separate — the
  tie-breakers can handle fragmentation, but false merging can't be audited out.
- A vaguer position pools with a more specific one only if no competing
  specific position exists (see the general rule: "a relational DB" pools with
  "Postgres" only when no plan says "MySQL").
- Hedged positions ("we recommend X; Y is defensible") vote for X.
- A plan whose docs don't address a point **abstains** — it shrinks that
  point's denominator and is never counted as opposition. Expect this
  especially from plan-4 (no OA) and plan-10's `all-plans` copy (use its claude
  branch to minimize abstentions).

---

## 4. Tally

One table per decision point in `consensus/tally.md` on this branch:

```
## Q5: Vesting schedule
| Position | Votes | Plans |
|---|---|---|
| 48-month, activity-conditioned (vest only in ≥half-time months) | 2 | 7, 9 |
| 48-month straight, 12-month cliff | 2 | 2, 3 |
| Quarterly earn-in, use-it-or-lose-it | 1 | 1 |
| (abstain) | 4 | 4, 5a, 5b, 10 |
**Ruling: TIE → §5.**
```

The ruling is the top row. A 2/9 plurality over seven scattered or abstaining
plans wins exactly like a 8–1 landslide does. (The example above is
illustrative, not a pre-judged result.)

---

## 5. Tie-breaking (deterministic, in order)

1. **Specificity:** the more actionable, fully specified position wins.
2. **Evidence:** the position whose backing plans cite verifiable sources for
   it wins; here `plan-review`'s assessment of those plans counts as a signal,
   and a position a plan's own references file rates as weakly sourced loses
   to one rated strongly sourced.
3. **Compatibility:** the position consistent with rulings already made wins —
   the consensus design must not contradict itself (a 75% contribution pool
   ruling on Q3 is incompatible with a 30% founder reserve on Q2).
4. **Re-vote:** put only the tied positions to 3 fresh agents, blind to plan
   authorship, given the same original brief; their plurality decides.
5. **Recorded arbitrary pick:** lowest plan number among the tied positions'
   supporters wins; the ruling is marked `TIE-BROKEN (arbitrary)`.

---

## 6. Assemble the consensus design

Write `consensus/CONSENSUS.md` on this branch: one coherent governance & equity
design composed of the winning position on every decision point, in the shape
the plans themselves use (equity architecture → people → governance → legal),
each section footnoted to its tally row (`[Q9: 3/7 voting]`).

Sanity passes before publishing:

- **Coherence:** if two independently-won rulings conflict (e.g. pool
  percentages that don't sum with the reserve), re-tally those points
  **jointly** — count which combination the most plans actually held.
- **Arithmetic:** the cap table must sum to 100% after applying all equity
  rulings together.
- **Coverage:** every Q has exactly one ruling; abstention counts and
  denominators are stated per ruling.

Rulings that won with ≤ 3 of 9 supporting plans stand (the plurality rule is
absolute) but are marked `LOW CONFIDENCE` so a reader knows which parts of the
consensus rest on thin agreement.

---

## 7. Execution pipeline (agent fan-out)

1. **Extractor agents** — one per voter (9 parallel), each reading only its own
   plan's files via `git show`, emitting structured positions
   `{Q-id, position, source_file, hedged?, cited?}` against the Q-list in §2,
   plus any new decision points found.
2. **Merger** — one agent with all nine extractions: unify new Q-ids, cluster
   positions per §3. Blind to plan numbers during clustering to avoid halo
   effects; numbers re-attached afterward for the tally.
3. **Tally** — plain code, no agent: count, rank, emit `consensus/tally.md`,
   flag ties and ≤3/9 rulings.
4. **Tie-break judges** — 3 blind agents per surviving tie (§5.4 only).
5. **Writer + coherence critic** — one agent composes `consensus/CONSENSUS.md`
   from the rulings; a second agent runs the §6 sanity passes and files
   discrepancies back to step 3 for joint re-tally.

---

## 8. Outputs (all on `claude/multi-agent-consensus-j7lzgr`)

| File | Contents |
|---|---|
| `CONSENSUS_PLAN.md` | This plan |
| `consensus/claims.md` | Final decision-point list (§2 seed + additions) |
| `consensus/tally.md` | One tally table + ruling per decision point |
| `consensus/CONSENSUS.md` | The single consensus governance & equity design |

Nothing is ever written to `all-plans` or any `plans/plan-*/` directory, and no
pull requests are opened for `all-plans`, per the repo's own rules.
