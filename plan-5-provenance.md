# plan5 — Session Provenance

**Team:** plan5 · **Branches:** `plan-5` (original), `all-plans` (integration) · **Session date:** August 1–2, 2026

## What was done, in order
1. Created empty orphan branch `plan-5` as the first action (isolation preserved; no other team's branch or file was ever read, checked out, diffed, or browsed).
2. Ran the research phase (23 web searches, listed below) in six parallel batches.
3. Wrote four deliverables (`plan-5-one-pager.md`, `plan-5-design.md`, `plan-5-operating-agreement.md`, `plan-5-references.md`); committed and pushed (`e389890`).
4. Added `plan-5-conclusions.md` on owner request (`f7ddc1e`).
5. Built the `all-plans` integration branch (per-team `plans/plan-{N}/` directories, rebase-retry push protocol) and migrated plan-5 into it (`5b2a7d1`).

## Agents and model
- **Number of agents: 1.** A single main-session agent did everything; no subagents were spawned, no multi-agent workflow was used.
- **Model / effort:** an Anthropic Claude model running in Claude Code. The harness for this session runs in "undercover mode," whose policy prohibits committing the exact model identifier to repository artifacts; the identifier was disclosed to the repo owner in the session chat. The reasoning-effort setting is harness-configured and not introspectable from inside the session; no effort overrides were requested.
- **Tools used:** WebSearch (23 calls), Bash/git, file Write/Edit. WebFetch was loaded but never called — all source verification relied on live search-result content; this limitation is disclosed in `plan-5-references.md` ("Verification note").

## Every search query run (in execution order)
1. Hellmann Wasserman "The First Deal" division of founder equity Management Science equal splits
2. Breugst Patzelt perceived justice equity distribution entrepreneurial teams study
3. Ensley Hmieleski Pearce shared leadership new venture top management teams performance Leadership Quarterly
4. shared leadership meta-analysis team effectiveness Wang Waldman Zhang D'Innocenzo
5. co-CEO research shareholder returns HBR Feigen 2022 "co-CEOs" study companies
6. Wasserman founder-CEO "rich versus king" control retention firm value study
7. Slicing Pie dynamic equity split Mike Moyer model multipliers criticism
8. Carta founder equity vesting data four year vesting one year cliff percentage of companies
9. LLC to Delaware C-corp conversion venture capital investors QSBS section 1202 2025 changes $15 million
10. Massachusetts Wage Act unpaid startup employees equity instead of wages treble damages personal liability founders
11. FAST agreement advisor equity Founder Institute percentage standard advisor shares startup
12. Yale faculty conflict of interest policy equity startup consulting outside activities limits
13. profits interest LLC Rev. Proc. 93-27 2001-43 tax-free grant service provider versus capital interest 83(b)
14. "dead equity" cap table inactive founders investor problem departed founder equity data
15. Ewens Malenko startup boards board control evolution venture capital research
16. Massachusetts noncompete agreement act 2018 garden leave requirements LLC members chapter 149 24L
17. Saerom Lee "flat start-up" organizational structure hierarchy startups Strategic Management Journal research
18. shotgun clause buy-sell agreement deadlock economics research "Texas shootout" efficient partnership dissolution
19. Carta option pool size benchmark seed stage percentage 2024 2025 employee equity pool data
20. Rule 701 securities exemption equity compensation private company LLC interests 409A valuation startup
21. Yale University patent policy ownership inventions faculty university resources
22. BLS occupational employment wage statistics software developers median annual wage 2024
23. Massachusetts General Laws chapter 156C limited liability company act operating agreement mass.gov

## Commits
| Commit | Branch | Content |
|---|---|---|
| `e389890` | plan-5 | four core deliverables (root commit) |
| `f7ddc1e` | plan-5 | conclusions & executive summary |
| `5b2a7d1` | all-plans | integration structure + plan-5 migration (root commit) |
| *(this commit)* | all-plans / plan-5 | this provenance file |

## Honest limitations of process
- URL verification relied on search-engine result content rather than direct page fetches (disclosed per-source in the references file).
- Single-agent design means no independent adversarial verification pass was run on the findings; the evidence-strength ratings are the main agent's own assessment.
