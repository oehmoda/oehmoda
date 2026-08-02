# plan-2 — Provenance Report

Truthful account of how the plan-2 deliverables were produced. Written for cross-team comparison; nothing here is embellished.

## 1. Session narrative, step by step, in order

1. Listed remote branch **names only** (`git ls-remote --heads origin`) to pick an unused plan number; only `claude/startup-governance-equity-8webj5` existed. Created empty orphan branch `plan-1` (`git checkout --orphan plan-1; git rm -rf .`).
2. Launched **six research subagents in parallel** (tasks in §2), each instructed to research one topic slice via web search/fetch and to verify every URL before citing.
3. While agents ran, drafted the operating-agreement deliverable (business-terms design work, not citation-dependent) and committed it. Computed the worked allocation example by hand (rates, hours, points, unit math) in a scratch file.
4. Agents completed (order: advisor/Yale, industry norms, LLC/tax, academic literature + Massachusetts law, governance). Each independently reported that **direct page fetching was blocked** by the environment's egress proxy (HTTP 403 policy denial on every external host), so all URL verification was via live web-search index results (URL + title + content excerpt matching the claim). No agent routed around the block.
5. Edited the operating agreement to reflect tax findings (retroactive grants taxable at FMV; unit holders become K-1 partners). Wrote the one-pager, then the full design document, then the annotated bibliography — synthesizing and citing only what the agents had surfaced, carrying the search-verified-not-fetch-verified caveat into every deliverable.
6. First push of branch `plan-1` was **rejected**: another team had pushed a remote `plan-1` while this session worked. That branch was never fetched, read, diffed, or checked out. Renamed the local branch and all files to `plan-2` (`sed` renumbering of internal cross-references), committed, and pushed `plan-2` successfully.
7. Answered two user questions in chat (two-line plan summary; confirmation that no other branches were inspected).
8. Integration task (this step): fetched and checked out `all-plans`; copied the four deliverables from this team's own branch only, via `git show plan-2:<file>`; extracted the verbatim search-query log below from this session's own subagent transcript files using a JSON-parsing script (no other team's artifacts touched); wrote this file; committed under `plans/plan-2/` only; pushed; mirrored this provenance file onto branch `plan-2`.

**Isolation:** at no point were any other team's branches, files, or `plans/plan-*/` directories opened, read, diffed, checked out, or browsed. The only contact with other teams' work was seeing branch *names* in `git ls-remote` output.

## 2. Agents used

**1 main agent + 6 research subagents** (launched concurrently in one batch). No other subagents, workflows, or external services were used.

| Agent | Task |
|---|---|
| Main | Orchestration, all design decisions, all four deliverables' text, worked-example arithmetic, git operations. Ran **zero** web searches and zero fetches itself. |
| Agent 1 | Academic (peer-reviewed) literature: founder equity splits, team conflict, dynamic equity, founder departure, team size |
| Agent 2 | Industry/practitioner norms: vesting, employee/advisor equity benchmarks, dynamic-equity frameworks, dead equity, cap-table optics, unpaid-work compensation |
| Agent 3 | LLC equity instruments and taxation; entity strategy for VC investability (profits interests, §83, 83(b), QSBS/OBBBA, conversion) |
| Agent 4 | Massachusetts law: c. 156C, close-company fiduciary duties/freeze-out, noncompete act, Wage Act, dissolution/deadlock |
| Agent 5 | Academic-advisor issues: Yale consulting/COI/patent policies, advisor-equity norms, university IP risk, oral equity promises |
| Agent 6 | Startup governance: board composition norms, CEO selection/removal, co-CEO evidence, decision rights, deadlock mechanisms |

## 3. Every web search query, verbatim, in execution order, by agent

All queries were run with the harness `WebSearch` tool. The six agents ran **concurrently**, so there is no meaningful global ordering across agents; within each agent, queries are listed in exact execution order. Total: **151 searches**. The main agent ran none.

### Agent 1 — academic founder-equity literature (22 queries)
1. Hellmann Wasserman "The First Deal" "Division of Founder Equity" Management Science 2017 equal split
2. Breugst Patzelt Rathgeber "perceived justice" equity distribution entrepreneurial teams Journal of Business Venturing 2015
3. Hellmann Wasserman "First Deal" founder equity PDF "equal split" percentage teams "one third" OR "32%" OR "33%" negotiation "a day or less"
4. Wasserman "Founder's Dilemmas" data 10000 founders "rich versus king" percentage founder CEO replaced "three years" fired board
5. Wasserman 2003 Organization Science "Founder-CEO succession and the paradox of entrepreneurial success" sample findings
6. Wasserman HBR 2008 "The Founder's Dilemma" "65%" fail management OR conflict co-founders "80%" reluctant give up CEO
7. Klotz Hmieleski Bradley Busenitz 2014 "New venture teams" review Journal of Management findings team composition turnover
8. Eisenhardt Schoonhoven 1990 founding team size growth semiconductor ventures Administrative Science Quarterly findings
9. Ensley Pearson Amason 2002 "new venture top management teams" cohesion conflict performance Journal of Business Venturing sample Inc. 500
10. Ruef Aldrich Carter 2003 "The structure of founding teams" American Sociological Review homophily sample PSED findings equal ownership
11. Kotha George 2012 "Friends, family, or fools" entrepreneur experience equity distribution resource mobilization Journal of Business Venturing findings
12. "Hellmann" "Wasserman" founder equity "within a day" OR "one day or less" negotiate equal split vesting percentage founders survey CompStudy
13. Patzelt entrepreneurial team member exit systematic review "Review of Managerial Science" 2021 findings frequency exits
14. Boeker Karichalil 2002 "founder departure" Academy of Management Journal entrepreneurial transitions sample findings
15. academic study "dynamic equity" OR "vesting" founders startup performance Hellmann Thiele "contracting" founder agreements economics
16. Hellmann "Ownership dynamics within founder teams" Strategic Entrepreneurship Journal 2019 external financing sample findings
17. Gorman Sahlman 1989 "What do venture capitalists do" Journal of Business Venturing failure attributed senior management percentage
18. Greenberg Mollick "Sole survivors" solo ventures versus founding teams performance findings crowdfunding
19. Wasserman "65%" high-potential startups fail "people problems" OR "co-founder" conflict Founder's Dilemmas source
20. "First Deal" Hellmann Wasserman "negotiated" "a day or less" percentage teams equal split larger teams less likely
21. "How should we divide the pie" Breugst "eight" teams six months justice equity spirals abstract
22. Wasserman "The throne vs. the kingdom" founder control value creation Strategic Management Journal 2017 sample valuation lower percentage

### Agent 2 — industry equity norms (34 queries)
1. Carta data percentage of grants 4-year vesting one-year cliff standard
2. Holloway Guide to Equity Compensation vesting 4 years one year cliff
3. Index Ventures OptionPlan rewarding talent option pool size employee equity benchmarks
4. FAST agreement Founder Institute advisor equity tiers 0.25% 1%
5. Carta equity benchmarks employee equity by role stage engineer percentage
6. Slicing Pie Mike Moyer grunt fund multipliers 2x cash 1x time fair market rate
7. Frank Demmler Founders Pie Calculator equity split
8. Fred Wilson AVC founder vesting dead equity blog post
9. Carta "dead equity" cap table founder departed
10. Cooley GO founder stock vesting repurchase right back vesting
11. Y Combinator guide founder vesting standard four year cliff
12. double-trigger acceleration prevalence startups single trigger data
13. Carta founder ownership dilution by stage seed Series A median
14. Carta advisor equity data median advisor grant percentage
15. Slicing Pie criticism problems tax investor perception dynamic equity
16. deferred compensation startup unpaid founder work convert to equity risks wage law
17. "scientific advisory board" equity percentage biotech advisor 0.25% 1% norms
18. investor cap table red flags too many small shareholders clean cap table VC guidance
19. ycombinator.com how to split equity co-founders vesting site:ycombinator.com
20. founder joins later "vesting credit" OR "back vesting" time already served startup
21. carta.com "vesting" learn cliff "one-year" percentage of cliffs acceleration double trigger
22. Index Ventures rewarding talent ESOP size seed 10% US startups 15-20%
23. FAST agreement grid growth stage expert 0.6% startup 0.8% idea 1.0% monthly vesting
24. AVC "Employee Equity: Vesting" Fred Wilson 2010 four year vest
25. Holloway "how equity is granted" option pool "10%" OR "15%" OR "20%" employee equity ranges
26. Slicing Pie recovery framework departure fired for cause without cause resignation slices buyout
27. Perkins Coie "Dealing with Dead Equity" founder shares repurchase
28. TechCrunch "solve the dead equity problem" longer founder vesting schedule author
29. Carta data first hire equity median employee 1 through 10 grant size Peter Walker
30. carta.com advisory shares "0.21%" OR "0.12%" advisor equity pre-seed seed median
31. YC "how to split equity among co-founders" library Michael Seibel equal split vesting
32. AVC 2011 "how to allocate founder and employee equity" formula best people
33. Index Ventures rewarding talent seed option grants first hires percentage benchmarks VP engineer
34. YC founder breakup departed co-founder equity buyback advice a16z founder vesting cap table

### Agent 3 — LLC equity & tax (22 queries)
1. Rev. Proc. 93-27 profits interest safe harbor IRS
2. Rev. Proc. 2001-43 profits interest vesting safe harbor
3. Rev Proc 93-27 full text irs.gov pdf "profits interest" 1993
4. Holland Knight profits interests LLC equity compensation explained
5. profits interest holder cannot be W-2 employee self-employment partner dual status Rev Rul 69-184
6. Carta profits interest guide equity incentive plans LLC threshold amount
7. LLC options unit appreciation rights phantom equity why LLC options are rare messy tax
8. why VCs require Delaware C corporation not LLC startup investment Cooley
9. QSBS section 1202 OBBBA 2025 changes $15 million tiered holding period 3 4 5 years $75 million asset limit
10. LLC to C corporation conversion Rev Rul 84-111 assets-over assets-up interests-over statutory conversion section 351 tax-free
11. 83(b) election 30 day deadline IRS instructions restricted stock partnership interest
12. capital interest granted for past services taxable compensation income fair market value section 83 partnership
13. profits interest holders self-employment tax K-1 guaranteed payments estimated taxes quarterly practical implications employees
14. Massachusetts LLC convert to Delaware corporation statutory conversion merger domestication Massachusetts does not allow conversion
15. QSBS timing LLC conversion sooner vs later 10x basis appreciation holding period starts at incorporation Fenwick
16. Cooley GO LLC vs corporation formation venture financing "profits interests"
17. protective 83(b) election profits interest why file "profits interest" 83(b) safe harbor fails
18. employee becomes partner tax consequences no withholding lose cafeteria plan benefits quarterly estimated taxes profits interest grant practical
19. converting LLC to corporation before venture financing law firm memo Fenwick Goodwin "conversion" Delaware timing series A
20. hklaw.com OR foley.com profits interests LLC equity incentive alert
21. 26 USC 1202 qualified small business stock text law.cornell.edu OR IRS Form 15620 section 83(b) election
22. Massachusetts chapter 156C LLC no statutory conversion provision merger into Delaware corporation to reincorporate

### Agent 4 — Massachusetts law (26 queries)
1. Massachusetts LLC Act Chapter 156C operating agreement fiduciary duties malegislature.gov
2. Allison v. Eriksson 2018 SJC LLC freeze-out fiduciary duty Massachusetts
3. Massachusetts Noncompete Agreement Act G.L. c. 149 section 24L garden leave equity holders members applicability
4. Massachusetts Wage Act unpaid startup founders treble damages equity in lieu of wages law firm
5. "chapter 156C" "section 24" management of limited liability company vested in members Massachusetts text
6. "chapter 156C" "section 36" resignation of member Massachusetts LLC withdraw
7. "chapter 156C" "section 40" charging order judgment creditor Massachusetts LLC text
8. "chapter 156C" "section 43" dissolution "not reasonably practicable" Massachusetts LLC judicial dissolution deadlock
9. "156C" section 9 records information member access LLC Massachusetts "section 10" operating agreement
10. Massachusetts LLC Act default rules profits distributions allocated per capita "section 28" OR "section 29" 156C voting
11. Donahue v. Rodd Electrotype 367 Mass. 578 Wilkes v. Springside 370 Mass. 842 legitimate business purpose test freeze-out apply to LLC Pointer v. Castellani
12. Massachusetts noncompete act 24L exclusions nonsolicitation "sale of a business" separation agreement nonexempt employees students independent contractors
13. Cook v. Patient Edu LLC 465 Mass. 548 Wage Act individual liability LLC managers Reuter v. Methuen treble damages
14. unpaid interns volunteers for-profit company illegal Massachusetts minimum wage law FLSA primary beneficiary test law firm explainer
15. Massachusetts G.L. c.149 section 148 "special contract" no waiver text section 150 treble damages private right of action c.151 minimum wage $15
16. Massachusetts LLC expel member involuntary redemption operating agreement 156C no statutory expulsion provision
17. "156C" "section 21" consent members "more than fifty percent" unreturned contributions voting default "section 29" allocation of distributions
18. Massachusetts noncompete law 12 month maximum restricted period exempt nonexempt employees students under 18 terminated without cause laid off
19. Stanton Lighthouse Financial Services co-founder employee Wage Act deferred salary special contract unenforceable
20. Massachusetts LLC operating agreement can modify fiduciary duties section 63 law firm explainer freedom of contract close corporation Blank v. Chelmsford
21. Donahue v. Rodd Electrotype "367 Mass. 578" 1975 "utmost good faith and loyalty" close corporation masscases
22. Steffans Legal Raleigh Lighthouse shareholder LLC member Wage Act claim employee
23. Massachusetts 156C "section 2" definition "operating agreement" "written or oral" agreement of members
24. Massachusetts LLC judicial dissolution "not reasonably practicable" deadlock case law Superior Court 156C section 44 standard
25. Koshy v. Sachdev 477 Mass. 2017 true deadlock corporate dissolution 156D 14.30
26. "156C" "section 32" distribution upon resignation "fair value" limited liability company interest Massachusetts

### Agent 5 — academic advisor / Yale (19 queries)
1. Yale Faculty Handbook outside consulting one day per week policy
2. Yale University conflict of interest policy faculty equity startup disclosure
3. Yale Patent Policy inventions faculty Office of Cooperative Research ownership
4. Yale policy faculty start-up companies students involvement supervision conflict
5. Perkmann academic engagement commercialisation review literature faculty consulting Research Policy
6. startup advisor equity how much percent FAST agreement Founder Institute 0.25% 1%
7. scientific advisory board equity biotech professor advisor 0.1% to 0.5% vesting four years
8. university spinout faculty advisor intellectual property assignment risk law firm guidance consulting agreement carve-out university obligations
9. oral promise of equity startup enforceability statute of frauds quantum meruit advisor sued for shares
10. handshake equity promise dispute lawsuit startup "promised equity" law firm commentary get it in writing
11. Fenn v. Yale University patent dispute professor electrospray Nobel assigned invention ruling
12. Cooley GO advisor equity agreement academic founder "university" IP representation no university resources
13. "Engaging Advisors From Universities" Cooley institution policies IP consulting agreement conflict pre-existing obligations
14. Yale "conflict of interest" policy "start-up" appendix faculty equity "Significant Financial Interest" research
15. Yale Faculty Handbook "one day" seven-day week consulting "outside" section provost pdf
16. Siegel Wright academic entrepreneurship rethink Small Business Economics university conflict of interest management
17. case advisor sued startup over promised stock "quantum meruit" shares oral agreement court decision
18. Yale Ventures consulting guidance faculty "consulting agreement" IP patent policy equity terms
19. scientific co-founder "chief scientific advisor" equity 1% 2% university professor spinout founding scientist

### Agent 6 — startup governance/boards (28 queries)
1. startup board composition by stage seed Series A Carta data board members founders investors
2. Wasserman "rich versus king" founder CEO control tradeoff study
3. Garg "venture boards" Academy of Management Review 2013 distinctive monitoring
4. Hellmann Puri 2002 venture capital professionalization founder CEO turnover Journal of Finance
5. NVCA model term sheet protective provisions list voting agreement board composition
6. co-CEO arrangements research evidence HBR "co-CEOs" performance shared leadership
7. Y Combinator advice choosing CEO among co-founders one CEO decision making
8. shotgun clause buy-sell agreement problems capital asymmetry "Texas shootout" deadlock law firm
9. Wasserman founders dilemma HBR 2008 "by the time the ventures were three years old" 50% founders no longer CEO
10. Brad Feld Startup Boards board composition seed stage recommendation "Startup Boards" book
11. Cooley GO board of directors seed deals percentage board seat venture financing report
12. Bain research "decide and deliver" seven people decision effectiveness 10% rule group size
13. First Round Review co-founder CEO decision who should be CEO startup
14. LLC operating agreement supermajority provisions list admission of new members sale of company annual budget compensation
15. deadlock resolution LLC shareholders agreement mediation escalation baseball arbitration independent director tie-breaker mechanisms
16. "It Takes Two" incidence effectiveness co-CEOs Arena Ferris Unlu Financial Review
17. Yermack 1996 board size firm valuation smaller boards higher market value study
18. removing founder CEO startup mechanics board vote founder vesting "for cause" cure period notice
19. YC "series A term sheet" standard board "common stockholders" director composition Aaron Harris
20. Michael Seibel YC why every startup needs one CEO co-founder decide CEO
21. "who should be CEO" co-founders startup advice one accountable leader venture capital blog
22. Carta board of directors data seed Series A independent seats founders
23. model legal documents term sheet voting agreement
24. series A term sheet board directors common stock elect preferred director
25. cofounders tactical guide CEO decision disagreements
26. "how to create and manage a board" YC startup library board size seed stage
27. founder CEO removal employment agreement "cure period" written notice board resolution law firm startup explainer
28. Wasserman founder's dilemma "four out of five" founder-CEOs forced to step down

## 4. Model and reasoning effort

The harness operating this session **prohibits writing the model identifier into repository files**; per that instruction, the identifier is disclosed in the chat conversation instead of here. The same model powered the main agent and all six subagents (subagents inherited the session model; no per-agent model overrides were set). The session's reasoning-effort setting is not exposed to the model itself, so it is not reported here rather than guessed.

## 5. Tools used, and fetch-vs-search honesty

- **WebSearch** (subagents only): 151 queries, listed above. **This is the sole source of every citation.**
- **WebFetch** (subagents only): **45 attempts, every one blocked** by the environment's egress proxy with an HTTP 403 policy denial (confirmed by the agents at the proxy status endpoint; hosts included irs.gov, malegislature.gov, yale.edu, carta.com, hbr.org, ssrn.com, nber.org, and even example.com). Agent 5 additionally attempted two archive.org/Wayback fallback URLs, which were **also blocked**; no content was obtained from any fetch by any agent. **Therefore: no cited URL was ever actually fetched.** Every URL was verified only by appearing in live search-engine results with a title and content excerpt matching the claim cited to it. This caveat is stated in all four deliverables.
- **Bash / file tools** (main agent): git operations, file writing/editing, arithmetic scratch work, and a JSON-parsing script over this session's **own** subagent transcript files to extract the query log above.
- **Agent tool**: to launch the six subagents.
- No other data sources (no GitHub browsing of other branches, no MCP data tools, no prior-session material, no memorized-URL citation).

## 6. Commit table

| Hash | Branch | Content |
|---|---|---|
| `e996d37` | plan-1 → plan-2 (renamed) | Business-terms draft of the operating agreement (initial version, pre-research-integration edits) |
| `0a78725` | plan-1 → plan-2 (renamed) | All four deliverables complete (one-pager, design, references; operating agreement updated with tax flags) |
| `1062697` | plan-2 | Renumbering: branch and files renamed plan-1 → plan-2 after the push rejection revealed another team had claimed remote `plan-1`; internal cross-references updated |
| (integration commit) | all-plans | `plans/plan-2/`: the four deliverables copied verbatim from branch `plan-2` via `git show`, plus this provenance file |
| (mirror commit) | plan-2 | This provenance file added to the team's own branch |

(The two integration-step hashes are created after this file is written; they are visible in `git log` on their branches.)

## 7. Honest limitations

1. **No cited URL was directly fetched.** All verification is search-index-level (URL + title + excerpt). Quotes and figures are as returned by search excerpts; a reviewer or counsel should load primary pages before relying on any single figure.
2. **A few figures rest on secondary reporting** and are flagged in-line where used: the "~65% co-founder departure before Series B" stat (Carta data via SaaStr), the Stanton and Raleigh Wage Act case summaries (law-firm blogs, not opinions), and a claimed 2026 FAST-agreement revision (single secondary source; not relied on).
3. **The evidence base is correlational.** No causal studies exist for the core equity-split claims; the design document says this explicitly (its §12) and the bibliography rates every source A–E.
4. **No peer-reviewed validation exists for any dynamic-equity framework** (Slicing Pie multipliers, Demmler factors). Their constants were adopted as transparent conventions, and the calibration constants in the design (multipliers, vision cap, hour thresholds, block sizes) are judgment, labeled as such.
5. **The worked allocation example uses illustrative rates and hours**, hand-computed; the real system requires the adopted Rate Card and audited hours. Arithmetic was checked manually, not by an independent tool.
6. **Single-pass authorship.** The deliverables were synthesized by one main agent from six research reports; no independent adversarial review pass or second-opinion agent was run over the final documents.
7. **Massachusetts/tax/securities conclusions are business-level, not legal advice**; securities-law compliance for 15+ holders was explicitly not researched (flagged as out of scope in the design's risk register).
8. **Branch-name collision handling:** the session began on `plan-1`; after another team pushed a remote `plan-1` mid-session, this team renamed to `plan-2` without ever fetching or viewing the other branch. Earlier commit messages on this team's branch therefore still say "plan-1:"; the content is unaffected.
