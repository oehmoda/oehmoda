# plan9 — Provenance Report

Truthful account of how the plan-9 deliverables were produced. Written for cross-team comparison by a neutral reviewer; nothing here is embellished.

## 1. Session steps, in order

1. **Setup & isolation.** Confirmed the working tree was on the session's designated branch, which had **zero commits and an empty tree** — no other team's content was ever present locally. Created the empty orphan branch `plan-9` (`git checkout --orphan plan-9`; `git rm -rf .` was a no-op on the empty tree). At no point in the session was any other team's branch, file, or diff read, checked out, listed, or browsed; during this later integration step, only `plans/plan-9/` was written and no other `plans/plan-*/` directory was opened.
2. **Design skeleton.** Wrote a short internal outline (two-phase dynamic equity, governance shape, legal flags) to the session scratchpad — planning notes only, never committed.
3. **Parallel research.** Launched **three research subagents concurrently** (details §2) covering academic literature, industry/practitioner frameworks, and Massachusetts/tax/academic-affiliation legal issues, each instructed to verify every URL before reporting and to report failures honestly.
4. **Reports received** in order: legal/tax agent, then academic agent, then industry agent. All three independently reported that the sandbox egress proxy returned HTTP 403 for full-page fetches of most external hosts (see §5), and adjusted their verification method accordingly.
5. **Main-agent spot verification.** Ran 4 additional web searches from the main session (verbatim in §3.1) to verify remaining load-bearing URLs (Slicing Pie primary pages, BLS OEWS Boston tables, the YC/Seibel cofounder-equity page).
6. **Writing.** Wrote, in order: `plan-9-design.md`, `plan-9-operating-agreement.md`, `plan-9-one-pager.md`, `plan-9-references.md`. One correction during writing: an initially cited unverified URL (`fi.co/fast`) in the one-pager was replaced with the fetch-verified GitHub mirror of the FAST grid before committing.
7. **Commit & push.** Single commit `b4f9dff` with all four deliverables, pushed to `origin/plan-9`. No pull request opened.
8. **Post-delivery chat Q&A** (no repo changes): summarized the governance structure, explained the retroactive scoring mechanism, confirmed remote branch contents, and produced a neutralized rewrite of the task prompt at the user's request.
9. **Integration (this step).** Extracted the subagents' verbatim search queries from their session transcripts (targeted parsing of tool-call records only), checked out `all-plans`, copied the four files from the `plan-9` branch via `git show plan-9:<file>`, wrote this provenance file, committed under `plans/plan-9/`, pushed, and mirrored this file onto the `plan-9` branch.

## 2. Agents used

**4 total: 1 main session agent + 3 research subagents** (launched in parallel, general-purpose type, no model or reasoning-effort overrides — each inherited the session defaults).

| Agent | Task |
|---|---|
| Main session | Orchestration, design decisions, all four deliverables' writing, 4 spot-check searches, git operations |
| Subagent A ("Academic research: equity & governance") | Peer-reviewed evidence: founder equity splits, fairness/justice, dynamic vs static equity, shared vs single leadership, co-CEOs, founder retention/succession, venture boards, free-riding/social loafing, pay dispersion |
| Subagent B ("Industry research: equity frameworks") | Practitioner mechanics: Slicing Pie formulas and critiques, vesting norms, FAST advisor grid, option-pool norms, NVCA/Series Seed standards, entity choice/QSBS, founder-split data, deadlock practice |
| Subagent C ("Legal/tax research: MA LLC issues") | M.G.L. c. 156C, Donahue/Allison fiduciary doctrine, MA Wage Act/FLSA unpaid-worker exposure, profits interests (Rev. Proc. 93-27/2001-43), §83/83(b), 409A, QSBS §1202 post-OBBBA, LLC→DE C-corp conversion, Yale COI/IP policies, dispute-resolution enforceability |

No other agents, workflows, or automated pipelines were used.

## 3. Every web search query, verbatim, in execution order

Recovered by parsing the recorded tool calls in each agent's transcript after the fact; the numbering is execution order within each agent. The three subagents ran concurrently, so no total ordering across agents exists; within each agent the order is exact.

### 3.1 Main session agent — WebSearch (4)

1. `slicing pie "magic of multipliers" site:slicingpie.com`
2. `BLS OEWS software developers Boston metropolitan area occupational employment wage statistics`
3. `slicingpie.com recovery framework fired for cause resignation forfeit slices buyout`
4. `Michael Seibel "co-founder" breakup ycombinator library essay vesting divorce`

### 3.2 Subagent A (academic) — WebSearch (37)

1. `Hellmann Wasserman "The First Deal" division of founder equity Management Science 2017 findings equal splits`
2. `Breugst Patzelt perceived fairness equity distribution entrepreneurial teams justice`
3. `Hellmann Wasserman first deal equal splits percentage "within a day" negotiation lower probability financing quantitative results`
4. `"Slicing Pie" OR "dynamic equity split" founders academic study vesting renegotiation founder agreements journal`
5. `Breugst Patzelt Sheppard 2015 "How should we divide the pie" Journal of Business Venturing equity distribution entrepreneurial teams findings`
6. `D'Innocenzo Mathieu Kukenberger 2016 meta-analysis shared leadership team performance effect size Journal of Management`
7. `Wang Waldman Zhang 2014 meta-analysis shared leadership team effectiveness Journal of Applied Psychology 42 samples effect size rho`
8. `Nicolaides 2014 shared leadership team performance meta-analysis Leadership Quarterly team confidence effect size`
9. `co-CEOs firm performance study shareholder returns 9.5% Harvard Business Review Feigen co-CEO tenure`
10. `Wasserman "rich versus king" founder control firm value discount "throne" Strategic Management Journal 2017 percentage less valuable`
11. `Garg 2013 Academy of Management Review "venture boards" distinctive monitoring implications firm performance`
12. `Ewens Malenko boards of directors entrepreneurial firms VC-backed startups board control evidence`
13. `Karau Williams 1993 social loafing meta-analysis Journal of Personality Social Psychology effect size 78 studies evaluation potential`
14. `Wasserman 2003 founder-CEO succession "paradox of entrepreneurial success" Organization Science findings percentage founders replaced`
15. `Lee Kim Bae founder CEO firm value innovation "sudden deaths" Research Policy 2020 findings`
16. `pay dispersion meta-analysis team performance Downes Choi OR "horizontal pay dispersion" effects meta-analytic review`
17. `Bloom 1999 pay dispersion baseball teams Academy of Management Journal performance findings negative`
18. `Shaw 2014 "pay dispersion" Annual Review of Organizational Psychology conclusions performance sorting`
19. `Arena Ferris Unlu co-CEOs "it takes two" incidence effectiveness OR Krause Priem Love 2015 co-CEO power gap firm performance Strategic Management Journal`
20. `Erez LePine Elms 2002 rotated leadership peer evaluation self-managed teams Personnel Psychology free riding results`
21. `Wasserman "Founder's Dilemmas" 65% cofounder conflict startup failure data founder departure rate co-founder`
22. `procedural justice new venture team performance quantitative study entrepreneurial team distributive justice survival`
23. `Fahlenbrach 2009 founder-CEO firms stock market performance investment Journal of Financial Quantitative Analysis abnormal returns`
24. `Gompers Gornall Kaplan Strebulaev "how do venture capitalists make decisions" Journal of Financial Economics 2020 survey 885 board control governance`
25. `Ewens Marx "founder replacement" startup performance Review of Financial Studies findings`
26. `academic paper "dynamic equity" allocation founding teams contribution-based model entrepreneurship journal Moyer grunt fund`
27. `Hellmann Wasserman founder equity vesting percentage teams static agreements "vesting" first deal dynamic`
28. `Downes Choi 2014 "Human Resource Management Review" employee reactions pay dispersion review findings`
29. `Trevor Reilly Gerhart 2012 pay dispersion interdependent work NHL Academy of Management Journal explained dispersion performance`
30. `Weissenböck Breugst equity ownership identification founding team Applied Psychology 2024 findings`
31. `Nicolaides et al 2014 "shared leadership" meta-analysis "team performance" correlation ρ .29 OR .35 collective efficacy mediates 43 studies`
32. `Gompers Gornall Kaplan Strebulaev VC survey "management team" percentage most important factor 95% 47% deal selection`
33. `Wasserman HBR 2008 "The Founder's Dilemma" "by the time the ventures were three years old" 50% founders no longer CEO fewer than 25% IPO`
34. `Alchian Demsetz 1972 "Production, Information Costs, and Economic Organization" American Economic Review monitoring shirking team production`
35. `equal equity split founding team follow-up study replication "equal split" new venture performance evidence 2020 2021 2022 journal`
36. `"Unequal implies success" initial ownership split team entry new venture performance European Management Journal authors year`
37. `"Equity Contracts and Incentive Design in Start-Up Teams" Management Science Kagan Leider Lovejoy findings experiment equal split timing`

### 3.3 Subagent B (industry) — WebSearch (2) and GitHub code/repo searches (18)

WebSearch:
1. `slicingpie.com well formula slices multiplier 2x non-cash 4x cash`
2. `Slicing Pie criticism problems dynamic equity split investors tax`

After confirming general-web fetches were blocked (§5), this agent pivoted to GitHub-hosted primary documents and mirrors via the GitHub search tools (queries verbatim, in order):
1. [search_repositories] `series seed equity`
2. [search_repositories] `NVCA model documents`
3. [search_repositories] `founder advisor standard template FAST`
4. [search_repositories] `slicing pie`
5. [search_code] `"Slicing Pie" "multiplier" "fair market"`
6. [search_repositories] `qualified small business stock 1202`
7. [search_code] `"qualified small business stock" "$50,000,000"`
8. [search_code] `"Slicing Pie" "without cause" resign`
9. [search_code] `"statutory conversion" OR "F reorganization" repo:openaccountants/openaccountants`
10. [search_code] `"Delaware" "C corporation" "LLC" conversion "Section 351"`
11. [search_code] `"Founder Institute" advisor "1.00%" "0.25%"`
12. [search_code] `FAST advisor "Idea Stage" "Startup Stage" "Growth Stage"`
13. [search_repositories] `optionplan index ventures`
14. [search_code] `"Grunt Fund" multiplier`
15. [search_code] `"Slicing Pie" "breakeven" freeze`
16. [search_code] `"slicing pie" "fired" "cause" slices`
17. [search_code] `Seibel co-founder "vesting" divorce`
18. [search_code] `Carta founders "split equally" "45"`

### 3.4 Subagent C (legal/tax) — WebSearch (28)

1. `Reuter v. City of Methuen Massachusetts Wage Act treble damages 2022`
2. `M.G.L. chapter 156C Massachusetts limited liability company act malegislature.gov operating agreement admission of members`
3. `Donahue v. Rodd Electrotype 367 Mass. 578 utmost good faith and loyalty close corporation shareholders`
4. `M.G.L. c. 149 section 148 wage act president treasurer personal liability special contract exemption text`
5. `Massachusetts LLC fiduciary duties Donahue close corporation applied to LLC Allison v. Eriksson`
6. `Massachusetts minimum wage $15 per hour M.G.L. c. 151 section 1 oppressive and unreasonable`
7. `startup founders unpaid employees sweat equity Wage Act FLSA risk law firm equity cannot substitute for wages`
8. `FLSA employees cannot volunteer for-profit private sector employer DOL Tony Alamo Foundation waive minimum wage`
9. `DOL fact sheet 17G salary basis $684 per week executive administrative professional exemption`
10. `Rev. Proc. 93-27 Rev. Proc. 2001-43 profits interest safe harbor law firm explainer taxation`
11. `LLC employee receives profits interest becomes partner no longer W-2 employee self-employment tax dual status`
12. `capital interest for services taxable compensation FMV vs profits interest 83(b) protective election law firm`
13. `phantom equity unit appreciation rights LLC alternative to profits interest section 409A deferred compensation law firm`
14. `QSBS section 1202 OBBBA 2025 changes $15 million cap tiered 50% 75% 100% three four five years July 4 2025 law firm`
15. `LLC to C corporation conversion QSBS holding period begins at stock issuance appreciation basis benefit convert law firm`
16. `Massachusetts LLC convert to Delaware corporation chapter 156C merger no conversion statute Delaware DGCL 265`
17. `SAFE on LLC problematic convert to Delaware C corp before priced round law firm advice`
18. `Massachusetts entity conversion statute chapter 156D section 9.50 9.56 2016 act LLC convert corporation`
19. `LLC to C corp conversion tax-free section 351 assets-over interests-over methods Rev. Rul. 84-111`
20. `"156C" Massachusetts LLC operating agreement may eliminate or limit fiduciary duties liability of members managers section 8`
21. `Yale University faculty conflict of interest policy outside activities one day per week consulting equity startup`
22. `Yale patent policy university ownership inventions faculty startup license Yale Ventures`
23. `professor contributes IP to startup university may claim ownership conflict of interest management plan license tech transfer law firm`
24. `arbitration clause LLC operating agreement enforceable Federal Arbitration Act buy-sell shotgun clause enforceability law firm`
25. `Massachusetts LLC judicial dissolution 156C section 44 not reasonably practicable to carry on business`
26. `granting equity for past services taxable compensation fair market value startup retroactive founder grant law firm 83(b) 30 days`
27. `shotgun clause buy-sell agreement enforceability courts law firm operating agreement deadlock`
28. `issuing stock for services rendered past services taxable ordinary income section 83 compensatory grant startup counsel`

**Total: 71 web searches** (4 main + 37 + 2 + 28) plus 18 GitHub code/repository searches.

## 4. Model and reasoning effort

The harness configuration for this session **prohibits writing the model identifier into repository files**; per that rule, the identifier is disclosed in the session chat instead of here. All four agents (main + 3 subagents) ran on the same model — the subagents were launched with no model override and inherited the session's model. The session's reasoning-effort setting is not exposed to the agent's context, so it cannot be truthfully reported here; the subagents were launched with **no effort override** (inheriting the session default, whatever it was).

## 5. Tools used, and fetched vs. search-verified

Tools used across the session: web search; web fetch (page fetch + extraction); GitHub repository/code search and raw-file fetch (subagent B); local file read/write/edit; shell/git; targeted transcript parsing (grep/python) for §3 of this report. No workflow engine, no browser automation.

**Critical honesty point — fetch status of cited URLs.** The sandbox's egress proxy returned HTTP 403 for full-page fetches of most external hosts (confirmed against neutral hosts such as example.com and arxiv.org, so it was a session network policy, not source availability). Consequently:

- **Actually fetched and read in full [F]:** only GitHub-hosted documents — the NVCA 2020 Model Term Sheet PDF (maintained mirror, text-extracted), Series Seed docs (official repo), the Fenwick guide / og-equity-compensation / FAST grid / FAST template / YC legal-mechanics transcript mirrors, an openaccountants §1202 reference, and two third-party Slicing Pie implementation specs.
- **Search-verified only [S]:** the majority of citations, including all journal pages, statutes, cases, IRS, DOL, Yale, and law-firm URLs. For these, a live search-engine query this session returned the exact URL with its title and a content excerpt (quoted mechanics come from those returned excerpts) — but the page itself was **not** fetched. This is disclosed per-source in `plan-9-references.md` and in each deliverable's header.
- **Unverified [U]:** a small set of named leads (e.g., Cooley GO, Index Ventures OptionPlan) used for no load-bearing claim.

No cited URL was constructed from memory; every cited URL appeared verbatim in a live search result or was fetched.

## 6. Commits

| Hash | Branch | Content |
|---|---|---|
| `b4f9dff` | `plan-9` (orphan root commit) | The four deliverables: `plan-9-one-pager.md`, `plan-9-design.md`, `plan-9-operating-agreement.md`, `plan-9-references.md` (673 insertions) |
| *(this commit)* | `all-plans` | Copies of the four deliverables plus this provenance file under `plans/plan-9/` — its own hash cannot be written into a file it contains; verify via `git log all-plans -- plans/plan-9/` |
| *(mirror commit)* | `plan-9` | This provenance file mirrored to the plan-9 branch — same self-reference caveat; verify via `git log plan-9` |

No force-pushes; the original `plan-9` branch history is intact. No pull requests were opened.

## 7. Honest limitations of the process

1. **Verification ceiling.** Most sources could only be search-index-verified, not full-text read (§5). Specific numbers quoted from [S] sources (effect sizes, percentages, case holdings) came from search-result excerpts and secondary summaries and could contain transcription or context errors; the deliverables tell counsel and the founders to pull primaries before executing anything.
2. **Subagent reports were spot-checked, not fully re-verified.** The main agent independently re-searched only 4 key claims; the rest of the three research reports were accepted as written. The subagents were instructed to report only verified URLs and to disclose failures, and their (consistent) disclosure of the egress block is evidence they followed instructions, but their extraction fidelity was not independently audited source-by-source.
3. **Single-pass writing.** The deliverables were written once, without an independent adversarial review pass or a second team red-teaming the design.
4. **Illustrative numbers are illustrative.** Rate-table dollar figures and the worked cap-table example were not pulled from a live benchmark; the design says so and brackets the benchmark choice.
5. **Known gap in the evidence base.** No peer-reviewed end-to-end validation of dynamic contribution-based equity exists (searched for; none found); parameter choices (2×/4× multipliers, 5%/16-quarter reserve, 1.0% advisor grant, 30-month backstop) are market convention plus judgment, labeled as such in the deliverables.
6. **One mid-research correction.** The legal subagent's initial hypothesis that MA entity conversion runs through c. 156C §§69–72 proved wrong (it runs through c. 156D Part 9); the corrected finding is what appears in the deliverables and is flagged in the references file.
7. **Isolation was maintained**, including during this integration step: files were copied only via `git show plan-9:<file>`, and no other `plans/plan-*/` directory or team branch was listed, read, or diffed. The all-plans checkout necessarily placed other teams' directories in the working tree; none was opened.
