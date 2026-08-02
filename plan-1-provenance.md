# Plan 1 — Provenance Report

Honest account of how Plan 1 was produced. Plan 1's original branch is
`claude/startup-governance-equity-8webj5` (created before the plan-{N} naming
convention existed); file names there are descriptive rather than plan-1-prefixed,
except `plan-1-operating-agreement.md`.

## 1. What the session did, step by step, in order

All work occurred in a single interactive session on 2026-08-02, driven by an
iterative dialogue with the founder, whose constraints arrived incrementally
(this matters for interpreting the commit history — see §7).

1. Received the initial brief: 5-founder MA LLC, ~10 employees, diverged
   contributions, inactive founders, informal two-layer equity understanding;
   requested a research-backed one-pager on governance and equity for 4–5
   founder startups.
2. Launched **three research subagents in parallel** (see §2), covering
   (a) academic literature, (b) industry practice, (c) governance & MA LLC law.
3. On subagent completion, the main agent synthesized their reports into
   `founder-governance-and-equity-one-pager.md` and preserved the three raw
   briefs under `research/`. Committed and pushed.
4. Founder fixed parameters (5% per founder max; remainder competed identically
   by founders and employees; investor-attractiveness priority) → wrote
   `implementation-plan.md`.
5. Founder asked whether a CEO is necessary → answered in chat from already-
   gathered research (no new research run).
6. Founder requested full referencing → wrote `references.md` (44 annotated
   entries) and rewrote both deliverables with inline citations.
7. Q&A rounds, each generating document updates: inactive-founder treatment;
   correction that the 5% is a use-it-or-lose-it set-aside (not a guarantee) —
   a **material design revision** replacing earlier "guaranteed base" framing;
   board seat mechanics (election, terms, independent seat, compensation).
8. Wrote `plan-1-operating-agreement.md` (19-article annotated design draft).
9. Q&A rounds continued: CEO removal mechanics; merit formula for an
   all-engineer team → `merit-formula-and-rate-table.md`; retroactive backfill
   protocol; new facts from founder (all personnel unpaid; a Yale ML professor
   promised "a decent share") → Chief Scientist rate bucket, advisor-grant
   guidance, university-IP/COI flag; market-rate-as-measuring-stick
   clarification and MA Wage Act flag for unpaid workers.
10. Drafted the replication prompt for the other teams (at founder request,
    revised once to remove design-anchoring language, e.g., the presumption of
    a single leader).
11. This integration step: copied deliverables to `plans/plan-1/`, wrote this
    provenance file.

## 2. Agents and subagents

**Four agents total: 1 main agent + 3 research subagents** (general-purpose
type, run in parallel in the background at step 2, each instructed to use web
search/fetch and return a structured brief with sources; none wrote files).

| Subagent | Task | Reported tool uses | Reported tokens |
|---|---|---|---|
| Academic | Peer-reviewed literature: founder equity splits (Hellmann & Wasserman), founder conflict, team size, dynamic vs. static splits, agency/stewardship theory, boards | 19 | ~42,300 |
| Industry | YC/Seibel, Shapiro, Slicing Pie mechanics, Carta & Index data, vesting norms, leaver provisions, LLC profits interests | 15 | ~33,600 |
| Governance | Board structures, decision tiers, one-CEO debate, founder roles, MA LLC law (c. 156C), deadlock, performance measurement, case studies | 16 | ~42,800 |

No subagents were used after step 2; all subsequent work was the main agent
synthesizing, drafting, and responding to founder questions.

## 3. Web search queries — NOT REPRODUCIBLE (disclosure)

**I cannot list the verbatim search queries.** All web searching was performed
inside the three background subagents; their reports returned findings and
source URLs but not their query logs, and the harness does not expose subagent
transcripts to the main agent (reading the raw transcript files is prohibited
as a context-overflow risk). The main agent itself ran **zero** web searches
and zero web fetches during the entire session. The tool-use counts above
(19/15/16) bound the combined number of searches+fetches per subagent, but the
split and the query strings are unknown to me. This is the largest honesty gap
in this provenance report.

## 4. Model and reasoning effort

The harness for this session prohibits writing the model identifier into
repository files; the identifier has been disclosed in the session chat
instead, per the integration task's fallback. Reasoning effort: the session's
default interactive setting; no explicit effort level was configured or is
visible to me.

## 5. Tools used

- **Main agent:** Agent (subagent launch), Write/Edit (documents), Bash (git
  only), no WebSearch, no WebFetch.
- **Subagents:** instructed to use WebSearch and WebFetch; reports indicate
  both were used, but **I cannot verify per-URL whether each cited source was
  actually fetched versus seen only in search-result snippets.** Citation
  accuracy therefore rests on the subagents' reports. A citation audit (as
  specified in the review prompt) is the appropriate check.
- One citation offered in chat from the main agent's memory (Fahlenbrach 2009,
  founder-CEO performance) was explicitly flagged to the founder as unverified
  and was deliberately **kept out of** `references.md`.

## 6. Commits (original branch `claude/startup-governance-equity-8webj5`)

| Hash | Content |
|---|---|
| 9ca43eb | One-pager + three research briefs (root commit) |
| 6a0a227 | Implementation plan (5% base + 75% merit pool) |
| 6d5594a | references.md + inline citations throughout |
| 54ce363 | Inactive-founder treatment section |
| b5e695b | Reframe 5% as use-it-or-lose-it set-aside (design correction) |
| e168f3c | Board seat mechanics |
| 844fb33 | Plan 1 operating agreement |
| 91c5de8 | Merit formula & market-rate table |
| 59ef73a | Backfill protocol |
| 5da4fd7 | Chief Scientist rate, advisor guidance, university-IP flag |
| 8a112c3 | Measuring-stick section + MA Wage Act flag |

Plus, on branch `all-plans`: one commit adding `plans/plan-1/` (deliverables +
this file), mirrored provenance commit on the original branch.

## 7. Honest limitations

1. **Search queries unreproducible** (§3) — the process cannot be replayed.
2. **No independent re-verification of citations by the main agent.** URLs and
   claims were carried from subagent reports into the deliverables; subagents
   were instructed to verify, but the main agent did not re-fetch sources.
3. **Rate-table salary figures are illustrative placeholders**, stated as such
   in the document, drawn from general knowledge rather than a live benchmark
   pull; the design requires replacing them with current Carta/Pave/levels.fyi
   data at ratification.
4. **Iterative constraint arrival caused design churn**: the "guaranteed 5%
   base" framing (commits 9ca43eb–e168f3c) was corrected to use-it-or-lose-it
   (b5e695b) when the founder clarified intent; earlier documents were revised
   but the one-pager retains some generic (non-parameterized) framing.
5. **Legal content is non-lawyer analysis** flagged for counsel throughout
   (MA c.156C, noncompete structuring, Wage Act, university IP, tax); none of
   it was reviewed by an attorney.
6. **Advocacy risk**: because design and Q&A were interleaved with one
   founder's questions, the plan may reflect that founder's framing more than
   a fully adversarial process would; the independent replication (plans 2–5)
   exists precisely to test this.
7. Some sources are practitioner-grade (blogs, vendor content); evidence-
   strength ratings in `references.md` flag this per entry.
8. This session also **authored the replication prompt** used by the other
   teams (step 10) — a structural asymmetry the reviewer should know: Plan 1
   defined the problem statement others received (facts and fixed requirements
   only; design conclusions were deliberately excluded, and the prompt was
   revised at founder direction to remove a leadership-structure presumption).
