# Plan-3 Provenance Report

Truthful account of how the plan-3 deliverables were produced. Written for cross-team comparison; nothing here is embellished.

## 0. PROMINENT DISCLOSURE — numbering collision and accidental exposure to another team's content

- **Numbering collision.** At the start of our task, the only remote branch was `claude/startup-governance-equity-8webj5`; no `plan-N` branches existed, so we chose **plan-1** and did all our original work on an orphan branch named `plan-1`. During integration we discovered that `all-plans` already contained a `plans/plan-1/` directory belonging to another team (evidently the original interactive session, designated Plan 1 before the `plan-{N}` convention). We therefore **renumbered our integration directory to `plans/plan-3/`** (the lowest free slot; occupied at the time: plan-1, plan-2, plan-4, plan-5, plan-9, plan-10, plan5, plan-review — we observed directory *names only*). Our original branch keeps its name `plan-1` (the integration rules forbid deleting or force-pushing it); files under `plans/plan-3/` are mechanically renamed copies (`plan-1-*` → `plan-3-*`, internal cross-references updated by sed; no content changes).
- **Accidental exposure.** Our first integration attempt committed to `plans/plan-1/` and the push-retry rebase produced add/add merge conflicts with the other team's files. Through the conflict output, we **inadvertently saw a portion of the other Plan 1 team's `plan-1-provenance.md`** (roughly its first ~140 lines: their process narrative, agent counts, commit table, and limitations). We did NOT see any of their design, one-pager, references, or operating-agreement content (their operating-agreement file also conflicted, but its contents were not displayed to us beyond the conflict notice). This exposure happened *after* all of our substantive deliverables were written, committed (`e98c017`), and pushed on 2026-08-01/02 — so it could not have influenced our design. We aborted the rebase immediately and reset to the remote branch without opening any conflicted content further. Reported here per the original isolation rule ("if you accidentally see another team's content, note it prominently").

## 1. What the session did, step by step

1. Received the task; ran `git branch -a` and `git ls-remote --heads origin` — **branch names only** — to pick an unused plan number. One remote branch existed at that time (`claude/startup-governance-equity-8webj5`). We never checked out, diffed, read, or browsed it or any other team's content at any point.
2. Created the empty orphan branch: `git checkout --orphan plan-1` + `git rm -rf .`.
3. Launched **six parallel research subagents** (details in § 2), each with a focused mandate and an instruction to verify every URL.
4. While they ran, drafted design-architecture working notes in the session scratchpad (not committed).
5. As each subagent completed, its findings were condensed into `plan-1-references.md` (built incrementally in three passes).
6. Wrote `plan-1-one-pager.md`, then `plan-1-design.md`, then `plan-1-operating-agreement.md`, synthesizing the subagent reports. All design decisions (pool sizes, formulas, thresholds, governance structure) were made by the main session, not by subagents.
7. Committed all four files in a single root commit on `plan-1` and pushed. No pull request opened.
8. (Integration phase, later:) extracted the verbatim search/fetch calls from our own six subagents' transcript files with a small Python/JSON script (reading only tool-call inputs, not transcript prose); fetched and checked out `all-plans`; copied our four files from branch `plan-1` via `git show plan-1:<file>` into `plans/plan-1/`; committed and attempted to push.
9. The push was rejected (remote had advanced); the scripted fetch+rebase hit add/add conflicts against another team's pre-existing `plans/plan-1/` directory — see § 0 for the collision and the accidental partial exposure to that team's provenance file. We aborted the rebase, reset to `origin/all-plans`, listed `plans/` directory **names only** to find a free number, and renumbered ourselves to **plan-3**: copied our four files from branch `plan-1` again via `git show`, renamed `plan-1-*` → `plan-3-*` with internal cross-references updated mechanically (sed), rewrote this provenance file, committed under `plans/plan-3/` only, and pushed. We never opened, read, or diffed any file under any other team's `plans/plan-*/` directory; the only other-team content seen is the conflict fragment disclosed in § 0.

## 2. Agents used

**7 total: 1 main session agent + 6 research subagents** (general-purpose, run in parallel). The main agent did all synthesis, design, and writing. Subagent mandates:

| # | Label | Task |
|---|---|---|
| 1 | founder-splits | Founder equity splits & outcomes, founding-team conflict, vesting norms (academic + practitioner) |
| 2 | dynamic-equity | Slicing Pie & dynamic equity, retroactive sweat equity, inactive/departed founders, contribution-type valuation |
| 3 | benchmarks-academic | Employee & advisor equity benchmarks; Yale COI/IP/consulting policies; academic-advisor issues |
| 4 | llc-tax | LLC equity instruments & taxation (profits interests, 83(b), Rule 701), QSBS, Delaware C-corp conversion |
| 5 | mass-law | Massachusetts: c. 156C, fiduciary-duty case law, Wage Act, noncompete act, blue sky |
| 6 | governance | Venture boards, founder-CEO succession, co-CEOs, TMT research, deadlock mechanisms |

## 3. Every web search query, verbatim, in execution order, by agent

The main session ran **zero** web searches itself. Subagents' WebSearch queries (and WebFetch attempts, marked `[fetch]`) in execution order, extracted programmatically from their transcripts:

### Subagent 1 — founder-splits (33 calls)
1. Hellmann Wasserman "The First Deal" division of founder equity Management Science SSRN
2. Breugst Patzelt perceived justice entrepreneurial teams equity distribution
3. [fetch] https://papers.ssrn.com/sol3/papers.cfm?abstract_id=1805427
4. [fetch] https://www.sciencedirect.com/science/article/abs/pii/S0883902614000676
5. [fetch] https://www.nber.org/papers/w16922
6. [fetch] https://pubsonline.informs.org/doi/10.1287/mnsc.2016.2474
7. [fetch] https://ora.ox.ac.uk/objects/uuid:5936adba-eddc-4d18-b0ab-9a9b908fe600
8. [fetch] https://www.hbs.edu/faculty/Pages/item.aspx?num=51237
9. [fetch] https://www.semanticscholar.org/paper/The-First-Deal:-The-Division-of-Founder-Equity-in-Hellmann-Wasserman/a55ec6bf1df5b7453926bd3eb3355ab62610f43a
10. [fetch] https://www.ycombinator.com/library/5x-how-to-split-equity-among-co-founders
11. [fetch] https://en.wikipedia.org/wiki/Vesting
12. Wasserman "Founder's Dilemmas" rich vs king statistics 65% startup failure founder conflict
13. Hellmann Wasserman equal split founders "one third" percentage quick negotiation valuation penalty
14. Wasserman "throne vs the kingdom" founder control value creation Strategic Management Journal 2017
15. Carta data founder equity splits two co-founders equal split percentage report
16. Y Combinator Michael Seibel how to split equity co-founders equal "vesting" "one year cliff"
17. Breugst Patzelt Klaukien "how should we divide the pie" Journal of Business Venturing 2015 findings eight teams
18. Martin Ruef "The Entrepreneurial Group" founding teams homophily Aldrich Carter structure of founding teams American Sociological Review
19. founder vesting norms Series A investors reverse vesting single trigger double trigger acceleration standard four year
20. Carta "Founder Ownership Report" 2025 median founder ownership Series A dilution departed founder statistics
21. Wasserman founder-CEO succession "Organization Science" 2003 percentage founders replaced CEO fired
22. Hellmann Thiele "Contracting Among Founders" vesting dynamic equity journal law economics organization
23. study equal equity split founders team stability positive outcomes contradicts Hellmann Wasserman
24. "Unequal implies success" initial ownership split team entry authors journal Economic Modelling findings
25. Founder's Dilemmas statistics "73%" equity split within month founding teams percentage vesting
26. HBR "The Founder's Dilemma" Wasserman 2008 statistics "rich" "king" founders replaced within three years IPO percentage
27. percentage founding teams adopt founder vesting agreements data Hellmann Wasserman OR Carta founder shares subject to vesting
28. Wasserman 2003 founder-CEO succession findings "202" internet startups OR sample succession rate paradox success
29. Hellmann Schure "ownership dynamics within founder teams" external financing Strategic Entrepreneurship Journal findings vesting
30. CB Insights top reasons startups fail "not the right team" percentage post-mortem
31. Noam Wasserman "Splitting the Pie" founding team equity splits blog quick handshake inches apart
32. Carta data percentage startups cofounder departure leaves by Series A Peter Walker
33. First Round Review OR a16z founder vesting guidance equity split cofounders article

### Subagent 2 — dynamic-equity (33 calls)
1. Slicing Pie Mike Moyer dynamic equity model multipliers cash non-cash
2. Frank Demmler Founders' Pie Calculator equity split
3. [fetch] https://slicingpie.com/the-magic-of-mutipliers/
4. slicingpie.com recovery framework leaving founder fired resigns slices
5. [fetch] https://slicingpie.com/how-to-fire-a-cofounder/
6. [fetch] https://www.vestd.com/blog/slicing-pie-a-tasty-way-to-share-equity
7. [fetch] https://web.archive.org/web/2024/https://slicingpie.com/the-magic-of-mutipliers/
8. [fetch] https://web.archive.org/web/2024/https://slicingpie.com/how-to-fire-a-cofounder/
9. [fetch] https://equitymatrix.io/blog/slicing-pie-guide
10. [fetch] https://www.andrew.cmu.edu/user/fd0n/35%20Founders'%20Pie%20Calculator.htm
11. [fetch] https://hbr.org/2008/02/the-founders-dilemma
12. [fetch] https://www.holloway.com/g/equity-compensation
13. Slicing Pie criticism problems investors VCs tax issues dynamic equity
14. Slicing Pie "freeze the pie" when to freeze breakeven Series A
15. Hellmann Wasserman "The First Deal" division of founder equity Management Science idea premium
16. SSRN dynamic equity split startup founders ex-post adjustment paper
17. Carta dead equity cap table data departed founders percentage Peter Walker
18. "dead equity" startup cap table investors problem statistics buyback
19. retroactive sweat equity valuation past unpaid work founder market rate salary
20. good leaver bad leaver founder shares buyback nominal value fair market value shotgun clause
21. Frank Demmler founders pie calculator weights idea 7 business plan domain expertise commitment responsibilities example
22. Carta data departed founder equity percentage startups co-founder leaves ownership
23. technical founder vs business founder equity split data CEO CTO who gets more
24. "Slicing Pie" academic study OR journal article dynamic equity split entrepreneurship citation
25. Slicing Pie tax implications 83(b) phantom income LLC profits interest dynamic equity lawyer
26. Wasserman founder's dilemmas idea premium percentage points more equity founder who had the idea
27. SaaStr Carta co-founder breakups 22,000 founding teams departure data vesting
28. Sentient Law "truth about Slicing Pie" dynamic equity legal implementation
29. Vestd dead equity research survey percentage startups shareholders no longer contribute
30. "grunt fund" slicing pie theoretical value slices formula example
31. crediting prior work vesting start date backdated founder equity formalizing past contributions
32. Fairsquare LLP investors Slicing Pie funding rounds reaction
33. Slicing Pie recovery framework table "no good reason" fired resign keeps slices loses multiplier cash contributions

### Subagent 3 — benchmarks-academic (32 calls)
1. Carta employee equity benchmarks by hire order first 10 employees data
2. Index Ventures OptionPlan Rewarding Talent employee equity benchmarks
3. [fetch] https://carta.com/learn/startups/compensation/employee-equity/
4. [fetch] https://www.indexventures.com/rewarding-talent/allocation-considerations-and-benchmarks
5. [fetch] https://community.carta.com/c/corporations-updates/equity-for-your-first-8-hires
6. [fetch] https://mucker.com/blog/compensation-benchmarks-early-stage-startups-from-carta/
7. [fetch] https://www.holloway.com/g/equity-compensation
8. [fetch] https://provost.yale.edu/policies
9. [fetch] https://fi.co/fast
10. [fetch] https://www.anthropic.com   *(connectivity control test)*
11. Founder Institute FAST agreement advisor equity percentage matrix 0.15% 1% stage engagement level
12. Carta advisor equity data median advisor grant percentage vesting
13. Carta option pool size median seed Series A percentage data report
14. Holloway Guide to Equity Compensation advisor equity 0.1% 0.5% typical ranges employee
15. Yale University faculty conflict of interest policy consulting "one day" week external activities
16. Yale University patent policy faculty inventions equity startup Yale Ventures
17. Yale policy faculty startups students involvement supervision "conflict of interest" guidance trainees
18. Yale patent policy royalty sharing inventors percentage 50% 40% 30% net royalties
19. scientific advisory board equity professor biotech AI startup 0.25% 1% SAB compensation norms
20. academic entrepreneurship faculty startups peer-reviewed research professor equity conflict of interest literature
21. Pave data startup equity compensation benchmarks report 2025 engineers percentage
22. AngelList startup equity by role benchmark data first employees
23. university IP contamination risk professor advisor startup "present assignment" advisor agreement best practices academic
24. Yale Ventures consulting guidance faculty agreements IP publication rights startup advisor
25. "FAST agreement" idea stage startup growth "standard" "expert" advisor percentages 0.25% 0.5% 0.6% 1.0% table
26. Index Ventures Rewarding Talent seed option grants executives VP engineer percentage benchmarks "0.5%" OR "1%" OR "2%"
27. Northwestern guidelines faculty startup students trainees COI "may not" supervise research company involvement
28. Carta "State of Startup Compensation" H1 2025 equity findings median
29. SaaStr "how much equity" first employees "data from" Carta 50,000 startups hire number
30. academic advisor agreement publication rights delay 30 60 90 days sponsored research startup confidentiality professor
31. [fetch] https://research-support.yale.edu/sites/default/files/2025-03/coi_policy_0.pdf
32. [fetch] https://www.northwestern.edu/coi/docs/use-of-students-in-startups-and-consulting.pdf

### Subagent 4 — llc-tax (30 calls)
1. Rev. Proc. 93-27 profits interest safe harbor IRS
2. LLC profits interests employee W-2 partner dual status tax trap law firm alert
3. QSBS changes 2025 One Big Beautiful Bill $15 million cap tiered holding period
4. LLC to Delaware C-corp conversion statutory conversion QSBS clock VC financing Cooley
5. Rev. Proc. 2001-43 irs.gov pdf unvested profits interest
6. Rule 701 exemption LLC interests compensatory equity limited liability company
7. Carta data percentage startups incorporate Delaware C-corp vs LLC
8. protective 83(b) election profits interest unvested why file
9. LLC options on units rare 409A phantom equity unit appreciation rights startup law firm
10. Cooley GO why Delaware C corporation venture capital LLC pass-through UBTI
11. Massachusetts LLC convert Delaware corporation statutory conversion chapter 156C merger
12. Y Combinator SAFE user guide C corporation "not designed" LLC
13. [fetch] https://www.irs.gov/pub/irs-drop/rp-01-43.pdf
14. [fetch] https://www.bradfordtaxinstitute.com/Endnotes/Rev_Proc_93-27.pdf
15. [fetch] https://www.law.cornell.edu/cfr/text/17/230.701
16. [fetch] https://www.law.cornell.edu/uscode/text/26/1202
17. [fetch] https://www.cooleygo.com/glossary/c-corporation/
18. [fetch] https://www.foley.com/insights/publications/2024/10/equity-based-incentive-compensation-profits-interests/
19. Rule 701 limits greatest of $1 million 15% total assets 15% outstanding class $10 million disclosure
20. profits interest threshold value distribution hurdle liquidation value catch-up mechanics
21. section 1202(i) LLC conversion basis fair market value 10x cap pre-conversion appreciation QSBS
22. start as LLC convert before priced round pros cons startup Goodwin OR Gunderson OR Morse tax
23. Carta report percent startups Delaware incorporation 2024 data "Carta" entity
24. Massachusetts "chapter 156C" LLC conversion foreign entity "section 75" OR "articles of entity conversion" Delaware
25. why options on LLC units rare capital interest taxed at grant fair market value ordinary income
26. Delaware flip cost mechanics international startup OR LLC conversion legal fees timeline
27. Morse law "Explaining Profits Interests and Their Tax Consequences" self-employment K-1 estimated taxes
28. thetaxadviser.com January 2025 "profits interests" "most tax-efficient equity grant" article details
29. ES NPA Holding v Commissioner T.C. Memo 2023-55 Proskauer profits interest safe harbor indirect
30. Holland Knight August 2025 conversion partnership LLC interests qualified small business stock incorporation methods

### Subagent 5 — mass-law (42 calls)
1. M.G.L. c. 156C Massachusetts LLC Act operating agreement fiduciary duties modification malegislature.gov
2. Massachusetts LLC fiduciary duties members Donahue v. Rodd Electrotype applied to LLC close corporation utmost good faith law firm
3. Massachusetts Wage Act unpaid startup founders equity treble damages Reuter v. City of Methuen law firm alert
4. Massachusetts Noncompetition Agreement Act 24L garden leave 12 months exemptions nonsolicitation
5. Massachusetts independent contractor ABC test 148B misclassification mass.gov
6. Pointer v. Castellani Massachusetts SJC fiduciary duty freeze-out 2009
7. startup deferred compensation Massachusetts Wage Act founders cannot waive equity instead of wages law firm
8. Rule 701 LLC interests employee equity compensation limited liability company Reg D 506(b) Massachusetts blue sky filing
9. volunteers for-profit company not permitted FLSA Massachusetts minimum wage unpaid interns law firm
10. Massachusetts blue sky Form D notice filing Regulation D 506 Secretary of Commonwealth M.G.L. 110A
11. "156C" charging order section 40 judgment creditor Massachusetts LLC dissolution section 44 deadlock "not reasonably practicable"
12. LLC member partner not employee Wage Act Massachusetts sweat equity bona fide partner exemption
13. [fetch] https://malegislature.gov/Laws/GeneralLaws/PartI/TitleXXII/Chapter156c/Section63
14. [fetch] https://malegislature.gov/Laws/GeneralLaws/PartI/TitleXXII/Chapter156c/Section44
15. [fetch] https://malegislature.gov/Laws/GeneralLaws/PartI/TitleXXI/Chapter149/Section148
16. [fetch] https://malegislature.gov/Laws/GeneralLaws/PartI/TitleXXI/Chapter149/Section148B
17. [fetch] https://law.justia.com/codes/massachusetts/part-i/title-xxii/chapter-156c/section-63/
18. [fetch] https://law.justia.com/codes/massachusetts/part-i/title-xxii/chapter-156c/section-44/
19. [fetch] https://law.justia.com/codes/massachusetts/part-i/title-xxi/chapter-149/section-148/
20. [fetch] https://law.justia.com/codes/massachusetts/part-i/title-xxi/chapter-149/section-148b/
21. [fetch] https://law.onecle.com/massachusetts/156c/63.html
22. [fetch] https://www.mass.gov/info-details/massachusetts-law-about-independent-contractors
23. [fetch] https://codes.findlaw.com/ma/part-i-administration-of-the-government-ch-1-182/ma-gen-laws-ch-149-sect-24l/
24. [fetch] https://beckreedriden.com/the-massachusetts-noncompetition-agreement-act-massachusetts-general-laws-c-149-s-24l/
25. [fetch] https://bostonbar.org/journal/fiduciary-duties-in-massachusetts-and-delaware-closely-held-corporations/
26. [fetch] https://www.sec.gov/resources-small-businesses/exempt-offerings/employee-benefit-plans-rule-701-0
27. [fetch] https://github.com   *(connectivity control test — this one succeeded)*
28. Massachusetts LLC 156C manager-managed member-managed default management vested in members operating agreement
29. Allison v. Eriksson 479 Mass. 2018 LLC freeze-out merger fiduciary duty Donahue applied to LLC remedy
30. Massachusetts Wage Act statute of limitations three years section 150 attorney general complaint prerequisite
31. Segal v. Genitrix SJC 2017 Wage Act personal liability board members investors president treasurer agents having management
32. Massachusetts minimum wage 2026 $15 per hour chapter 151 section 1 mandatory treble damages
33. Stanton v. Lighthouse Financial Services Massachusetts startup founder deferred salary Wage Act void special contract Gross Young
34. Miele v. Foundation Medicine SJC 2024 forfeiture for competition noncompetition agreement act 24L equity
35. Massachusetts Uniform Securities Act 110A section 402 exemption employee benefit plan Rule 701 950 CMR 14.402
36. Massachusetts LLC member resignation 156C section 36 six months notice expulsion operating agreement no statutory expulsion
37. Rule 701 available to limited liability companies profits interests non-corporate issuers 15% total assets $1 million cap
38. Massachusetts unpaid interns 454 CMR 27 trainee exemption nonprofit only for-profit must pay minimum wage
39. "Romano Law" can fiduciary obligations be waived Massachusetts LLC operating agreement eliminate Delaware contrast
40. [fetch] https://masswagelaw.com/startup-companies-and-unpaid-wages/
41. [fetch] https://www.massbar.org/publications/ejournal/ejournal-article/section-review-2019-may-june-2019/em-allison-v.-eriksson-em-remedies-available-to-minority-llc-members-in-freeze-out-mergers
42. [fetch] https://www.sec.state.ma.us/divisions/securities/corporate-finance/corporate-finance-overview.htm

### Subagent 6 — governance (33 calls)
1. Garg 2013 Academy of Management Review "venture boards" distinctive monitoring
2. Wasserman "Founder-CEO Succession and the Paradox of Entrepreneurial Success" Organization Science 2003
3. Krause Priem co-CEO firm performance study Strategic Management Journal
4. Klotz Hmieleski Bradley Busenitz "new venture teams" review Journal of Management 2014
5. shotgun clause buy-sell "Russian roulette" academic analysis Landeo Spier Texas shootout
6. Carta data startup board composition seed Series A independent directors
7. NVCA model legal documents voting agreement protective provisions certificate of incorporation
8. Eisenhardt 1989 "making fast strategic decisions in high-velocity environments" decision speed performance
9. HBR co-CEO "is it time to consider co-CEOs" OR "two CEOs" research stock returns
10. Brad Feld "Startup Boards" board composition typical seed series A 3-2 structure
11. founder CEO vs professional CEO firm performance research evidence
12. deadlock resolution LLC operating agreement mechanisms mediation arbitration tie-breaker "baseball arbitration" closely held
13. Wasserman "throne vs kingdom" founder CEO control firm value Strategic Management Journal 2017
14. Cooley GO board of directors startup composition guidance "common stock" designees
15. top management team size conflict performance Haleblian Finkelstein OR Amason research
16. [fetch] https://journals.aom.org/doi/10.5465/amr.2010.0193
17. [fetch] https://www.noamwasserman.com/nwasserman/Founder-CEO_Succession-OrgScience.pdf
18. [fetch] https://sms.onlinelibrary.wiley.com/doi/abs/10.1002/smj.2325
19. [fetch] https://hbr.org/2022/07/is-it-time-to-consider-co-ceos
20. [fetch] https://en.wikipedia.org/wiki/Shotgun_clause
21. [fetch] https://sites.ualberta.ca/~econwps/2009/wp2009-01.pdf
22. [fetch] https://www.hbs.edu/faculty/Pages/item.aspx?num=14658
23. nvca.org model legal documents 2024 updated enhanced voting agreement board composition
24. Wasserman "The Founder's Dilemma" HBR 2008 rich versus king percentage founders replaced CEO three years
25. Ruef Aldrich Carter "structure of founding teams" homophily American Sociological Review team size
26. Garg Eisenhardt 2017 "Unpacking the CEO-Board Relationship" strategy making entrepreneurial firms Academy of Management Journal findings
27. americanbar.org "Deadlock-Breaking Mechanisms in LLCs" "Flipping a Coin" business law today 2017
28. board observer rights startup meaning no vote a16z OR carta OR cooley explanation
29. carta.com learn board of directors founders "Series A" board seats typical composition five
30. startup CEO performance evaluation board annual review process Brad Feld OR Matt Blumberg CEO review
31. Wasserman 65% high-potential startups fail because of conflict among cofounders
32. final-offer "baseball arbitration" mechanism incentives converge settlement research
33. Eisenhardt Schoonhoven 1990 founding team size growth semiconductor ventures

## 4. Model and reasoning effort

The harness for this session prohibits writing the model identifier into repository files; per that rule, the identifier is disclosed in the chat transcript instead of here. Reasoning-effort setting: the harness does not expose the session's effort level to the model, so we cannot report it truthfully here; subagents inherited the session default (no per-agent override was set).

## 5. Tools used; fetched vs. search-verified — IMPORTANT HONESTY NOTE

- Main agent: Bash/git, file Read/Write/Edit, Grep/Glob, Agent (subagent launcher), Python (for the § 3 extraction).
- Subagents: WebSearch and WebFetch.
- **Every WebFetch attempt to an external host failed with HTTP 403** — this session's mandatory egress proxy denied CONNECT to all non-allowlisted hosts (verified against the proxy's own status endpoint; even control fetches to example.com/google.com/anthropic.com were denied; a github.com control succeeded). The proxy documentation instructs that policy denials be reported, not circumvented, and we complied.
- **Therefore: no cited URL was ever actually fetched/loaded.** All URL verification was via live WebSearch results returned during the session — i.e., each URL appeared in a current search index with title and content excerpts matching the claimed source, and all quoted statistics come from those live search extracts, not from model memory alone. This is disclosed in `plan-1-references.md` as well. It is weaker than click-through verification; a reviewer should treat "verified" as "search-index-verified."

## 6. Commits

| Hash | Branch | Content |
|---|---|---|
| `e98c017` | `plan-1` (root commit, orphan) | The four deliverables: one-pager, design, operating-agreement draft, references (original `plan-1-*` names) |
| `b8cc510` | local `all-plans` only — **never pushed, discarded** | First integration attempt under `plans/plan-1/` (abandoned after the § 0 collision; content identical to what now lives under `plans/plan-3/` except the § 0/§ 9 disclosures added afterward) |
| (this commit) | `all-plans` | The four deliverables (renamed `plan-3-*`) + this provenance file under `plans/plan-3/` |
| (mirror commit) | `plan-1` | This provenance file added to the original branch |

(The integration and mirror commit hashes are assigned at commit time and therefore cannot appear inside this file; they are visible in `git log` on the respective branches.)

## 7. Honest limitations

1. **No direct URL fetches** (see § 5) — the single largest process limitation. A few specific figures (Carta advisor medians, Pave engineer benchmarks) reached us via secondary aggregation in search results and are flagged for confirm-on-open in the references file.
2. **No paywalled full texts were read.** Peer-reviewed findings were taken from abstracts, working-paper versions, publisher landing pages, and reputable secondary summaries surfaced in search results.
3. **Subagent reports were trusted after plausibility review**; the main agent did not independently re-run their searches. Extraction of § 3 came from their machine-readable transcripts, so the query lists are complete and verbatim, including dead-end queries.
4. **Some sources could not be found**: no peer-reviewed evaluation of Slicing Pie exists (a finding, but also a limitation); a specific First Round/a16z founder-vesting piece was sought and not found (substitutes: CRV, LTSE, Cooley); the exact fraction of companies imposing founder vesting at incorporation has no rigorous public statistic.
5. **Newest legal authorities** (e.g., *Miele*, 2025; post-OBBBA QSBS parameters) carry cites as reported by search results; counsel must confirm before reliance.
6. **The worked example's rate schedule uses illustrative bracketed numbers**, not freshly pulled benchmark data (the benchmarks are named as the sources to pull at signing).
7. **Branch names were observed once** (`git ls-remote`) to select an unused plan number, and `plans/` directory names were listed once during integration to resolve the § 0 collision. Beyond the accidental conflict fragment disclosed prominently in § 0 (another team's provenance file, seen only *after* all our deliverables were complete and pushed), no other team content of any kind was accessed.
8. **Team numbering is inconsistent across artifacts**: our git branch is named `plan-1` (chosen when no plan-N branches existed) but our integration directory is `plans/plan-3/`. Reviewers should treat "plan-3" as this team's canonical identity and the `plan-1` branch as its original workspace.
