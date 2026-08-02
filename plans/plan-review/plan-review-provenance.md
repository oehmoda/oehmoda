# plan-review — Session Provenance

**Role disclaimer, read first.** This session was not a plan team. It was the **neutral reviewer** tasked with reading *all* plan branches in full and producing a comparison report (`review.md`). The integration task's isolation rules therefore apply to this session in modified form, and this file reports that honestly rather than mimicking a plan team's attestation:

- This session **did** read, in full, every plan branch that existed on the remote at review time: `claude/startup-governance-equity-8webj5`, `plan-1`, `plan-2`, and `claude/founder-governance-equity-inactivity-sgxk74`. That was its assigned task, not a violation.
- During this integration step, this session did **not** open, read, or diff any file under any other team's `plans/plan-*/` directory on `all-plans`. It listed top-level directory names once (`ls plans/`) to confirm no collision with its own directory, observed that `plans/plan-5/` exists, and read nothing inside it.
- Consequence disclosed: **`review.md` does not cover plan-5.** No `plan-5` branch existed on the remote when the review was researched and written (verified then via `git ls-remote`); plan-5's deliverables evidently arrived directly on `all-plans` afterward or in parallel. The review states that plan-3 and plan-5 "do not exist" — true of the branch namespace at review time, now known to be incomplete for plan-5. A follow-up review pass would be needed to cover it; per the isolation rules of this integration task, this session did not peek at it while migrating.

## What the session did, step by step

1. Received the review brief (read all plan branches; produce `review.md` on branch `plan-review` with consensus map, divergence table, citation audit, gaps, verdict).
2. Fetched all remote branches; enumerated them (`git ls-remote`, `git branch -a`). Found 4 plan branches; confirmed `plan-3`/`plan-5` absent from the branch namespace. Noted the naming collision (two teams self-titled "Plan 1") and defined labels: Plan A = `claude/startup-governance-equity-8webj5`, Plan B = `plan-1`, Plan C = `plan-2`, Plan D = `claude/founder-governance-equity-inactivity-sgxk74`.
3. Extracted every file from all 4 branches via `git show <branch>:<file>` into a session scratchpad and read all 18 files in full (~390 KB total).
4. Re-computed every worked example arithmetically (Plan A's quarterly slice table; Plan B's Year-1 points table; Plan C's 15-person Year-1 table and professor units/hour comparison). All reconciled.
5. Ran the citation audit: 19 web searches (listed verbatim below) plus 2 direct-fetch attempts (both blocked by the environment's egress proxy with HTTP 403 — the same constraint Plans B and C disclose in their own bibliographies).
6. Wrote `review.md`; committed it on the designated session branch `claude/governance-equity-plan-review-7mm5t0`; pushed; created branch `plan-review` at the same commit and pushed it (as the brief required).
7. Received the integration task. Fetched and checked out `all-plans`; created `plans/plan-review/`; copied `review.md` from the `plan-review` branch via `git show plan-review:review.md`; wrote this provenance file; committed and pushed per the prescribed retry loop; mirrored this provenance file onto the `plan-review` branch (and the designated session branch) and pushed.

## Agents

**1 agent, no subagents.** All reading, verification, computation, and writing was done in a single session context. No Agent/subagent spawns, no workflows.

## Web search queries (verbatim, in execution order, all by the single main agent)

1. `Reuter v. City of Methuen Massachusetts SJC 2022 "489 Mass." OR "490 Mass." treble damages Wage Act`
2. `Miele v. Foundation Medicine Massachusetts SJC noncompetition act forfeiture nonsolicitation "Mass." reporter citation`
3. `"Reuter v. City of Methuen" "489 Mass. 465"`
4. `Carta Peter Walker co-founder departures data "by year 3" OR "within 3 years" percentage leave startup SaaStr`
5. `"co-founder" departure "before Series B" "65%" OR "by year 8" Carta founding teams`
6. `Hellmann Wasserman "First Deal" founder equity "73%" first month "one day" quick handshake equal split percentage`
7. `Gorman Sahlman 1989 "What do venture capitalists do" 95% ineffective senior management startup failure`
8. `Wasserman "Throne vs. the Kingdom" founder control "6,130" OR "17.1" OR "22.0" lower valuation Strategic Management Journal`
9. `Founder Institute FAST agreement advisor equity matrix expert tier idea stage startup stage 1.0% 0.8% percentages`
10. `QSBS section 1202 One Big Beautiful Bill July 2025 "$15 million" cap "$75 million" gross assets "50%" "75%" "100%" three four five years`
11. `Carta advisory shares data median advisor equity "0.21%" pre-seed OR "0.12%" seed`
12. `Forbes "18 common mistakes that kill startups" Y Combinator 2025 Jodie Cook "20%" founder leaves`
13. `nyu entrepreneur blog "startup board structure" 2026 board composition pre-seed founders`
14. `"Segal v. Genitrix" "478 Mass. 551" Wage Act personal liability`
15. `Hennicke Mueller "Unequal" ownership split new venture performance European Management Journal 24,194 OR "24.5%"`
16. `Carta founder equity split data "45.9%" two-founder teams equal 2024 "31.5%" 2015`
17. `Brooks Landeo Spier "Trigger Happy or Gun Shy" Texas shootouts RAND Journal partnerships experiments financial constraints`
18. `"ES NPA Holding" Tax Court "T.C. Memo. 2023-55" profits interest Rev Proc 93-27 services benefit partnership`
19. `Yale "external professional activities" faculty "one day" seven consulting limit students prohibition provost`

Direct fetch attempts (WebFetch), both returned **HTTP 403** from the egress proxy and yielded no page content:

1. `https://law.justia.com/cases/massachusetts/supreme-court/2022/sjc-13121.html`
2. `https://www.saastr.com/carta-co-founder-break-ups-are-accelerating`

## Model and reasoning effort

The harness for this session prohibits writing the model identifier into repository files; per that rule and this task's explicit allowance, the identifier is disclosed in the accompanying chat message instead of here. The session's configured reasoning-effort setting is not exposed to the model by the harness, so it is not reported; extended thinking was active during the session.

## Tools used

- `git` (Bash): branch enumeration, `git show` extraction of all plan files, commits, pushes.
- File read/write tools: reading extracted plan files; writing `review.md` and this file.
- **WebSearch**: 19 queries as listed. This is the only channel through which cited URLs were verified.
- **WebFetch**: attempted twice; blocked (403) both times.
- No subagents, no workflows, no GitHub API tools for content access.

**Fetch-vs-search disclosure:** none of the URLs cited in `review.md`'s audit was directly fetched. All verification is based on live search-engine results returning the URL together with title/excerpt content matching (or failing to match) the audited claim. This is the same verification standard Plans B and C disclosed for their own work, and it carries the same limitation: excerpts can omit context, and a small number of conclusions marked "confirmed" rest on excerpt-level rather than full-page evidence. Claims that could not be confirmed at excerpt level are labeled as such in `review.md` (e.g., the Gorman & Sahlman "95%" figure, the Hennicke & Mueller "24.5%" coefficient, the "~40% by year 8" tail).

## Commits by this session

| Hash | Branch(es) | Content |
|---|---|---|
| `562f964` | `claude/governance-equity-plan-review-7mm5t0`, `plan-review` (same commit) | `review.md` — the full comparison review |
| (this commit) | `all-plans` | `plans/plan-review/review.md` (copied unchanged from `plan-review` via `git show`) + `plans/plan-review/plan-review-provenance.md` |
| (mirror commit) | `plan-review`, `claude/governance-equity-plan-review-7mm5t0` | `plan-review-provenance.md` mirrored at branch root |

Exact hashes for the latter two are visible in `git log` on the respective branches; they are created immediately after this file is written, so they cannot be listed by hash inside the file itself.

## Honest limitations

1. **Plan-5 is not covered by the review** (explained in the role disclaimer above); plan-3 was absent everywhere and is genuinely unreviewed because it does not exist.
2. **Citation verification was search-excerpt-based, not fetch-based** (egress proxy). Reporter-citation checks (Reuter, Miele, Segal) are high-confidence because the volume/page appeared verbatim in primary-adjacent sources; some statistical confirmations rest on excerpt text.
3. **Spot-check, not census.** ~20 load-bearing claims were audited out of several hundred citations across the three citing plans. The per-plan audit summaries generalize from that sample; unaudited citations could contain errors in either direction.
4. **Single-reviewer judgment.** The divergence adjudications, gap scoring (0–2 matrix), ranking, and synthesis recommendation are one reviewer's judgment applied to the verified evidence; no adversarial second pass or panel was run.
5. **Legal conclusions are research, not legal advice**, in the review exactly as in the plans it reviews.
6. The review's arithmetic re-computations covered every worked example presented in the plans, but not every derived percentage in prose.
