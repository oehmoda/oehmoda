# plan5 — Provenance Report

Truthful record of how team plan5's deliverables were produced. Written for
cross-team comparison; nothing here is embellished.

---

## 0. Two integrity disclosures, up front

**(a) A rival "plan-5" existed before we ever pushed.** When we first pushed our
finished work, a `plan-5` branch already existed on the remote that we did not create.
Per the isolation rules we never read, fetched, diffed, or checked out its content; we
observed only ref *names* (`git ls-remote`). Rather than force-push over unknown work, we
pushed our orphan history to this session's explicitly designated branch,
`claude/plan5-llc-governance-equity-j5kmc7`, and documented the situation in
`plan-5-NOTE.md`.

**(b) The integration branch's `plans/plan-5/` directory was already occupied.** On
checking out `all-plans`, `plans/plan-5/` already contained six files we did not write —
including a `plan-5-provenance.md` purporting to be this team's provenance, and a
`plan-5-conclusions.md` that was never among our deliverables. We did not open any of
them (file *names* only were observed via `git ls-tree` / `git status`). To comply with
the instruction that our work live at `plans/plan-5/` without destroying or
misrepresenting anyone's work, we moved those six files, unread and byte-for-byte intact,
into `plans/plan-5/_preexisting-unverified/`, and placed our genuine deliverables at the
canonical path. **Team plan5 did not author anything inside `_preexisting-unverified/`,
and the provenance file in there is not ours.** Our authentic deliverables are exactly:
`plan-5-one-pager.md`, `plan-5-design.md`, `plan-5-operating-agreement.md`,
`plan-5-references.md`, `plan-5-NOTE.md`, and this file.

## 1. What the session did, step by step

1. Created an empty orphan branch immediately (`git checkout --orphan plan-5`;
   `git rm -rf .`) before reading anything; never viewed any other branch's content at
   any point in the session.
2. Launched **six research subagents in parallel** (one message, six Agent calls), each
   with instructions to verify every cited URL and label verification status honestly.
3. While subagents ran, drafted `plan-5-operating-agreement.md` (mechanism design needing
   few citations) and committed it (`ec2c9c9`).
4. As each subagent completed, archived its key findings to session scratchpad files.
5. After all six returned, wrote `plan-5-design.md` (framework + rationale + worked
   numeric example), `plan-5-references.md` (annotated bibliography with per-source
   evidence ratings and verification statuses), and `plan-5-one-pager.md`; committed
   (`f1deec9`).
6. First push to `plan-5` was rejected (pre-existing remote branch, disclosure 0a);
   inspected remote ref names only; wrote `plan-5-NOTE.md`; committed (`88aab42`);
   pushed the branch to `claude/plan5-llc-governance-equity-j5kmc7`.
7. Answered several founder Q&A turns in chat (no repo changes).
8. Integration task: extracted the verbatim WebSearch queries from the six subagent
   transcripts (targeted `jq` extraction of query strings only); fetched and checked out
   `all-plans`; found disclosure 0b; quarantined the pre-existing files unread; copied
   own files from the local `plan-5` branch via `git show plan-5:<file>`; wrote this
   provenance file; committed and pushed; mirrored this file onto the team branch.

## 2. Agents used

**1 main agent + 6 research subagents** (no other agents; no nested subagents; the
Workflow orchestration tool was not used).

| Subagent | Task | # web searches |
|---|---|---|
| A — Founder-equity academia | Peer-reviewed literature on founder equity splits, consequences, fairness/pay-dispersion evidence | 27 |
| B — Governance/leadership academia | Shared leadership meta-analyses, self-managing orgs, co-CEOs, fast decisions, venture boards, deadlock, founder control | 26 |
| C — Dynamic-equity frameworks | Slicing Pie mechanics + criticisms, alternative calculators, salary/consulting benchmarks, vesting/pool norms, dead equity | 28 |
| D — Investor/tax structuring | DE C-corp preference, QSBS/OBBBA 2025, LLC→C-corp conversion, profits interests, 83(b), Rule 701, SAFEs, diligence | 25 |
| E — Massachusetts law + Yale policies | Wage Act, ABC test, c.156C, noncompete act, blue sky, Yale handbook/COI/patent policy, NIH FCOI | 22 |
| F — Advisor norms | FAST agreement, Carta advisor data, SAB norms, star-scientist and signaling literature, consulting-for-equity | 22 |

The main agent ran **no web searches** itself. Total: **150 queries**.

## 3. Every web search query, verbatim, in execution order

The six subagents ran concurrently (launched simultaneously); within each subagent,
queries are listed in that agent's execution order.

### Subagent A — Founder-equity academia (27)
1. Hellmann Wasserman "The First Deal" division of founder equity Management Science 2017
2. Breugst Patzelt Preller equity distribution justice entrepreneurial teams Journal of Business Venturing
3. Hellmann Wasserman first deal founder equity "equal split" percentage "within a day" negotiation valuation discount findings
4. Wasserman Founder's Dilemmas 65% startup failures cofounder conflict statistic source
5. Breugst Patzelt Rathgeber 2015 "How should we divide the pie" equity distribution entrepreneurial teams abstract findings justice
6. Kotha George 2012 Journal of Business Venturing "Friends, family, or fools" entrepreneur experience equity distribution resource mobilization abstract
7. Wasserman "The Founder's Dilemma" HBR 2008 rich versus king statistics founder CEO replaced "three years" percentage
8. dynamic equity split startup academic research renegotiation founder equity agreement empirical study
9. Ewens Marx founder replacement startup performance Review of Financial Studies 2018 findings
10. Wasserman founder-CEO succession Organization Science 2003 paradox of entrepreneurial success findings percentage founders fired
11. Hochberg Lindsey 2010 broad-based employee stock options firm performance Journal of Financial Economics findings
12. Breza Kaur Shamdasani "morale effects of pay inequality" QJE 2018 findings output attendance percent
13. Hellmann Thiele "Contracting among founders" vesting founder agreements journal
14. Shaw pay dispersion review Annual Review Organizational Psychology 2014 findings when dispersion helps hurts
15. Kim Ouimet 2014 Journal of Finance broad-based employee stock ownership plans wages firm value findings
16. Bloom 1999 Academy of Management Journal pay dispersion baseball performance findings compressed pay
17. "Squaring the founders' circle" equity split paper
18. Carta data cofounder equity splits percent equal split report
19. Hellmann Wasserman what fraction of founding teams split equity equally "a third" OR "one-third" OR "32%" OR "33%" 511 ventures
20. Wasserman "73%" teams split equity "within a month" founding negotiation day handshake
21. "Slicing Pie" Moyer dynamic equity split academic peer-reviewed evaluation grunt fund
22. Adams 1965 "Inequity in social exchange" Advances in Experimental Social Psychology equity theory citation
23. cofounder departure rate percentage startups research "leave" within years founding team turnover study vesting
24. equity split founders recent study Management Science OR "Strategic Management Journal" 2020..2025 equal split performance gender
25. "Unequal implies success" initial ownership split team entry new venture performance Economic Modelling authors citation
26. Hellmann Wasserman equal splitters "day or less" negotiating founder equity quick negotiation share
27. de Wit Greer Jehn 2012 meta-analysis intragroup conflict relationship conflict team performance findings

### Subagent B — Governance/leadership academia (26)
1. Nicolaides et al. 2014 shared leadership team performance meta-analysis Leadership Quarterly effect size
2. D'Innocenzo Mathieu Kukenberger 2016 meta-analysis shared leadership team performance Journal of Management
3. Wang Waldman Zhang 2014 "meta-analysis of shared leadership and team effectiveness" Journal of Applied Psychology rho .34 moderators new-genre task complexity
4. Nicolaides 2014 "shared leadership of teams" meta-analysis corrected correlation team performance value task interdependence team tenure
5. D'Innocenzo 2016 shared leadership meta-analysis rho .21 team performance moderators task complexity team size
6. "Nicolaides" 2014 meta-analysis shared leadership "team performance" "ρ" OR "rho" ".26" OR ".27" OR ".28" overall effect 3000 individuals
7. Lee Edmondson 2017 "Self-managing organizations" Research in Organizational Behavior less hierarchical review findings limits
8. Zappos holacracy outcomes turnover buyout 18% abandoned self-management journalism
9. Eisenhardt 1989 "Making fast strategic decisions in high-velocity environments" findings more information more alternatives counselors "consensus with qualification"
10. Harvard Business Review 2022 co-CEOs study 87 companies shareholder returns 9.5% Feigen Jenkins
11. Krause Priem Love co-CEO 2015 Strategic Management Journal power gap firm performance empirical
12. Garg 2013 Academy of Management Review "Venture boards" distinctive monitoring startup board CEO duality
13. Wasserman 2003 "Founder-CEO succession" Organization Science paradox of entrepreneurial success findings
14. Wasserman 2017 "throne" "kingdom" Strategic Management Journal founder control firm valuation lower value percentage
15. Aghion Tirole 1997 "Formal and Real Authority in Organizations" Journal of Political Economy delegation overload initiative
16. Jin et al 2017 meta-analysis "new venture teams" team size composition performance Entrepreneurship Theory and Practice
17. Edmondson 1999 psychological safety team learning Administrative Science Quarterly 51 teams findings
18. Garg 2013 "Venture Boards: Distinctive Monitoring" abstract venture board smaller CEO influence institutional investors firm performance
19. "Beyond the Holacracy Hype" Bernstein Bunch Canner Lee Harvard Business Review 2016 findings
20. deadlock closely held corporations 50/50 owners dispute resolution empirical law review
21. "Venture Boards: Past Insights, Future Directions" Garg Furr 2017 Strategic Entrepreneurship Journal abstract
22. early stage startup board size norms seed Series A three five directors Brad Feld startup boards guidance
23. Greenberg Mollick "Sole Survivors" solo founders versus founding teams survival revenue findings
24. "Nicolaides" shared leadership meta-analysis abstract "team confidence" "team performance" number of independent samples teams 3861 OR "42" OR "5,000"
25. D'Innocenzo Mathieu Kukenberger shared leadership team performance overall corrected correlation "0.21" OR "= .21" OR ".19"
26. "Irreconcilable Differences" "Judicial Resolution of Business Deadlock" University of Chicago Law Review Hwang deadlock dissolution

### Subagent C — Dynamic-equity frameworks (28)
1. Slicing Pie Mike Moyer multipliers 4x cash 2x non-cash slices formula
2. "slicing pie" criticism lawyer tax problems dynamic equity split investors
3. slicingpie.com recovery framework fired for cause resignation "well" bake the pie Series A breakeven
4. Slicing Pie "well" definition slices "bake" pie terminates breakeven Series A funding grunt fund
5. Frank Demmler "Founders' Pie Calculator" methodology weights idea business plan domain expertise commitment risk
6. foundrs.com co-founder equity split calculator questionnaire methodology
7. levels.fyi 2025 senior software engineer median total compensation United States report
8. Carta data percentage companies 4-year vesting one-year cliff standard founder vesting
9. Index Ventures OptionPlan option pool size seed 10% employee grants first 10 hires percentage
10. Michael Seibel Y Combinator how to split equity among co-founders equally YC library
11. "dead equity" startup Fred Wilson AVC founder departed cap table problem essay
12. Joel Spolsky fair equity split layers method "stripe" answer onstartups 50-50
13. Buffer transparent salary formula equity formula open equity percentages employees
14. Walker Corporate Law "dynamic equity" OR "slicing pie" founders equity split lawyer problems
15. Holloway Guide to Equity Compensation holloway.com contents 409A vesting acceleration double trigger
16. machine learning PhD consulting day rate academic consultant typical $1000 2000 per day
17. Carta Peter Walker data median equity grant first employee 1% hires 1-5 employees percentage seed startup
18. Carta "founding engineer" median equity grant "1.54" percent
19. Gust cofounders.gust.com equity split questionnaire how it works methodology dynamic
20. "Pie Slicer" software slicing pie app track contributions slices pricing
21. fairsquarellp "investors and slicing pie" what investors think convert fixed split funding
22. Sentient Law "truth about slicing pie" implementation perils tax phantom income LLC corporation
23. Cooley GO founder stock vesting back-vesting credit prior service acceleration double trigger recommendation
24. levels.fyi "end of year pay report" 2025 median compensation senior engineer L5 E5 numbers
25. equitymatrix "slicing pie problems" no cliff hourly rate disputes time inflation investor confusion list
26. TechCrunch "solve the dead equity problem" longer founder vesting 2020 details percentages founders leave
27. Slicing Pie recovery framework table "fired without cause" keeps slices "resign with good reason" treated like fired buyout multiplier removed
28. Forbes "Overcoming the Misconceptions of Dynamic Equity" 2017 author legal council

### Subagent D — Investor/tax structuring (25)
1. Cooley GO why Delaware C corporation venture capital investors LLC
2. OBBBA QSBS section 1202 changes $15 million cap $75 million gross assets tiered holding period law firm alert
3. Y Combinator "should you incorporate" LLC or C corporation startup library
4. Frost Brown Todd QSBS incorporating partnership LLC conversion section 1202 10x basis appreciated assets
5. Massachusetts LLC statutory conversion Delaware corporation chapter 156C 2016 amendment entity conversion permitted
6. Rev. Proc. 93-27 Rev. Proc. 2001-43 profits interest not taxable grant liquidation threshold law firm explainer
7. "156C" Massachusetts LLC cannot convert corporation merger "conversion" statute LLC to corporation Massachusetts 156D entity conversion
8. Carta data percent startups incorporated Delaware C corporation venture backed
9. convert Massachusetts LLC to Delaware corporation merger method no statutory conversion law firm
10. 83(b) election 30 days IRS instructions consequences failure to file Cooley Carta
11. NVCA model legal documents Delaware corporation assumption venture financing enhanced model documents
12. Rule 701 exemption employee equity compensation $10 million disclosure threshold SEC compensatory
13. YC SAFE designed for Delaware corporation LLC adapted SAFE friction convert C-corp before SAFE
14. "dead equity" cap table how much is too much investors former founders percentage
15. profits interest recipient becomes partner cannot be W-2 employee self-employment tax K-1 Rev. Rul. 69-184 law firm
16. phantom equity unit appreciation rights LLC alternative to profits interests avoids partner status law firm
17. Cooley GO founder vesting "investors will" require vesting Series A unvested founder stock
18. Fenwick OR Orrick OR Cooley alert "One Big Beautiful Bill" section 1202 QSBS "July 4, 2025" tiered exclusion 50% 75% 100%
19. ycombinator.com library incorporate Delaware corporation "we require" OR "standard" YC companies Delaware
20. LLC to C-corp conversion tax-free section 351 "Rev. Rul. 84-111" three methods assets-over timing before financing round
21. Rule 701 state blue sky laws not preempted "not covered securities" state exemption 25102(o)
22. Perkins Coie OBBBA 1202 included portion 28% rate AMT preference three-year 50% exclusion inflation adjustment 2027
23. Cooley GO OR YC due diligence checklist IP assignment agreements every employee founder invention assignment importance financing
24. SAFE for LLC "membership interest" adapted SAFE exists convertible instrument LLC startup lawyer
25. section 1202(d) aggregate gross assets contributed property fair market value at contribution basis equals FMV incorporation partnership 10x exclusion cap Frost Brown Todd

### Subagent E — Massachusetts law + Yale policies (22)
1. Reuter v. City of Methuen 2022 SJC treble damages Wage Act mandatory late wages
2. Cook v. Patient EDU LLC 465 Mass. 548 LLC manager personal liability Wage Act
3. "section 148" chapter 149 Massachusetts "president and treasurer" "officers or agents having the management" deemed employers text
4. M.G.L. c. 149 section 150 treble damages "lost wages and other benefits" attorney's fees text
5. M.G.L. c.149 148B ABC test text "free from control" "outside the usual course of the business" "independently established trade"
6. DOL FLSA volunteers for-profit private sector employers "may not volunteer" elaws or fact sheet
7. Massachusetts independent contractor statute 148B three prong "independently established trade, occupation, profession or business" mass.gov advisory 2008/1
8. startup paying employees equity instead of cash wages violates minimum wage FLSA law firm alert founders sweat equity
9. Massachusetts minimum wage $15.00 per hour January 2023 G.L. c.151 section 1 mass.gov
10. Massachusetts LLC Act chapter 156C fiduciary duties operating agreement modify eliminate Delaware 18-1101(c) contrast case law
11. converting Massachusetts LLC to Delaware corporation merger conversion chapter 156C law firm redomestication mechanics
12. Massachusetts Noncompetition Agreement Act G.L. c.149 24L garden leave 12 months terminated without cause requirements
13. Donahue v. Rodd Electrotype 367 Mass. 578 close corporation fiduciary duty "utmost good faith and loyalty" applied to LLC Massachusetts
14. Rule 701 compensatory benefit plan exemption Massachusetts blue sky exemption stock options 950 CMR employee equity
15. Yale faculty handbook consulting "one day" per seven-day week outside employment limit
16. Yale University conflict of interest policy faculty equity outside entity disclosure students involvement research
17. Yale Patent Policy university ownership inventions "significant use" of university facilities royalties ocr.yale.edu
18. Yale faculty founder startup guidance equity officer role Yale Ventures policy "faculty member" company leadership restrictions
19. NIH financial conflict of interest regulation 42 CFR 50.603 significant financial interest $5,000 equity non-publicly traded any equity investigator disclosure
20. Cooley Orrick founder technology assignment agreement confirmatory IP assignment prior employer claims diligence startup
21. Massachusetts LLC cannot statutory conversion foreign corporation merger only c.156C section 59 60 Delaware DGCL 265 conversion Massachusetts entity
22. granting founder equity for past services tax consequences compensation income ordinary income fair market value 83(b) restricted stock past work startup

### Subagent F — Advisor norms (22)
1. FAST agreement Founder Institute advisor equity template percentages grid
2. Carta data advisor equity grants median percentage vesting
3. Carta Peter Walker advisor equity data median percent pre-seed seed "advisor" grants blog
4. scientific advisory board equity percentage biotech startup 0.1% 0.5% SAB member norms
5. Zucker Darby Brewer 1998 American Economic Review "Intellectual Human Capital and the Birth of U.S. Biotechnology Enterprises" star scientists
6. Hsu 2004 Journal of Finance "What do entrepreneurs pay for venture capital affiliation" certification effect findings offer acceptance discount
7. Plummer Allison Connelly 2016 "better together" signals legitimacy early stage ventures Academy of Management Journal
8. Y Combinator part-time founders "won't fund" commitment Paul Graham investors discount part-time
9. "advisor equity" regret "too expensive" founder essay cap table advisors never showed up Fred Wilson OR Calacanis OR "advisory shares"
10. Jason Calacanis "should you give advisors equity" advice 0.1% 0.25% shares LinkedIn essay
11. Toole Czarnitzki academic entrepreneurs NIH SBIR "brain drain" firm performance star scientists Management Science
12. Stuart Hoang Hybels 1999 "interorganizational endorsements" performance entrepreneurial ventures IPO biotech prominent affiliates findings
13. Higgins Stephan Thursby star scientists signals biotech IPO "Research Policy" conveying quality
14. part-time founders investors won't fund "part-time" founder commitment signal venture capital essay Michael Seibel OR "Dalton Caldwell" OR angel
15. compensating consultants with equity startup law firm 1099 income tax FMV vesting "consulting for equity" Cooley GO explainer
16. FAST v3 Founder Institute 2026 advisor equity grid "Standard" "Expert" pre-seed 0.5% percentages by stage
17. Bruce Booth LifeSciVC scientific advisory boards "what works" equity compensation academic founders biotech percentage
18. Paul Graham "18 Mistakes That Kill Startups" "half-hearted effort" part-time consulting job startups
19. Ding Stuart academic scientists SAB participation OR Murray 2004 "academic inventors in entrepreneurial firms" Research Policy laboratory life
20. advisor equity "single trigger" acceleration acquisition standard advisor agreement norm 100% vesting change of control
21. study celebrity endorsement crowdfunding OR fundraising startup evidence does having famous advisor help raise capital research
22. Carta advisor grants vesting "2 years" cliff "no cliff" percent of advisor grants single-trigger data cartadata

## 4. Model and reasoning effort

This session's harness **prohibits writing the model identifier into repository files**;
per the provenance instructions, the identifier is disclosed in the accompanying chat
message instead. The harness does not expose its configured reasoning-effort setting to
the agent; subagents inherited the session's default settings. We will not guess values
we cannot observe.

## 5. Tools used, and fetch-vs-search honesty

- **WebSearch** (subagents only): the 150 queries above. Search results returned live
  page content (titles, URLs, abstract/statistic excerpts) on which verification rests.
- **WebFetch / curl:** attempted by all six subagents and **blocked by the sandbox's
  egress policy** (HTTP 403 CONNECT denial) for every non-GitHub host, confirmed against
  control URLs. **Exactly two cited sources were directly fetched** (both GitHub-hosted):
  the Spolsky equity-split gist and the Open Guide to Equity Compensation repo. **Every
  other cited URL was verified only via live search-retrieved content, not by direct
  fetch** — each entry in `plan-5-references.md` is labeled accordingly.
- **Agent tool** (6 subagents), **Bash/git**, **Read/Write/Edit**, and `jq` (to extract
  the query lists above from the session's own subagent transcripts — query strings only).
- No GitHub MCP tools, no Workflow tool, no artifacts, no PRs.

## 6. Commits

| Hash | Branch | Content |
|---|---|---|
| `ec2c9c9` | team branch (pushed as `claude/plan5-llc-governance-equity-j5kmc7`) | `plan-5-operating-agreement.md` v1 (pre-research-integration draft) |
| `f1deec9` | team branch (same) | `plan-5-design.md`, `plan-5-one-pager.md`, `plan-5-references.md` |
| `88aab42` | team branch (same) | `plan-5-NOTE.md` (branch-collision & isolation disclosure) |
| *(this commit)* | `all-plans` | `plans/plan-5/`: our six files at canonical path; six pre-existing files quarantined unread into `_preexisting-unverified/` |
| *(mirror commit)* | team branch (same) | this provenance file mirrored |

## 7. Honest limitations

1. **No direct fetch of 68 of ~70 cited URLs** (egress policy). Search-retrieved page
   content is strong but weaker than reading full texts; specific statistics flagged
   "partially verified" in the references were not confirmed and are treated as such.
2. **Subagent-reported findings were not independently re-verified** by the main agent
   against full texts; cross-checks were limited to internal consistency across agents
   and across multiple independent search results.
3. **The centerpiece mechanism (dynamic contribution ledger) has no peer-reviewed
   validation anywhere** — disclosed in the design itself (§5.2, §10), chosen because the
   founders' fixed requirements demand contribution metering.
4. **Single-session work.** No founder interviews, no company documents, no cap-table
   data for this specific company; the worked example uses invented illustrative hours.
5. **Legal content is business-level triage, not legal advice**; several statutory
   details (MA outbound-conversion mechanics, the MA blue-sky subsection, FAST v3 grid)
   are explicitly flagged as needing counsel/primary-text confirmation.
6. **Bracketed parameters** (120 h/month threshold, 50% evidence discount, audit rate,
   etc.) are design choices, not research findings, and are labeled as such.
7. **Collision handling** (disclosures 0a/0b) required judgment calls made without
   reading the conflicting content; if the pre-existing `plan-5` material turns out to be
   legitimately another team's, the reviewer should attribute `_preexisting-unverified/`
   to them, not to us.

*— plan5*
