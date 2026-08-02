# plan-7 — Provenance Report

Truthful account of how the plan-7 deliverables were produced. Written 2026-08-02.

## 1. What the session did, step by step

1. Session started in a fresh clone of `oehmoda/oehmoda` with an unborn (empty) branch checked out; no repository files were present, and **no other team's branch or content was ever read, checked out, diffed, or browsed** at any point in the session.
2. Created empty orphan branch `plan-7` (`git checkout --orphan plan-7`; `git rm -rf .` was a no-op on the empty tree).
3. Launched **5 parallel background research subagents** (see §2), each instructed to research an assigned topic area and to verify every cited URL by fetching it.
4. Drafted a pre-research framework skeleton in the session scratchpad (candidate architecture and open questions to resolve against evidence).
5. Received the completion report of the advisor/professor research subagent, including its finding that the sandbox's egress proxy blocked direct fetches (HTTP 403 policy denial) to essentially all non-GitHub hosts, limiting URL verification to search-index corroboration.
6. The session was then interrupted; over several conversational turns the user asked design questions (one-line structure summary; board size; who elects the board and who sits on it; whether annually elected leadership is investor-acceptable; measuring the unrecorded Year 1; handling inactive members). Answers given in chat were consistent with, and became part of, the final design (3-member elected board with financing sunset; Year-1 coarse banding with blind peer rating; earned-equity-is-kept treatment of inactive founders).
7. On receiving the integration task: discovered the four remaining subagent tasks were no longer in the task registry (lost in the interruption). Their transcript files had survived on disk; the final report text and the verbatim WebSearch queries were extracted from those transcripts with targeted `jq` filters (only assistant text and tool-use query fields were extracted; full transcripts were not loaded).
8. Read all five research reports; synthesized and wrote the four deliverables (`plan-7-one-pager.md`, `plan-7-design.md`, `plan-7-operating-agreement.md`, `plan-7-references.md`) directly in the main session (no writing subagents).
9. Committed the four deliverables to orphan branch `plan-7` (single root commit) and pushed `plan-7` to origin.
10. Fetched and checked out `all-plans`; copied plan-7's four files into `plans/plan-7/` using only `git show plan-7:<file>` (no other team's directory was listed, opened, or read); wrote this provenance file; committed and pushed to `all-plans`; mirrored this provenance file onto branch `plan-7` and pushed it there as a second commit.

## 2. Agents used

**6 total contexts: 1 main (orchestrating/writing) agent + 5 research subagents.** All research subagents ran concurrently in the background. Their tasks:

| # | Subagent task |
|---|---|
| 1 | Academic literature on founder equity splits, dynamic vs. static agreements, free-riding/effort incentives, fairness/procedural justice, splits vs. fundraising/survival |
| 2 | Practitioner/industry: Slicing Pie mechanics and critiques, alternative frameworks, Carta/Index/Pave/Holloway market data, YC guidance, retroactive sweat-equity valuation, LLC equity vehicles |
| 3 | Legal/tax: LLC vs. Delaware C-corp and QSBS (incl. OBBBA), conversion mechanics, Massachusetts Wage Act / misclassification / c.156C, profits interests / 83(b) / 409A, founder vesting norms, MA fiduciary-duty and freeze-out case law |
| 4 | Advisor/professor: FAST and advisor-equity benchmarks, academic advisory norms, Yale COI/external-activity/IP policies, informal-promise enforceability, differential "star" rates |
| 5 | Governance: single vs. shared leadership evidence, decision speed/consensus, investor board norms and NVCA documents, deadlock mechanisms, role clarity and founder-team size |

The main agent wrote all deliverable text; subagents contributed research findings only.

## 3. Every web search query, verbatim, in execution order

All 131 web searches were run by the five subagents (the main agent ran zero). The five subagents ran **concurrently**, so a single global interleaving order is not recoverable; within each subagent, queries are listed in exact execution order.

### Subagent 1 — academic founder-equity literature (29 queries)
1. Hellmann Wasserman "The First Deal" division of founder equity Management Science 2017 equal split findings
2. Breugst Patzelt Rathgeber "How should we divide the pie" Journal of Business Venturing 2015 findings
3. Hellmann Wasserman first deal "equal split" percentage "quick handshake" valuation discount pre-money founders negotiation days
4. Wasserman Founder's Dilemmas equity split "within a month" percentage founders vesting data CompStudy survey
5. Holmstrom 1982 "Moral Hazard in Teams" Bell Journal of Economics free-rider problem budget breaker key result
6. Kandel Lazear 1992 "Peer Pressure and Partnerships" Journal of Political Economy findings profit sharing mutual monitoring
7. founder departure equity turnover startup research "founder exits" entrepreneurial team member exit empirical study
8. Ucbasaran Lockett Wright Westhead entrepreneurial team member entry exit turnover 2003 findings percentage
9. Kaplan Stromberg "Financial Contracting Theory Meets the Real World" founder vesting percentage VC contracts
10. Kaplan Stromberg 2003 venture capital contracts "vesting" founder shares "41%" OR "40%" OR percentage of financings sample 213
11. equal equity split startup performance survival empirical study founding teams "equal split" venture performance regression
12. "Unequal implies success" initial ownership split team entry new venture performance European Management Journal authors German startups
13. Wasserman "throne vs kingdom" Strategic Management Journal 2017 founder control firm value lower valuation percentage
14. "Equity Contracts and Incentive Design in Start-Up Teams" Management Science authors findings
15. Ewens Marx "Founder Replacement and Startup Performance" Review of Financial Studies findings percentage
16. Wasserman "65%" high-potential startups fail cofounder conflict "Founder's Dilemmas" source statistic
17. Kotha George 2012 Journal of Business Venturing entrepreneur experience equity distribution resource mobilization "helpers" findings
18. Kagan Leider Lovejoy equity contracts startup teams experiment equal split performance-based timing findings laboratory
19. Nalbantian Schotter 1997 "Productivity Under Group Incentives" American Economic Review experiment findings free riding
20. "dynamic equity" split research renegotiation founder agreement academic study "equity split" adjust over time vesting entrepreneurial team
21. Bapna Ganco gender gap founder equity splits Management Science 2022 findings women founders percentage
22. "gender gap in the first deal" equity split founding teams Journal of Banking and Finance 2024 authors findings women founders receive
23. perceived justice fairness entrepreneurial team equity distribution conflict study distributive procedural justice new venture team
24. Carta data founder equity split equal percentage two-founder teams 2024 trends
25. Hellmann Wasserman founder equity "idea premium" percentage points serial entrepreneur capital contribution equity stake regression
26. Breugst Patzelt Rathgeber equity distribution teams renegotiation "equity split" changed adjustments case study spirals attraction repulsion details
27. free riding new venture teams empirical study effort equity stake entrepreneurial team members shirking
28. "Effort provision in entrepreneurial teams" team size free-riding peer pressure Journal of Business Economics authors findings inverted U
29. Narayanan "Distributing Start-Up Equity" Journal of Small Business Management 2019 theoretical foundation emerging practice dynamic equity slicing pie

### Subagent 2 — dynamic-equity practice & market data (22 queries)
1. Slicing Pie Mike Moyer dynamic equity model multipliers 2x cash 4x non-cash slices
2. Frank Demmler Founders Pie Calculator equity split weights
3. Slicing Pie recovery framework leaving company fired for cause resignation slices "well" buyback
4. Slicing Pie critique problems startup lawyer VC "dynamic equity" criticism
5. Carta data early employee equity first 10 employees percentage hire number
6. Index Ventures OptionPlan benchmarks option pool size employee equity seed Series A percentages
7. Carta data founder vesting schedule 4-year one-year cliff percentage of founders
8. Michael Seibel YC essay founder equity split "nearly equal" why equal splits vesting
9. BLS OES software developers median annual wage May 2024 occupational employment statistics
10. profits interests LLC explained law firm employee equity capital interest 83(b) hurdle amount threshold value
11. phantom equity plan LLC unit appreciation rights law firm explainer vs profits interest tax treatment
12. Slicing Pie "bake" freeze pie breakeven Series A termination of the model fair market value hourly rate salary calculation
13. Y Combinator standard deal $500,000 "$125,000" 7% safe MFN terms
14. Holloway Guide to Equity Compensation typical employee equity ranges hire 1-10 option pool 10-20%
15. converting deferred unpaid salary into equity startup framework risk premium discount sweat equity retroactive
16. Carta median option pool size seed stage percentage fully diluted data Peter Walker
17. Vestd "slicing pie" critique problems UK tax valuation issues dynamic equity
18. "Slicing Pie" recovery framework table "terminated without cause" keeps slices "terminated with cause" loses non-cash slices multiplier removed
19. Leo Polovets AngelList data equity first hires "employee #1" percentage salary tradeoff
20. Slicing Pie "the Well" cash contributions convert slices when spent grunt fund definition
21. Pave compensation benchmarking data equity software engineer startup percentage benchmarks 2025
22. co-founder equity split calculator foundrs.com alternatives dynamic equity split spreadsheet startup

### Subagent 3 — legal/tax structuring (25 queries)
1. Cooley GO why Delaware C-corp not LLC venture capital startup
2. QSBS section 1202 OBBBA 2025 changes $15 million cap tiered holding period July 4 2025
3. UBTI unrelated business taxable income venture capital fund tax-exempt limited partners LLC investment blocker corporation
4. QSBS section 1202 requirements $10 million 10x basis five year holding C corporation $50 million aggregate gross assets active business 80 percent
5. convert LLC to Delaware C corporation statutory conversion merger section 351 tax-free assets-over interests-over law firm
6. LLC to C-corp conversion QSBS holding period begins at conversion basis fair market value 1202(i) built-in gain
7. Massachusetts Wage Act M.G.L. c.149 s.148 treble damages personal liability president treasurer managers LLC
8. unpaid founders startup employees deferred compensation Massachusetts Wage Act equity instead of wages risk
9. Massachusetts independent contractor law 148B three prong ABC test misclassification presumption employee
10. Massachusetts minimum wage 2026 $15 per hour M.G.L. c.151 payment frequency weekly biweekly Wage Act six days
11. profits interest Rev. Proc. 93-27 Rev. Proc. 2001-43 safe harbor liquidation value unvested no taxable event
12. 83(b) election 30 days deadline restricted stock founders IRS section 83 consequences of missing
13. what happens to profits interests when LLC converts to C corporation vesting rollover stock options
14. ISO vs NSO incentive stock option $100,000 limit 409A valuation safe harbor 12 months exercise price fair market value
15. founder vesting Series A investors expect four year vesting one year cliff reverse vesting restricted stock Cooley Carta
16. Donahue v. Rodd Electrotype 367 Mass. 578 utmost good faith and loyalty close corporation freeze-out Wilkes v. Springside
17. Massachusetts LLC members fiduciary duties chapter 156C freeze-out close corporation standard applied to LLC members case law
18. Massachusetts Limited Liability Company Act chapter 156C default rules operating agreement per capita voting distributions
19. Cook v. Patient Edu LLC Massachusetts SJC wage act managers limited liability company personal liability
20. Massachusetts LLC convert to Delaware corporation chapter 156C merger section 59 60 Delaware DGCL 265 conversion mechanics
21. Stripe Atlas Y Combinator why Delaware C corporation standard startup incorporation ISOs QSBS guide
22. Orrick convert LLC to corporation before financing while valuation low tax timing QSBS "conversion"
23. 409A valuation safe harbor independent appraisal presumption 12 months rebuttable stock options deferred compensation penalties 20%
24. "Stanton v. Lighthouse Financial Services" citation D. Mass. wage act deferred salary founder president
25. Massachusetts Wage Act three year statute of limitations section 150 private right of action Attorney General complaint misclassification penalties

### Subagent 4 — advisor/professor equity & Yale (21 queries)
1. FAST agreement Founder Institute advisor equity percentage grid stage engagement
2. Yale faculty conflict of interest policy startup equity consulting one day per week
3. Carta data advisor equity grants median percentage startup advisors
4. Holloway guide equity compensation advisors typical 0.1% to 0.5% vesting
5. "FAST agreement" advisor equity grid idea stage startup growth "1.0%" OR "0.6%" OR "0.8%" standard strategic expert
6. FAST agreement grid "0.25%" "0.50%" "1.00%" idea "0.20%" "0.40%" "0.80%" startup "0.15%" "0.30%" "0.60%" growth
7. Yale patent policy royalty share inventor Office of Cooperative Research assignment inventions university resources
8. Yale patent policy faculty invention "significant use" university facilities ownership assign policy 2110
9. Yale Ventures faculty startup guidance equity conflict of interest management plan leadership role company
10. scientific advisory board equity biotech startup percentage 0.1% 0.5% professor SAB member typical
11. academic co-founder professor equity part-time AI startup how much equity technical founder stays at university
12. oral promise of equity startup lawsuit promissory estoppel quantum meruit "promised equity" enforceable statute of frauds
13. AI machine learning expert consulting hourly rate $300 $500 $1000 professor consultant expert witness rates
14. Sam Altman advisor equity blog OR First Round Review "how much equity" advisors board members
15. expert witness hourly rate machine learning computer science professor $500 $800 per hour litigation SEAK survey
16. Fenn v. Yale University patent dispute professor invention ruling breach fiduciary duty
17. cleaning up informal verbal equity promises startup best practice paper advisor agreement lawyer commentary handshake deal litigation
18. Slicing Pie dynamic equity split fair market rate multiplier non-cash contribution 2x argument against fixed equal split
19. Yale conflict of interest policy significant financial interest threshold $5,000 equity disclosure faculty research
20. AI professor advisor equity stake startup famous academic advisors "advisory shares" machine learning faculty affiliation disclosure
21. Yale Ventures "consulting guidance" faculty consulting agreement IP carve-out publication rights

### Subagent 5 — governance & leadership evidence (34 queries)
1. Krause Priem Love co-CEOs Strategic Management Journal "co-CEO" firm performance study
2. HBR 2022 "Is It Time to Consider Co-CEOs" study co-CEO shareholder returns 9.5%
3. D'Innocenzo Mathieu Kukenberger meta-analysis shared leadership team performance effect size correlation
4. Wang Waldman Zhang 2014 meta-analysis shared leadership 42 samples team effectiveness
5. Ensley Hmieleski Pearce 2006 vertical shared leadership new venture top management teams performance
6. Wasserman "rich versus king" founder CEO control wealth tradeoff study percentage valuation
7. "The Founder's Dilemma" Wasserman HBR 2008 "by the time the ventures were three years old" 50 percent founders no longer CEO 212 startups
8. Eisenhardt 1989 "Making Fast Strategic Decisions in High-Velocity Environments" fast decision makers more information better performance eight microcomputer firms
9. Baum Wally 2003 strategic decision speed firm performance growth profitability study
10. Malmendier Tate CEO overconfidence investment corporate decisions evidence overpay acquisitions
11. Hellmann Wasserman "The First Deal" division of founder equity equal splits Management Science negative outcomes
12. Sah Stiglitz hierarchies polyarchies decision making aggregation errors committees economics
13. Cooley GO seed Series A board composition typical 2-1 3-2 common investor independent director norms
14. Hellmann Puri 2002 venture capital professionalization startups Journal of Finance evidence CEO turnover stock option plans
15. Brooks Landeo Spier "Trigger Happy or Gun Shy" Texas shootouts RAND Journal of Economics shotgun clause common value partnerships
16. shotgun buy-sell clause deadlock closely held corporation law review analysis efficiency
17. NVCA model legal documents voting agreement board composition protective provisions Series A standard
18. Greenberg Mollick solo founders study "sole founders" outperform teams survival revenue crowdfunding
19. Wasserman founder team conflict equity split percentage cofounder disputes "65%" startups fail co-founder conflict
20. founding team size startup success optimal number founders research data First Round Startup Genome two founders
21. Krause Semadeni Cannella CEO duality review meta-analysis board chair separation performance near zero effect
22. Fahlenbrach founder-CEO firms stock performance investment behavior abnormal returns 8.3% study
23. Arena Ferris Unlu co-CEOs firm performance 2011 study "co-CEO" complementary shared executive power market reaction
24. Y Combinator advice board of directors seed stage keep board small founder control Sam Altman
25. Ewens Malenko board dynamics startup life cycle VC-backed boards data independent directors control
26. De Dreu Weingart 2003 meta-analysis task conflict relationship conflict team performance negative correlation
27. Carta data startup board composition seed Series A median board seats independent directors percentage
28. deadlock resolution LLC operating agreement tie-breaker director mediation arbitration escalation clause practitioner guidance odd number managers
29. Wasserman "throne vs. the kingdom" founder control firm value Strategic Management Journal lower valuation percentage
30. Bourgeois Eisenhardt 1988 politics of strategic decision making high-velocity firms centralized power politics poor performance "consensus with qualification"
31. co-CEO structure Korea firm performance adoption study Asia Pacific Journal of Management findings negative
32. co-CEO average tenure shorter than solo CEO Equilar data years criticism co-CEO arrangements fail
33. overlapping roles founding teams conflict research role clarity new venture team "role ambiguity" performance study
34. "too many founders" five co-founders venture capital red flag equity dilution guidance investors

## 4. Model and reasoning effort

The harness for this session prohibits writing the model identifier into repository files; the identifier is disclosed in the chat conversation instead. All six contexts (main agent and five subagents) ran on the same model. The session's configured reasoning-effort setting is not exposed to the model and is therefore not reported here rather than guessed.

## 5. Tools used and URL-verification honesty

- **WebSearch**: 131 queries (all by subagents; breakdown above). This was the primary research instrument.
- **WebFetch**: attempted by all five subagents (42 attempts total: 10/7/8/10/7 per subagent). **The environment's egress proxy returned HTTP 403 policy denials for every non-GitHub host attempted** (including malegislature.gov, irs.gov, bls.gov, carta.com, yale.edu, slicingpie.com, nber.org, ssrn.com, sciencedirect.com, and others). Consequence: **exactly one cited source was actually fetched and read** (the GitHub-hosted Open Guide to Equity Compensation). **Every other cited URL was verified only via the live web-search index** — the URL was returned by search together with title/content excerpts matching the claim — not by loading the page. This is disclosed in every deliverable and per-source in `plan-7-references.md`; figures that arrived only through secondary-source snippets are marked ⚠ there.
- **Bash** (git operations; `jq` extraction of subagent transcripts; environment checks), **Read/Write** (file authoring), **Glob/Grep** (not materially used), **Agent** (spawning the 5 subagents), **TaskOutput/ToolSearch** (task management). No GitHub MCP tools were used for repository writes; all git operations were local git + push.

## 6. Commits

| Hash | Branch | Content |
|---|---|---|
| `98ad478` | `plan-7` | Root commit: the four deliverables (`plan-7-one-pager.md`, `plan-7-design.md`, `plan-7-operating-agreement.md`, `plan-7-references.md`) |
| `af10242` | `all-plans` | Adds `plans/plan-7/`: the four deliverables copied byte-identical from `plan-7` via `git show`, plus this provenance file (with this table's later hashes still as placeholders) |
| `c161f09` | `plan-7` | Mirrors the provenance file onto the plan-7 branch |
| (this commit, and its mirror on `plan-7`) | `all-plans` / `plan-7` | Records the final hashes above in this table; no other changes |

## 7. Honest limitations of this process

1. **URL verification was materially constrained** (§5): one fetched source; everything else search-index-corroborated only. Load-bearing numbers (Slicing Pie multipliers, Carta medians, Yale policy language, statutory details) should be re-verified against primary sources before reliance.
2. **Four of five subagent completion notifications were lost** to a session interruption; their results were recovered afterward from on-disk transcripts. Recovery extracted final-report text and tool-call queries only; if a subagent's last message was not its intended final report, some nuance could have been lost (the extracted texts were complete, structured reports, so this risk appears low).
3. **Some figures are secondhand** (marked ⚠ in the references): e.g., the "65% of failures from people problems," "92% of companies impose founder vesting," FAST v3 grid details, and Startup Genome/First Round team-size claims.
4. **The design contains reasoned extrapolations beyond the evidence**, stated as such in the deliverables: the annually-elected pre-financing board, the specific 2x/4x multipliers, the $400/hr expert band, and the Year-1 banding thresholds are design choices anchored to — but not dictated by — sources.
5. **Interleaved user Q&A shaped parts of the design before all research returned** (board size, election mechanics, Year-1 banding, inactive-founder treatment). Final deliverables were checked against the full research set, but the sequencing is disclosed.
6. **No legal advice**: legal risks are flagged for counsel, not resolved; several statutory/case readings rest on law-firm explainers rather than primary texts (per §5).
7. All substantive text was written by the main agent in a single pass with self-review only; no independent adversarial review pass was run over the final documents.
