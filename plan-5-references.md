# Plan 5 — Annotated Bibliography & Evidence Ratings

**How these sources were verified (integrity note).** This work was performed in a
sandboxed environment whose network egress policy blocked *direct* page fetches to all
non-GitHub hosts (proxy CONNECT denials, confirmed against control URLs). Verification
was therefore performed through live web-search retrieval, in which the search backend
returns actual page content (titles, URLs, abstract text, statistics). Statuses used:

- **Verified (search-retrieved content)** — the URL resolved in the live search index this
  session *and* the specific claims/numbers we cite appeared in content retrieved from the
  page, usually corroborated across ≥2 independent results.
- **Verified (direct fetch)** — full content retrieved (possible only for GitHub-hosted
  sources).
- **Partially verified** — source and general finding confirmed; a specific detail we note
  could not be confirmed and is flagged inline.

No source below is cited from memory alone; items we *could not* adequately verify were
either dropped or explicitly flagged (see "claims we deliberately did not rely on" at the
end). We did not read, checkout, or view any other team's branch or files at any point.

Evidence-strength scale: **A** peer-reviewed causal (RCT/IV/experiment) · **B**
peer-reviewed meta-analysis or review · **C** peer-reviewed correlational/qualitative ·
**D** statute, regulation, case law, or official policy (primary) · **E** large-N data
provider (not peer-reviewed) · **F** practitioner framework/commentary · **G** journalism
/ anecdote.

---

## I. Founder equity splits (academic)

**[R-1] Hellmann, T., & Wasserman, N. (2017). "The First Deal: The Division of Founder
Equity in New Ventures." *Management Science* 63(8): 2647–2666.**
https://pubsonline.informs.org/doi/10.1287/mnsc.2016.2474 · SSRN:
https://papers.ssrn.com/sol3/papers.cfm?abstract_id=1805427 · NBER:
https://www.nber.org/papers/w16922 · Digest:
https://www.nber.org/digest/aug11/division-founder-equity-new-ventures
Verified (search-retrieved content). 1,476 founders / 511 ventures: ~⅓ split equally;
heterogeneity in idea, prior founding experience, and capital reduces equal-split
likelihood; equal splits associated with lower first-round pre-money valuations,
concentrated in negotiations of "a day or less"; magnitude ≈10% of equity / ≈$450K NPV.
Supports: don't fossilize a quick equal split; contribution heterogeneity should price
into shares. **Rating: C — authors explicitly frame the valuation result as association
(selection on unobservables), not causation.**

**[R-2] Wasserman, N. (2008). "The Founder's Dilemma." *Harvard Business Review* 86(2).**
https://hbr.org/2008/02/the-founders-dilemma
Verified (search-retrieved content). 212 startups: by year 3, 50% of founders no longer
CEO; by year 4 only 40% remain; <25% led their IPO; rich-vs-king tradeoff. Supports:
CEO-for-life design is counter-evidential. **Rating: F summarizing C.**

**[R-3] Wasserman, N. (2012). *The Founder's Dilemmas*. Princeton University Press.**
https://press.princeton.edu/books/paperback/9780691158303/the-founders-dilemmas
Verified (search-retrieved content). ~10,000-founder dataset. 65% of VC portfolio-company
failures attributed to "people problems" (attribution survey — often misquoted as
"cofounder conflict causes 65% of failures"); 73% of teams split equity within one month
of founding, mostly without adjustment mechanisms. Supports: early, static splits are the
modal error. **Rating: F built on C data; the 65% is attribution, not measurement.**

**[R-4] Breugst, N., Patzelt, H., & Rathgeber, P. (2015). "How should we divide the pie?
Equity distribution and its impact on entrepreneurial teams." *Journal of Business
Venturing* 30(1): 66–94.**
https://www.sciencedirect.com/science/article/abs/pii/S0883902614000676
Verified (search-retrieved content). Eight teams over six months: *perceived justice* of
the split — not its arithmetic — drives positive vs. negative team-interaction spirals.
Supports: transparent, justified process as the core intervention. (Note: third author is
Rathgeber; "Breugst, Patzelt & Preller" citations of this paper are miscitations.)
**Rating: C (qualitative, theory-building, n=8).**

**[R-5] Kotha, R., & George, G. (2012). "Friends, family, or fools: Entrepreneur
experience and its implications for equity distribution and resource mobilization."
*Journal of Business Venturing* 27(5): 525–543.**
https://www.sciencedirect.com/science/article/abs/pii/S0883902612000365
Verified (search-retrieved content). 611 entrepreneurs: experienced founders allocate
equity selectively against contribution and mobilize more resources. Supports: equity as
a priced resource. **Rating: C.**

**[R-6] Hellmann, T., & Thiele, V. (2015). "Contracting Among Founders." *Journal of Law,
Economics, and Organization* 31(3): 629–661.**
https://academic.oup.com/jleo/article-abstract/31/3/629/808939
Verified (search-retrieved content). Formal theory: contingent contracts with share
vesting mitigate hold-up and premature-commitment inefficiencies in team formation.
Supports: the closest academic anchor for vesting/contingent (dynamic-ish) equity.
**Rating: C (pure theory).**

**[R-7] Ewens, M., & Marx, M. (2018). "Founder Replacement and Startup Performance."
*Review of Financial Studies* 31(4): 1532–1565.**
https://academic.oup.com/rfs/article-abstract/31/4/1532/4604800
Verified (search-retrieved content). IV design (state noncompete-law changes): replacing
founders *improves* startup outcomes; naive OLS shows the opposite (selection). Supports:
removable-executive governance; plan for founder departure. **Rating: A (IV).**

**[R-8] Carta founder data (Peter Walker / Carta Insights).**
https://carta.com/data/how-co-founders-split-equity/ ·
https://carta.com/data/founder-equity-split-trends-2024/ ·
https://carta.com/data/founder-ownership/ · departure summary:
https://www.saastr.com/carta-co-founder-break-ups-are-accelerating
Verified (search-retrieved content). >45,000 startups (2015–2024): ~24% of founding teams
split equally; 2-person equal splits rose 31.5%→45.9% (2015→2024). Cofounder departures:
>23% gone by year 3; ~40% before IPO. Supports: base rates motivating earn-only
allocations and departure planning. **Rating: E (platform selection bias).**

**[R-9] "Unequal implies success? How initial ownership split impacts team entry and new
venture performance." *Economic Modelling* (2022).**
https://www.sciencedirect.com/science/article/abs/pii/S0263237322001785
Partially verified — findings and n (24,194 German startups; unequal splits ≈1.3 p.p.
higher 3-year growth; mediated by openness to team entry) search-confirmed; exact
author list not confirmed this session. Supports: non-US replication of the equal-split
association. **Rating: C.**

**[R-10] "The gender gap in the first deal." *Journal of Banking & Finance* 168 (2024),
art. 107277.** https://www.sciencedirect.com/science/article/pii/S0378426624001869
Verified (search-retrieved content). Female founder-CEOs own ~12 p.p. less than male
counterparts; pattern tracks social norms. Supports: splits absorb social bias unless
mechanized — an argument for formula over negotiation. **Rating: C.**

**[R-11] Hochberg, Y., & Lindsey, L. (2010). "Incentives, Targeting, and Firm
Performance." *Review of Financial Studies* 23(11): 4148–4186.**
https://academic.oup.com/rfs/article-abstract/23/11/4148/1609512 — Verified
(search-retrieved content). IV: broad-based non-executive option incentives → higher
operating performance, concentrated in small, high-growth firms. Supports: broad employee
equity in a 15-person company. **Rating: A (IV).** See also **Kim, E.H., & Ouimet, P.
(2014), *Journal of Finance* 69(3): 1273–1319**
(https://onlinelibrary.wiley.com/doi/abs/10.1111/jofi.12150): small (<5%) broad ESOPs
raise productivity and pay in small firms; free-riding grows with headcount. **Rating:
C/A-.**

**[R-12] Wasserman, N. (2003). "Founder-CEO Succession and the Paradox of Entrepreneurial
Success." *Organization Science* 14(2): 149–172.**
https://pubsonline.informs.org/doi/10.1287/orsc.14.2.149.14995 · PDF:
https://www.noamwasserman.com/nwasserman/Founder-CEO_Succession-OrgScience.pdf
Verified (search-retrieved content). 202 firms: founder-CEOs most likely replaced after
success milestones (product completion, financing rounds). **Rating: C.**

**[R-13] Wasserman, N. (2017). "The throne vs. the kingdom: Founder control and value
creation in startups." *Strategic Management Journal* 38(2): 255–277.**
https://sms.onlinelibrary.wiley.com/doi/abs/10.1002/smj.2478 · PDF:
https://msbfile03.usc.edu/digitalmeasures/nwasserm/intellcont/Wasserman-2017-Strategic_Management_Journal-1.pdf
Verified (search-retrieved content). 6,130 startups: each retained dimension of founder
control (board control, CEO seat) associated with 17.1–22.0% lower pre-money valuation.
Supports: anti-entrenchment governance as investor signal. **Rating: C (explicitly
correlational).**

**[R-14] Breza, E., Kaur, S., & Shamdasani, Y. (2018). "The Morale Effects of Pay
Inequality." *Quarterly Journal of Economics* 133(2): 611–663.**
https://academic.oup.com/qje/article-abstract/133/2/611/4430649 ·
https://www.nber.org/papers/w22491
Verified (search-retrieved content). RCT: pay inequality with unobservable productivity
differences cuts output (−0.24 SD avg; −0.45 SD where hardest to observe) and attendance
(−12 to −18 p.p.); **no detectable harm when productivity differences are clearly
observable**. Supports: the transparency-first ledger design. **Rating: A (RCT; wage
context — equity extrapolation untested).**
**[R-14b] Shaw, J.D. (2014). "Pay Dispersion." *Annual Review of Organizational
Psychology and Organizational Behavior* 1: 521–544.**
https://www.annualreviews.org/content/journals/10.1146/annurev-orgpsych-031413-091253 —
Verified (search-retrieved content). Dispersion harms when unexplained + interdependent;
explained, performance-based dispersion neutral-to-positive. **Rating: B.**
**[R-14c] Bloom, M. (1999). *AMJ* 42(1): 25–40** (https://journals.aom.org/doi/10.5465/256872)
— dispersion negatively related to team performance in interdependent settings (MLB).
**Rating: C.** **Adams, J.S. (1965), equity theory,** *Adv. Exp. Soc. Psych.* 2: 267–299
(https://www.semanticscholar.org/paper/3deb24731c666197b87d456439c66b8311fb886a) —
foundational input/output-ratio fairness theory. **Rating: C (canonical).**
**de Wit, Greer & Jehn (2012), *JAP* 97(2): 360–390**
(https://pubmed.ncbi.nlm.nih.gov/21842974/) — meta-analysis, 116 studies: relationship
and process conflict reliably damage group outcomes. **Rating: B.**

## II. Governance & leadership (academic + case)

**[R-15] Wang, D., Waldman, D.A., & Zhang, Z. (2014). "A meta-analysis of shared
leadership and team effectiveness." *Journal of Applied Psychology* 99(2): 181–198.**
https://pubmed.ncbi.nlm.nih.gov/24188392/
Verified (search-retrieved content). 42 samples: shared leadership–effectiveness ρ = .34
(new-genre .34; traditional .18); stronger for complex work and attitudinal outcomes.
**Rating: B.**

**[R-16] Nicolaides, V.C., et al. (2014). "The shared leadership of teams." *The
Leadership Quarterly* 25(5): 923–942.**
https://www.sciencedirect.com/science/article/abs/pii/S1048984314000691
Verified (search-retrieved content) for design and moderators: shared leadership predicts
performance *over and above* vertical leadership; strongest under task interdependence;
mediated by team confidence. Exact overall ρ not confirmed this session (~.2–.3
envelope). Supports: shared leadership as complement, not substitute. **Rating: B.**

**[R-17] D'Innocenzo, L., Mathieu, J.E., & Kukenberger, M.R. (2016). *Journal of
Management* 42(7): 1964–1991.**
https://journals.sagepub.com/doi/10.1177/0149206314525205
Verified (search-retrieved content): 50 effect sizes, 3,198 teams; positive but
measurement-sensitive effects. Exact overall ρ (≈.21 as commonly cited) not confirmed
this session. **Rating: B.**

**[R-18] Lee, M.Y., & Edmondson, A.C. (2017). "Self-managing organizations." *Research in
Organizational Behavior* 37: 35–58.**
https://www.sciencedirect.com/science/article/abs/pii/S0191308517300059
Verified (search-retrieved content). Whole-company radical decentralization: evidence
"limited — only a few empirical studies," largely descriptive. **Rating: B (narrative
review).**

**[R-19] Eisenhardt, K.M. (1989). "Making fast strategic decisions in high-velocity
environments." *Academy of Management Journal* 32(3): 543–576.**
https://journals.aom.org/doi/10.5465/256434
Verified (search-retrieved content). Fast, high-performing deciders use more real-time
information, more simultaneous alternatives, experienced counselors, and "consensus with
qualification" (voice for all; the responsible executive decides if consensus doesn't
come quickly). **Rating: C (8-firm inductive).**
**[R-19b] Edmondson, A.C. (1999). *ASQ* 44(2): 350–383**
(https://journals.sagepub.com/doi/10.2307/2666999) — psychological safety → learning →
performance; voice without flatness. **Rating: C.**

**[R-20] Zappos holacracy record (journalism).**
https://fortune.com/2016/01/14/zappos-holacracy-losing-employees ·
https://time.com/4180791/zappos-holacracy-buyouts/ ·
https://qz.com/work/1776841/zappos-has-quietly-backed-away-from-holacracy
Verified (search-retrieved content, three independent outlets). 210/1,503 (14%) initial
buyouts, ~18% cumulative; program "quietly" abandoned by ~2020. Plus **Bernstein et al.
(2016), "Beyond the Holacracy Hype," *HBR***
(https://hbr.org/2016/07/beyond-the-holacracy-hype): adopt elements piecemeal. **Rating:
G + F (field-grounded).**

**[R-21] Feigen, M.A., Jenkins, M., & Warendh, A. (2022). "Is It Time to Consider
Co-CEOs?" *HBR* July–Aug 2022.** https://hbr.org/2022/07/is-it-time-to-consider-co-ceos
Verified (search-retrieved content). 87 public co-CEO firms: 9.5% vs 6.9% average annual
returns. Cited *against* our design and answered: tiny, selection-biased, practitioner-
grade. **Rating: F/G.**

**[R-22] Krause, R., Priem, R., & Love, L. (2015). "Who's in charge here?" *Strategic
Management Journal* 36(13): 2099–2110.**
https://sms.onlinelibrary.wiley.com/doi/abs/10.1002/smj.2325
Verified (search-retrieved content). Among co-CEO firms, a power *gap* improves
performance (inverted-U) — unity of command wins even inside shared titles. **Rating: C.**

**[R-23] Landeo, C.M., & Spier, K.E. (2014). "Irreconcilable Differences: Judicial
Resolution of Business Deadlock." *University of Chicago Law Review* 81(1).**
https://chicagounbound.uchicago.edu/uclrev/vol81/iss1/10/ · practitioner corroboration:
https://natlawreview.com/article/common-ways-to-resolve-disputes-and-deadlocks-5050-business
Verified (search-retrieved content). 50/50 deadlock routinely ends in forced buyout or
dissolution; pre-committed tiebreakers essential. **Rating: C (theory + lab) + F.**

**[R-24] Seibel, M. (Y Combinator). "How to split equity among founders" / YC Library.**
https://www.michaelseibel.com/blog/how-to-split-equity-among-founders ·
https://www.ycombinator.com/library/5x-how-to-split-equity-among-co-founders
Verified (search-retrieved content). Split near-equally; "99% of the work is left to be
done"; motivation over retrospective accounting. **The strongest practitioner
counter-position to contribution-metering — presented, not suppressed, in design §2/§10.**
**Rating: F.**
**[R-24b] Aghion, P., & Tirole, J. (1997). "Formal and Real Authority in Organizations."
*Journal of Political Economy* 105(1): 1–29.**
https://www.journals.uchicago.edu/doi/10.1086/262063 — Verified (search-retrieved
content). Formal vs. real authority; delegation buys initiative. Basis for domain-lead
design. **Rating: C (canonical theory).**

**[R-28] Garg, S. (2013). *AMR* 38(1): 90–108** (https://journals.aom.org/doi/10.5465/amr.2010.0193)
and **[R-29] Garg, S., & Furr, N. (2017). *SEJ* 11(3): 326–343**
(https://sms.onlinelibrary.wiley.com/doi/10.1002/sej.1258) — venture boards differ from
public boards (investor-director "principal problem"); scholarship young. Verified
(search-retrieved content). **Rating: C/B (theory + review).**

**[R-30] Early-stage board-size norms.** Mercury:
https://mercury.com/blog/early-stage-board-composition · MaRS:
https://learn.marsdd.com/article/whats-the-right-board-size-and-structure/
Verified (search-retrieved content). Convergent practitioner norm: 3 at seed
(2 common + 1 investor), 5 at Series A, odd numbers. **Rating: F.**

Also consulted: **Jin, L., et al. (2017), *ETP* 41(5): 743–771**
(https://journals.sagepub.com/doi/abs/10.1111/etap.12232) — meta-analysis: team human
capital/diversity beat team *size* as performance predictors (**B**); **Greenberg &
Mollick (2018), SSRN 3107898** (https://papers.ssrn.com/sol3/papers.cfm?abstract_id=3107898)
— solo founders ≥ pairs on survival/revenue in a crowdfunding sample (working paper,
non-representative; **C−**). Nothing specific to five-founder teams exists — stated in
design §10.

## III. Contribution frameworks & compensation benchmarks (practitioner)

**[R-45] Slicing Pie (Moyer): multipliers & mechanics.**
https://slicingpie.com/the-magic-of-mutipliers/ ·
https://slicingpie.com/wp-content/uploads/2017/02/Slicing-Pie-Grunt-Fund-Cheat-Sheet.pdf ·
third-party walkthrough: https://equitymatrix.io/blog/slicing-pie-guide
Verified (search-retrieved content). Slices = FMV × 2 (non-cash) / × 4 (cash); "Well"
cash slices only when spent; model terminates ("bakes") at breakeven or Series A.
**Rating: F (no peer-reviewed evaluation exists — stated in design §5.2/§10).**
**[R-45b] Recovery framework:** https://slicingpie.com/slices-that-can-survive-separation/
· https://slicingpie.com/the-good-way-to-say-good-bye/ — for-cause/no-good-reason leavers
lose non-cash slices, keep 1× cash; no-fault leavers keep slices. We adopt a softened
version (design §6.4). **Rating: F.**
**[R-45c] Pie Slicer software:**
https://support.thepieslicer.com/article/show/66673-what-is-the-pie-slicer **Rating: F.**

**[R-46] Sentient Law, "The Truth About Slicing Pie."**
https://www.sentientlaw.com/dynamic-equity-slicing-pie/
Verified (search-retrieved content). Implementing attorney: US legal/tax framework "not
geared towards dynamic equity"; in-practice claim that it "virtually eliminated equity
disputes"; terminate before valuation events. **Rating: F (interested practitioner).**

**[R-47] Equity Matrix, "Slicing Pie problems."**
https://equitymatrix.io/blog/slicing-pie-problems
Verified (search-retrieved content). Failure-mode catalog: rate disputes, time inflation,
no cliff, tracking decay, investor confusion. (Competing vendor — bias noted; the
specific failure modes are concrete and design-actionable.) **Rating: F/G.**

**[R-48] Fairsquare LLP, "Investors and Slicing Pie."**
https://www.fairsquarellp.com/investors-and-slicing-pie/
Verified (search-retrieved content). Sympathetic implementer conceding priced rounds
require crystallized fixed shares. **Rating: F/G.**

**[R-49] Levels.fyi salary benchmarks (2025).**
https://www.levels.fyi/2024/ · https://www.levels.fyi/t/software-engineer/locations/united-states
Verified (search-retrieved content). US SWE median total comp ≈$192.5K; senior (L5)
median ≈$312K (2025). Named benchmark source for Schedule B. **Rating: E (self-reported +
offer-verified).**

**[R-50] Forbes Legal Council (2017), "Overcoming the Misconceptions of Dynamic Equity."**
https://www.forbes.com/sites/forbeslegalcouncil/2017/12/12/overcoming-the-misconceptions-of-dynamic-equity/
Verified (search-retrieved content). Rolling issuance creates tax/admin drag in
corporations; LLCs can adjust percentages without equivalent tax events — the entity-
sequencing patch we adopt. **Rating: F.**

**[R-51] Spolsky, J. "Totally Fair Method to Divide Up the Ownership of Any Startup."**
https://gist.github.com/isaacsanders/1653078
**Verified (direct fetch).** Fairness > stake size; layer-based equal splits; "ideas earn
nothing"; unpaid salary should be IOU/cash, not extra equity. Used for: ideas-earn-nothing
principle; fairness-perception framing. **Rating: F (most-cited practitioner answer in
the genre).**

**[R-52] ML consulting market rates.**
https://www.opinosis-analytics.com/blog/machine-learning-consulting-rates/ ·
https://www.contractrates.fyi/Data-Science-Machine-Learning-Consulting/hourly-rates
Verified (search-retrieved content). PhD-level ML consulting $250–500/h (up to $1,000);
crowdsourced average day rate ≈$787. Basis for the professor's documented-market-rate
mechanism. **Rating: F/E− (thin; flagged as such — the OA requires his *own documented
invoiced rate*, not these aggregates).**

**[R-31] Carta vesting norms.** https://carta.com/learn/equity/stock-options/vesting/
Verified (search-retrieved content). 92% of venture-backed companies implement founder
vesting; standard 4-year/1-year cliff. **Rating: E.**
**[R-31b] Pool sizes:** Carta median seed employee pool 12.1%
(https://carta.com/data/founder-ownership-2026/); Index Ventures OptionPlan seed ESOP
12.5–15%, range 10–15% (https://www.indexventures.com/rewarding-talent/esop-size-at-seed).
**Rating: E/F.**
**[R-31c] Acceleration norms:** Cooley GO
(https://www.cooleygo.com/what-are-single-and-double-trigger-acceleration-and-how-do-they-work/);
Open Guide to Equity Compensation — **verified (direct fetch)**
(https://github.com/jlevy/og-equity-compensation); Holloway Guide
(https://www.holloway.com/g/equity-compensation). **Rating: F.**

**[R-32] Cooley GO, "Founder's Stock, Vesting and Founder Departures."**
https://www.cooleygo.com/founder-basics-founders-stock/
Verified (search-retrieved content). Investors "very likely" to require vesting as a
condition of investment; typically want founders ≤~40% vested at Series A; endorses
"retroactive credit reflecting their respective periods of work before incorporation"
(back-vesting). **Rating: F (canonical startup-law explainer).**

**[R-33] Dead-equity thresholds.**
https://isaventures.substack.com/p/dead-equity-on-your-cap-table-is ·
https://equitymatrix.io/blog/what-investors-look-for-in-cap-tables
Verified (search-retrieved content). Departed cofounder at 25–40% = deal-killer; >2%
inactive stakes flagged; advisors 0.1–1% each, ≤5% aggregate; founders <50% at seed a red
flag. **Rating: G (named-investor opinion; treated as tolerance bands, not data).**

**[R-34] Founder-vesting/dead-equity essays.** Wilson:
https://avc.com/2018/03/founder-vesting/ · Jolis (Matrix/TechCrunch):
https://techcrunch.com/2020/10/17/solve-the-dead-equity-problem-with-a-longer-founder-vesting-schedule/
Verified (search-retrieved content). Worked example: 2.5-year quitter keeps ~22% under
4-year vesting vs ~11% under 8-year; "the opportunity cost of dead equity is talent and
capital." **Rating: F.**
**[R-34b] Index Ventures, "Rewarding Talent" — how much and who gets it.**
https://www.indexventures.com/rewarding-talent/how-much-and-who-gets-it — 2–3% grants
defensible for exceptional deep-tech hires. **Rating: F/E.**
Also: **Carta first-10-hire grant medians** (#1: 1.49%, #2: 0.85%, #3: 0.50%; founding
engineer median 1.54%, IQR 0.61–3.5%) —
https://carta.com/data/linkedin-founding-engineer-equity-1-54-percent/ ·
https://community.carta.com/c/corporations-updates/equity-for-your-first-8-hires
**Rating: E.** (Context check that our worked example's employee outcomes are generous
relative to salaried-market norms — appropriate, since these people were unpaid.)

## IV. Entity, tax, investor structuring

**[R-25] Cooley GO, "Choosing the Correct Business Entity: The Basics."**
https://www.cooleygo.com/choosing-correct-business-entity-basics/
Verified (search-retrieved content). VC funds avoid flow-throughs because tax-exempt LPs
would incur UBTI → corporations. **Rating: F (top firm).**

**[R-26] PitchBook (Carta data), "Startups aren't abandoning Delaware—yet."**
https://pitchbook.com/news/articles/startups-arent-abandoning-delaware-yet
Verified (search-retrieved content). ~88% of C-corp startups on Carta are Delaware-
incorporated (late 2024). (A circulating "99%" marketing figure was rejected as
unsupported.) **Rating: E.**

**[R-27] NVCA Model Legal Documents.**
https://nvca.org/press_releases/nvca-updates-model-legal-documents-to-support-venture-ecosystem/ ·
https://www.morganlewis.com/pubs/2024/09/whats-new-in-the-nvca-model-legal-documents-and-whats-next
Verified (search-retrieved content). The standard financing stack assumes a Delaware
corporation. **Rating: D−/F (industry-standard documents + firm commentary).**

**[R-35] SAFEs and LLCs.**
https://www.mintz.com/insights-center/viewpoints/2911/2019-02-01-llcs-and-convertible-debt-too-good-be-true
Verified (search-retrieved content). Standard (YC) SAFE presumes a corporation;
LLC-adapted instruments carry tax uncertainty and investor resistance. **Rating: F.**

**[R-56] Profits interests.** Rev. Proc. 93-27; Rev. Proc. 2001-43:
https://www.irs.gov/pub/irs-drop/rp-01-43.pdf · practitioner:
https://www.thetaxadviser.com/issues/2025/jan/profits-interests-the-most-tax-efficient-equity-grant-to-employees/
Verified (search-retrieved content; IRS primary located). No tax at grant if conditions
met; unvested interests tested at grant; protective 83(b)s customary. **Rating: D + F.**
**[R-56b] Rev. Rul. 69-184 (partner ≠ employee).**
https://bradfordtaxinstitute.com/Endnotes/Rev_Rul_69-184.pdf ·
https://rsmus.com/insights/services/business-tax/frequently-asked-questions-about-profits-interests.html
— profits-interest holders become K-1 partners (SE tax, no W-2). **Rating: D + F.**
**[R-56c] Phantom units / UARs.**
https://natlawreview.com/article/equity-and-phantom-equity-based-compensation-llcs ·
https://carta.com/learn/startups/compensation/equity-incentive-plans/phantom-equity/ —
keep workers W-2 at the cost of ordinary-income treatment; §409A applies. **Rating: F.**

**[R-57] QSBS post-OBBBA (July 4, 2025).**
https://www.hklaw.com/en/insights/publications/2025/07/one-big-beautiful-bill-act-increases-tax-benefits-for-qualified-small ·
https://www.thetaxadviser.com/issues/2025/nov/qsbs-gets-a-makeover-what-tax-pros-need-to-know-about-sec-1202s-new-look/
Verified (search-retrieved content; cross-confirmed across ≥4 firm alerts). For stock
issued after 7/4/2025: 50%/75%/100% exclusion at 3/4/5 years; per-issuer cap $15M (or
10× basis); gross-asset ceiling $75M; non-excluded portions at the 50/75 tiers taxed at
28%; pre-existing stock grandfathered under old rules ($10M, 5-year cliff) — the single
most-garbled detail in secondary coverage, resolved per law-firm/AICPA consensus.
**Rating: D (statute) via F (firm alerts) — flagged for counsel confirmation.**
**[R-57b] FBT Gibbons, LLC→C-corp QSBS conversion series.**
https://fbtgibbons.com/guide-to-converting-partnerships-into-c-corporation-issuers-of-qsbs-part-1/ ·
https://frostbrowntodd.com/corporations-are-eligible-to-issue-qualified-small-business-stock-qsbs-only-if-they-satisfy-section-1202s-aggregate-gross-assets-test/
Verified (search-retrieved content). Basis = FMV at conversion (larger 10× cap if
converting when appreciated; FMV also counts against the asset test); LLC interests are
never QSBS; clock starts at conversion. **Rating: F (leading §1202 practitioners).**
**[R-57c] Rev. Rul. 84-111 / §351 incorporation methods.**
https://www.thetaxadviser.com/issues/2007/apr/incorporatingapartnershiporllcdoesrevrul84-111needupdating/
Verified (search-retrieved content). Assets-over / assets-up / interests-over, generally
tax-free with 80% control. **Rating: D + F.**

**[R-58] 83(b) mechanics.** https://carta.com/learn/equity/stock-options/taxes/83b-election/ ·
https://www.haynesboone.com/news/blogs/mechanics-of-making-an-83b-election-and-irs-revocation-guidance
Verified (search-retrieved content). 30-day non-extendable deadline; Form 15620 with
e-filing since July 2025. **Rating: F (rule itself is D: IRC §83(b)).**

**[R-44] Rule 701 + blue sky.**
https://www.goodwinlaw.com/en/insights/publications/2018/01/01_30_18_rule-701-refresher-and-updates ·
https://pulley.com/guides/what-is-the-rule-701-exemption ·
https://marketedge.dlapiper.com/2026/03/sec-issues-new-and-revised-guidance-related-to-rule-701/ ·
MA: https://www.law.cornell.edu/regulations/massachusetts/950-CMR-14-402
Verified (search-retrieved content). Written compensatory plan; $10M/12-month enhanced-
disclosure trigger; no state preemption — Massachusetts exemption subsection (950 CMR
14.402(B) family) flagged for counsel confirmation. **Rating: D + F.**

**[R-66] IP assignment diligence.**
https://www.cooleygo.com/glossary/confidential-information-and-inventions-assignment-agreements/ ·
https://www.orrick.com/en/tech-studio/forms/Employee-Confidential-Information-and-Invention-Assignment-Agreement ·
https://www.cooleygo.com/documents/sample-vc-due-diligence-request-list/
Verified (search-retrieved content). Present-assignment CIIAAs from every contributor;
missing assignments the most common early-stage diligence gap; cured by confirmatory
assignments. **Rating: F (canonical forms).**

## V. Massachusetts & employment law (primary unless noted)

**[R-36] M.G.L. c. 149 § 148 (Wage Act) and § 150 (remedies).**
https://malegislature.gov/Laws/GeneralLaws/PartI/TitleXXI/Chapter149/Section148 ·
https://malegislature.gov/Laws/GeneralLaws/PartI/TitleXXI/Chapter149/Section150
Verified (search-retrieved content; statutory text quoted verbatim in results). Timely-
payment duties; no waiver "by special contract"; § 150: prevailing employee "shall be
awarded treble damages, as liquidated damages... and... costs... and reasonable
attorneys' fees"; 3-year limitations. **Rating: D.**

**[R-37] *Reuter v. City of Methuen*, 489 Mass. 465 (2022).**
https://law.justia.com/cases/massachusetts/supreme-court/2022/sjc-13121.html · analysis:
https://www.seyfarth.com/news-insights/no-quarter-sjc-mandates-treble-damages-for-any-late-payment-of-wages-even-honest-corrected-mistakes.html
Verified (search-retrieved content). Treble damages on the full late-paid amount, even
for honest mistakes cured before suit. **Rating: D.**

**[R-38] *Cook v. Patient Edu, LLC*, 465 Mass. 548 (2013).**
https://foleyhoag.com/news-and-insights/publications/alerts-and-updates/2013/june/ma-highest-court-decides-that-managers-at-llcs-can-be-individually-liable-for-wage-act-violations/ ·
https://www.duanemorris.com/alerts/applicability_of_massachusetts_wage_act_swells_in_june_2013_4918.html
Verified (search-retrieved content; holding corroborated across four firms). LLC managers
who "control, direct, and participate to a substantial degree in formulating and
determining policy" are personally liable (civil and criminal). **Rating: D (via
corroborated secondary).**

**[R-39] M.G.L. c. 156C — LLC Act; conversion/merger mechanics.**
https://malegislature.gov/Laws/GeneralLaws/PartI/TitleXXII/Chapter156C ·
§ 69: https://malegislature.gov/Laws/GeneralLaws/PartI/TitleXXII/Chapter156C/Section69 ·
§ 60: https://malegislature.gov/Laws/GeneralLaws/PartI/TitleXXII/Chapter156C/Section60
Partially verified: § 69 conversion is inbound-to-LLC only and MA provides no outbound
statutory conversion (two independent practitioner sources concur; one vendor site claims
otherwise and was rejected) — merger route under §§ 59–63 with >50%-of-unreturned-
contributions approval. **The one item we most want counsel to confirm against current
statutory text.** **Rating: D with flagged uncertainty.**

**[R-40] U.S. DOL, elaws FLSA Advisor — Volunteers.**
https://webapps.dol.gov/elaws/whd/flsa/docs/volunteers.asp
Verified (search-retrieved content). "Under the FLSA, employees may not volunteer
services to for-profit private sector employers." **Rating: D (agency guidance).**

**[R-41] Massachusetts minimum wage ($15.00/h, G.L. c. 151 § 1).**
https://www.mass.gov/info-details/massachusetts-law-about-minimum-wage — Verified
(search-retrieved content). **Rating: D.**
**[R-41b] Foley & Lardner (Oct 2024), "Compensating Employees With Equity Alone Likely
Violates the FLSA."**
https://www.foley.com/insights/publications/2024/10/equity-compensate-employees-violates-flsa/
Verified (search-retrieved content). Equity satisfies neither minimum wage nor the salary
basis test; narrow 20%+ owner-manager exemption (29 C.F.R. § 541.101). **Rating: F.**

**[R-42] M.G.L. c. 149 § 148B (ABC test) + AG Advisory 2008/1.**
https://malegislature.gov/Laws/GeneralLaws/PartI/TitleXXI/Chapter149/Section148b ·
https://www.mass.gov/doc/attorney-generals-advisory-on-the-independent-contractor-law/download
Verified (search-retrieved content). Employee unless all three prongs met; prong B
(service outside the usual course of the employer's business) defeats contractor
relabeling of core contributors. **Rating: D.**

**[R-43] Close-corporation fiduciary duties extended to LLCs.** *Donahue v. Rodd
Electrotype*, 367 Mass. 578 (1975):
https://law.justia.com/cases/massachusetts/supreme-court/1975/367-mass-578-2.html ·
*Allison v. Eriksson*, 479 Mass. 626 (2018) analysis:
https://bostonbar.org/journal/fiduciary-duties-in-massachusetts-and-delaware-closely-held-corporations/
Verified (search-retrieved content). "Utmost good faith and loyalty" among close-corp
holders; applied to LLC freeze-outs. **Rating: D.**
**[R-43b] Duty-modification contrast.** M.G.L. c. 156C § 63:
https://law.justia.com/codes/massachusetts/part-i/title-xxii/chapter-156c/section-63/ ·
6 Del. C. § 18-1101: https://delcode.delaware.gov/title6/c018/sc11/
Verified (search-retrieved content). MA: duties may be "expanded or restricted"; DE: may
be "eliminate[d]" (floor: implied covenant). **Rating: D.**

**[R-67] Massachusetts Noncompetition Agreement Act, G.L. c. 149 § 24L.**
https://www.mass.gov/info-details/mass-general-laws-c149-ss-24l ·
https://beckreedriden.com/the-massachusetts-noncompetition-agreement-act-massachusetts-general-laws-c-149-s-24l/
Verified (search-retrieved content). Garden leave (≥50% of highest base over prior
2 years) or other agreed consideration; 12-month cap; unenforceable against without-cause
terminations and non-exempt employees; NDAs/nonsolicits unaffected. **Rating: D + F.**

## VI. Advisors, star scientists, the professor

**[R-53] Carta advisor-grant data.**
https://carta.com/data/linkedin-startup-advisor-equity-cheatsheet/ ·
https://carta.com/data/linkedin-preseed-advisor-equity-h1-2023/ ·
https://carta.com/learn/startups/equity-management/advisory-shares/
Verified (search-retrieved content). 20,000+ advisors: medians ~0.21–0.275% pre-seed,
~0.12–0.165% seed, ~0.05–0.093% Series A, trending down; only ~10% of pre-seed advisors
get ≥1%; modal vesting 2-year monthly, no cliff; single-trigger acceleration customary
(Holloway:
https://www.holloway.com/g/equity-compensation/sections/typical-startup-advisor-equity-levels).
**Rating: E.**

**[R-54] Founder Institute FAST Agreement.** https://fi.co/fast
Verified (search-retrieved content + GitHub-mirrored corroboration). Standardized grid
~0.1–1.0%: 1.0% only for expert-level engagement at idea/pre-seed stage; 2-year monthly
vesting, no cliff. (Reports of a 2026 v3 revision raising floor tiers noted but not
independently confirmed — flagged.) **Rating: F (industry-standard template).**

**[R-55] Booth, B. (Atlas Venture). "Biotech Scientific Advisory Boards: What Works, What
Doesn't." LifeSciVC (2012).**
https://lifescivc.com/2012/09/biotech-scientific-advisory-boards-what-works-what-doesnt/
Verified (search-retrieved content). Typical SAB member: $2.5–5K/day + 0.1–0.3% equity;
SAB total ~1%; star scientists "much, much more expensive" and often low-engagement —
cautionary. **Rating: F (top-tier VC practitioner).**

**[R-59] Star-scientist engagement literature.** Zucker, Darby & Brewer (1998), *AER*
88(1): 290–306 — https://www.nber.org/papers/w4653 (star scientists drive biotech firm
births; **C+/A−**); Zucker & Darby, NBER Reporter (1998) —
https://www.nber.org/reporter/fall-1998/entrepreneurs-star-scientists-and-biotechnology
(benefits require hands-on collaboration, not affiliation); Toole & Czarnitzki (2009),
*Management Science* 55(1): 101–114 — https://www.researchgate.net/publication/45132636
(academic human capital helps only when matched to real firm tasks; **C**); Murray
(2004), *Research Policy* 33(4): 643–659 — https://escholarship.org/uc/item/38f3j3dg
(academics contribute lab know-how + networks/students; **C**). All verified
(search-retrieved content/citations).

**[R-60] Higgins, M.J., Stephan, P.E., & Thursby, J.G. (2011). "Conveying quality and
value in emerging industries: Star scientists and the role of signals in biotechnology."
*Research Policy* 40(4): 605–617.**
https://www.sciencedirect.com/science/article/abs/pii/S0048733311000151 ·
https://www.nber.org/papers/w14602
Verified (search-retrieved content). Nobel-laureate affiliation raised early-era biotech
IPO proceeds by >$30M; the signal "lost its luster" as investors learned to price
substance. Best pro-and-con evidence on name-value. **Rating: C.**

**[R-61] Affiliation/signaling studies.** Stuart, Hoang & Hybels (1999), *ASQ* 44(2):
315–349 — https://journals.sagepub.com/doi/10.2307/2666998 (prominent affiliates →
faster, richer IPOs; strongest when quality most uncertain; **C**); Hsu (2004), *Journal
of Finance* 59(4): 1805–1844 —
https://onlinelibrary.wiley.com/doi/abs/10.1111/j.1540-6261.2004.00680.x (affiliation is
priceable: 3× acceptance odds, 10–14% valuation discount for reputable VCs; **C+**);
Plummer, Allison & Connelly (2016), *AMJ* 59(5): 1585–1604 —
https://journals.aom.org/doi/10.5465/amj.2013.0100 (affiliations amplify other signals;
**C**). Verified (search-retrieved content/citations).
Also: Graham, P. (2006), "The 18 Mistakes That Kill Startups" —
https://paulgraham.com/startupmistakes.html (part-time commitment as leading failure
signal; **F**); Calacanis advisor norms (0.25–0.5%, ≥50 h/yr commitment) — GitHub-
mirrored checklist **verified (direct fetch)** plus
https://fi.co/insight/founder-advisor-template-agreement-jason-calacanis (**F/G**).

## VII. Yale & federal research policies (primary)

**[R-62] Yale Faculty Handbook (July 1, 2025), § XX.E — outside activities.**
https://provost.yale.edu/sites/default/files/files/July_1_2025%20Faculty%20Handbook.pdf
Verified (search-retrieved content, corroborated by Yale COI FAQ). Consulting limited to
"no more than one day per seven-day week" during full-time Yale service; day-to-day
management roles in outside entities restricted. **Rating: D (university policy).**

**[R-63] Yale Conflict of Interest policy & Provost guidance.**
https://research-support.yale.edu/sites/default/files/2025-03/coi_policy_0.pdf ·
https://provost.yale.edu/policies/external-professional-activities-guidance ·
https://research-support.yale.edu/research-compliance/conflict-of-interest-office/frequently-asked-questions
Verified (search-retrieved content). Annual + ad hoc disclosure of outside equity;
Provost's COI Committee management plans; student involvement a flagged scenario.
**Rating: D.**

**[R-64] Yale Patent Policy & consulting guidance.**
https://ventures.yale.edu/sites/default/files/2023-03/Yale_Patent_Policy.pdf ·
https://ventures.yale.edu/programs/consulting-guidance
Verified (search-retrieved content). Yale owns inventions made with significant use of
university funds/facilities; consulting inventions reportable to Yale Ventures; Yale's
standard startup license takes 3% (software) – 5% of founder shares. **Rating: D.**

**[R-65] NIH/PHS financial conflict of interest regulation, 42 C.F.R. Part 50 Subpart F.**
https://www.ecfr.gov/current/title-42/chapter-I/subchapter-D/part-50/subpart-F ·
https://www.law.cornell.edu/cfr/text/42/50.603
Verified (search-retrieved content). Any equity in a non-publicly-traded entity is a
"significant financial interest" for PHS-funded investigators, regardless of value.
**Rating: D.**

---

## Claims we deliberately did NOT rely on (found wanting during research)

1. "65% of startups fail because of cofounder conflict" — misquote of Wasserman's
   people-problems attribution statistic [R-3].
2. "Equal splits cause failure" — the association is selection-confounded [R-1].
3. Any peer-reviewed validation of Slicing Pie or dynamic equity — none exists.
4. "99% of VC-backed companies are Delaware C-corps" — marketing figure; used ~88%/">90%"
   from Carta/PitchBook instead [R-26].
5. Huawei's rotating-CEO system as evidence for rotating leadership — anecdote,
   unverified, no outcome data.
6. The "only 9% successfully renegotiate equity" statistic — single vendor blog, no
   methodology.
7. Causal evidence that vesting improves outcomes — motivated by theory [R-6] and
   departure base rates [R-8], not demonstrated causally.
8. A paper "Squaring the founders' circle" — appears not to exist.
9. FAST v3's full 2026 grid — reported by secondaries; unconfirmed against fi.co.

*— plan5*
