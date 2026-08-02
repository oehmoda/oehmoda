# plan9 — Full Governance & Equity Design
### For a five-founder, ~10-employee Massachusetts LLC, one year in, everyone unpaid

**Team:** plan9 · **Date:** August 2026 · **Status:** Business-terms design for counsel (not legal advice)

---

## 0. How to read this document

Part I summarizes what our research actually found, with honest strength ratings. Part II is the design itself: a **two-phase dynamic-equity system** ("the Contribution Ledger") wrapped in a **single-accountable-executive, elected-board governance structure**, with a hard **Crystallization** event that converts the dynamic system into a conventional, investor-standard cap table before any priced round. Part III covers limitations. Every substantive claim carries an inline citation; the annotated bibliography with per-source evidence ratings is in `plan-9-references.md`.

**Verification disclosure (applies to all four documents).** This work was produced in a sandboxed environment whose egress policy blocked full-page fetches of most external sites (HTTP 403 at the proxy). Citations are therefore verified at one of three levels, disclosed per-source in the references file: **[F]** full text fetched and read (GitHub-hosted primary documents and mirrors); **[S]** URL verified live via search-engine index (title + content excerpt returned this session — the URL exists, but full text was not fetched); **[U]** unverified lead (named but not cited for any load-bearing claim). No URL in these documents was constructed from memory. Counsel and the founders should pull primary documents before relying on any single number.

**Isolation note:** We did not read, check out, diff, or browse any other team's branch or files at any point. Work began on an empty orphan branch.

---

# Part I — What the evidence says

## I.1 Static equal splits are the well-documented failure mode

The single most-cited empirical result on founder equity is Hellmann & Wasserman's study of 1,476 founders across 511 ventures: **32% of teams split exactly equally**, **73% of teams split within the first month** of founding — at peak uncertainty about who will actually contribute what — and teams that split equally after a "quick handshake" negotiation are **less likely to raise outside financing and show lower pre-money valuations at first financing**, with roughly **$450K NPV (~25% of an average founder's stake)** at issue ([Hellmann & Wasserman 2017, *Management Science*](https://pubsonline.informs.org/doi/10.1287/mnsc.2016.2474); open working-paper version at [NBER w16922](https://www.nber.org/papers/w16922)). This is correlational — the authors are explicit that fast-equal-splitting teams differ in unobserved ways — but the direction replicates in a registry panel of **24,194 German startups**, where unequal-split teams show a **1.3 percentage-point higher 3-year growth rate** and higher subsequent team entry ([Mueller & Hennicke 2024, *European Management Journal*](https://www.sciencedirect.com/science/article/abs/pii/S0263237322001785)).

The causal mechanism has been isolated in the lab: in real-effort venture experiments, **equal-split contracts encourage free-riding and are disproportionately chosen by the least desirable collaborator types**, while performance-contingent equity screens and motivates; critically, **delaying the split lets founders learn each other's types before committing** ([Kagan, Leider & Lovejoy 2020, *Management Science* — experimental, causal within lab](https://pubsonline.informs.org/doi/10.1287/mnsc.2019.3439)).

This team has already lived the prediction: an early informal equal-partners deal, divergence of actual contribution, and now inactive founders holding presumptive equal shares. The research says the fix is not a better one-time static split (which would re-encode today's guesses about the future) but an allocation that **tracks contribution over time and is settled when uncertainty is lower**.

**Counter-evidence, reported honestly:** equal splits have become *more* common in practice, not less — Carta's cap-table data shows 2-person equal splits rising from 31.5% (2015) to 45.9% (2024) ([Carta founder-equity-split trends, 2024](https://carta.com/data/founder-equity-split-trends-2024/) [S]); and Y Combinator explicitly advises near-equal splits for teams that will all "work hard going forward," on motivation grounds ([YC Startup Legal Mechanics, Carolynn Levy et al.](https://raw.githubusercontent.com/shun-liang/yt2doc/main/examples/Carolynn%20Levy%20And%20Panel%20(Jon%20Levy%2C%20Jason%20Kwon)%20-%20Startup%20Legal%20Mechanics.md) [F-mirror]). The YC advice, however, presupposes the condition this company has already lost: that all founders remain comparably committed. Once contributions have visibly diverged, the fairness literature (next section) says an equal or reserved-heavy split is the *toxic* option, not the safe one.

## I.2 Perceived justice, not equality, is what protects the team

A six-month observational study of eight founding teams found that **the perceived justice of the equity distribution — not the distribution itself — drives team interaction spirals**: high perceived justice produces reinforcing cooperation; low perceived justice produces conflict and departures ([Breugst, Patzelt & Rathgeber 2015, *Journal of Business Venturing*](https://www.sciencedirect.com/science/article/abs/pii/S0883902614000676)). Procedural fairness — voice, transparency, consistent process — independently builds stakeholder trust and commitment in venture settings ([Sapienza & Korsgaard 1996, *AMJ*](https://journals.aom.org/doi/10.5465/256655)). And founder equity stakes show an **inverted-U relationship with identification with the team** — marginalizing some holders to near-zero carries cohesion costs, just as over-concentration does ([Weissenböck, Breugst, Patzelt & Dibbern 2024, *Applied Psychology*](https://iaap-journals.onlinelibrary.wiley.com/doi/full/10.1111/apps.12515)).

Design consequence: the system must be **procedurally airtight** — published formula, published rates, verifiable inputs, appeal rights — because the *process* is what makes an unequal outcome survivable. This is also the answer to the professor's premium (I.7).

## I.3 Contribution measurement: identifiability kills free-riding

Social loafing is one of the most robust effects in group psychology (meta-analysis of 78 studies), and it is **eliminated when individual outputs are identifiable and evaluable** ([Karau & Williams 1993, *JPSP* — meta-analysis of experiments, causal at mechanism level](http://www.psych.purdue.edu/~willia55/392F-'06/KarauWilliamsMetaAnalysisJPSP.pdf)). Teams using **peer evaluation** show higher workload sharing, voice, cooperation, and performance than externally evaluated teams (quasi-experiment, 38 self-managed teams: [Erez, LePine & Elms 2002, *Personnel Psychology*](https://asu.elsevierpure.com/en/publications/effects-of-rotated-leadership-and-peer-evaluation-on-the-function/)). The classic economics of team production reaches the same conclusion from the other direction: where individual marginal products are hard to meter, shirking follows, and the remedy is monitoring tied to residual claims ([Alchian & Demsetz 1972, *AER*](https://josephmahoney.web.illinois.edu/BA549_Fall%202010/Session%205/Alchian_Demsetz%20(1972).pdf)).

Design consequence: a ledger in which **every credited hour maps to an identifiable work item**, verified monthly, with peer-verification sampling — not a subjective annual "impact score."

## I.4 Dynamic equity: strong indirect evidence, no direct peer-reviewed validation — say so

The best-known operational framework for contribution-based equity is Mike Moyer's **Slicing Pie**: each participant's share = their "slices" ÷ all slices, where slices = fair-market value of contributions × a risk multiplier (**2× for non-cash contributions such as unpaid time; 4× for cash**), recalculated continuously until the pie **"bakes"** (freezes) at breakeven or a priced round ([Slicing Pie, "The Magic of Multipliers"](https://slicingpie.com/the-magic-of-mutipliers/) [S]; mechanics corroborated in two independently fetched derivative specs [F-mirror], see references). Its separation rules: termination **for cause or resignation without good reason forfeits non-cash slices** (expenses repaid when possible); termination **without cause or resignation with good reason keeps them** ([Slicing Pie, "Slices that Can Survive Separation"](https://slicingpie.com/slices-that-can-survive-separation/) [S]).

**Honest status of the evidence:** we found **no peer-reviewed study evaluating Slicing Pie itself**. Its support is (a) the Kagan et al. experiment showing delayed, contingent contracting dominates early equal splits (causal, lab); (b) the identifiability/peer-evaluation literature (I.3); (c) Hellmann & Wasserman's finding that only ~10% of teams adopt milestone-based vesting and that time-based vesting is "a weak proxy for value creation" ([Wasserman practitioner summary](https://www.noamwasserman.com/splitting-the-pie-founding-team-equity-splits/) [S]). Known practitioner criticisms: no built-in cliff, open-ended cap table alarms investors, conversion pain at institutional rounds, and tax complexity ([compiled practitioner reference, lawve-ai/awesome-legal-skills](https://raw.githubusercontent.com/lawve-ai/awesome-legal-skills/main/skills/founder-agreement-drafting-stephane-boghossian/REFERENCE.md) [F-mirror]; [Vestd critique](https://www.vestd.com/blog/slicing-pie-a-tasty-way-to-share-equity) [S]). Our design adopts the Slicing Pie *engine* but bounds it with a hard crystallization date and standard forward vesting specifically to neutralize those criticisms (II.9).

## I.5 Leadership: single accountable executive, shared leadership beneath — and no entrenchment

Three meta-analyses find **shared leadership positively predicts team effectiveness** — overall ρ ≈ .34 in [Wang, Waldman & Zhang 2014, *J. Applied Psychology*, 42 samples](https://pubmed.ncbi.nlm.nih.gov/24188392/); positive with network-based measures strongest in [D'Innocenzo, Mathieu & Kukenberger 2016, *J. Management*, 50 effect sizes](https://journals.sagepub.com/doi/10.1177/0149206314525205); mediated by team confidence in [Nicolaides et al. 2014, *Leadership Quarterly*](https://www.sciencedirect.com/science/article/abs/pii/S1048984314000691). But these study *team-level* leadership behaviors, mostly on attitudinal and behavioral outcomes — they are **not** evidence for co-equal command at the top. The co-CEO evidence points the other way: across 71 public co-CEO pairs, performance follows an **inverted-U in the power gap between the co-CEOs — truly co-equal command underperforms a moderate hierarchy** ([Krause, Priem & Love 2015, *SMJ*](https://sms.onlinelibrary.wiley.com/doi/abs/10.1002/smj.2325)); the favorable HBR co-CEO study (87 firms, 9.5% vs 6.9% annual returns) is non-peer-reviewed and survivorship-biased ([Feigen, Jenkins & Warendh 2022, HBR](https://hbr.org/2022/07/is-it-time-to-consider-co-ceos)).

On founders and control, the literature genuinely disagrees, and the disagreement is informative:

- **Founder control is expensive:** each additional lever of founder control (board control, CEO seat) is associated with **17–22% lower pre-money valuations** ([Wasserman 2017, *SMJ*](https://sms.onlinelibrary.wiley.com/doi/abs/10.1002/smj.2478)).
- **Founder replacement can help:** instrumenting with state non-compete-law changes, VC-driven founder replacement **causally improves** exit outcomes ([Ewens & Marx 2018, *RFS* — IV, causal](https://academic.oup.com/rfs/article-abstract/31/4/1532/4604800)).
- **Founder loss destroys innovation:** using CEO sudden deaths as natural experiments, replacing a founder-CEO with a professional causes a **43.8% drop in citation-weighted patents** ([Lee, Kim & Bae 2020, *Research Policy* — quasi-causal](https://www.sciencedirect.com/science/article/abs/pii/S0048733319301817)); founder-CEO public firms earned 4.4–8.3%/yr abnormal returns ([Fahlenbrach 2009, *JFQA*](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=606527)).

The reconciliation the field itself offers: **founder involvement is valuable; founder monopoly on control is what costs money.** Half of founder-CEOs are gone by year three anyway ([Wasserman 2008, HBR](https://hbr.org/2008/02/the-founders-dilemma)), and succession hazard *rises* with success milestones ([Wasserman 2003, *Organization Science*](https://pubsonline.informs.org/doi/10.1287/orsc.14.2.149.14995)).

Design consequence: **one CEO, selected and removable by an elected board, with no entrenchment devices** (no supervoting units, no permanent seats), plus institutionalized shared leadership below the CEO (functional DRIs, documented decision memos, peer verification). We considered and rejected: co-CEOs (Krause), rotating CEO (the only supportive study — Erez et al. 2002 — is a quasi-experiment on student self-managed teams; too thin to bet a company on, though we borrow its *rotating meeting-facilitation* practice at zero risk), and pure consensus (no empirical support at this scale; consensus is preserved only for the reserved supermajority matters in II.7).

## I.6 Boards and investors

At formation the typical VC-backed startup board is entrepreneur-controlled; **independent directors typically join around the second financing round and hold the tie-breaking vote**, mediating founder-VC conflict ([Ewens & Malenko, *Journal of Finance* 2025 / NBER w27769](https://www.nber.org/system/files/working_papers/w27769/w27769.pdf)). Venture boards are not public-company boards — concentrated ownership creates a distinctive "principal problem" of overbearing investors, per the leading theory piece ([Garg 2013, *AMR*](https://journals.aom.org/doi/10.5465/amr.2010.0193)). What investors actually screen on: in a survey of 885 institutional VCs, **95% rate the management team important and 47% rate it the single most important factor** ([Gompers, Gornall, Kaplan & Strebulaev 2020, *JFE*](https://www.nber.org/system/files/working_papers/w22587/w22587.pdf)). The NVCA model term sheet's default board is five seats (investor designee, second investor designee, common designee, CEO, independent) with a standard protective-provisions list, and it contemplates founder re-vesting at financing ([NVCA Model Term Sheet, July 2020, verified mirror](https://raw.githubusercontent.com/kemitchell/nvca-model-legal-documents/main/originals/2021-06-19/NVCA-2020-Term-Sheet-1.pdf) [F-mirror]).

Design consequence: build a small real board now (3 seats, elected, no entrenchment), and design every structure to **collapse cleanly into the NVCA-standard form at the first priced round** rather than fighting it.

## I.7 The professor: differential rates are fine only when they are legible

The pay-dispersion literature initially looks contradictory — dispersion hurt interdependent MLB teams ([Bloom 1999, *AMJ*](https://journals.aom.org/doi/10.5465/256872)) but helped NHL teams when explained by inputs ([Trevor, Reilly & Gerhart 2012, *AMJ*](https://www.semanticscholar.org/paper/82a405461b4a5c578d3b157d375a7c81eddbacc1)). The authoritative review resolves it: **dispersion explained by performance/inputs is neutral-to-positive; *unexplained* dispersion is what damages interdependent teams** ([Shaw 2014, *Annual Review of Organizational Psychology*](https://www.annualreviews.org/content/journals/10.1146/annurev-orgpsych-031413-091253); typology in [Downes & Choi 2014](https://www.sciencedirect.com/science/article/abs/pii/S1053482213000442)).

So the professor's "higher rate" is not inherently toxic — **provided it is an arm's-length market rate anyone can look up, applied through the same formula as everyone else**. What *is* out of line with industry norms is a large fixed grant: the Founder Institute's FAST framework — the de-facto standard for advisor equity — tops out at **1.00% for an "Expert"-level advisor at an idea-stage company** (0.80% startup-stage, 0.60% growth-stage), vesting over two years ([FAST grid, verified FI-content mirror](https://raw.githubusercontent.com/joelmoxley/founder-playbook/master/IV.%20Team%20%2B%20Execution/03%20-%20Team%20Building/05%20-%20Content%20-%20Early%20Stage%20Advisors/md/01%20-%20Founder%20Institute%20-%20Advisor%20Agreements%20.webloc.md) [F-mirror]; template mechanics in the [FAST-style agreement](https://raw.githubusercontent.com/skala-io/advisor-agreement-fast/main/Advisor-Agreement-FAST.md) [F-mirror]). A part-time academic advisor is also legally capped: Yale limits external professional activity to **about one day per seven-day week**, bars salaried outside employment, and treats faculty participation in day-to-day management of an outside entity as **presumptively inappropriate** ([Yale External Professional Activities Guidance](https://provost.yale.edu/policies/external-professional-activities-guidance) [S]); Yale requires COI disclosure and a management plan for faculty equity in research-adjacent startups ([Yale COI Office](https://your.yale.edu/research-support/conflict-interest-office/policies-procedures-guidance) [S]); and Yale owns faculty inventions made with university resources, so IP the professor "contributes" may not be his to give — the company may need a **license from Yale**, not an assignment from him ([Yale Ventures commercialization primer](https://ventures.yale.edu/innovation-and-commercialization-primer) [S]).

Design consequence: II.6 — a FAST-benchmark fixed advisory grant *plus* open access to the same Contribution Ledger as everyone else at his verifiable market rate, conditioned on Yale clearance and an IP-provenance representation.

## I.8 The legal landscape (flags, not advice)

Four findings materially constrain the design; all are developed in II.10–II.12 and the counsel list:

1. **The unpaid employees are a live, compounding liability.** Massachusetts Wage Act damages are **mandatory treble plus attorneys' fees**, even for wages paid late before suit ([Reuter v. City of Methuen, 489 Mass. 465 (2022)](https://law.justia.com/cases/massachusetts/supreme-court/2022/sjc-13121.html); [M.G.L. c. 149 §148](https://malegislature.gov/Laws/GeneralLaws/PartI/TitleXXI/Chapter149/Section148)), with **personal liability** for officers/agents managing the company, and the statute is **non-waivable** — "we all agreed to work for equity" is not a defense, and neither is an equity grant ([c. 149 §148 anti-exemption clause]; [M.G.L. c. 151 §1](https://malegislature.gov/Laws/GeneralLaws/PartI/TitleXXI/Chapter151/Section1) voids sub-minimum-wage agreements; federally, employees "may not volunteer services to for-profit private sector employers," [DOL](https://webapps.dol.gov/elaws/whd/flsa/docs/volunteers.asp), and unpaid equity-only workers fail the $684/week salary-basis test for exemption, [DOL Fact Sheet #17G](https://www.dol.gov/agencies/whd/fact-sheets/17g-overtime-salary)). Founders may qualify as bona fide owners (20%+ equity actively engaged in management — a fact question per [Wiggin & Dana's early-stage wage guide](https://www.wiggin.com/publication/wage-and-hour-fundamentals-a-guide-for-early-stage-companies/) [S]); the ~10 employees almost certainly do not.
2. **Massachusetts close-corporation fiduciary duties reach LLCs.** Members of a closely held MA LLC owe each other "utmost good faith and loyalty" ([Donahue v. Rodd Electrotype, 367 Mass. 578 (1975)](http://masscases.com/cases/sjc/367/367mass578.html), applied to LLCs in [Allison v. Eriksson, 479 Mass. 807 (2018)](https://caselaw.findlaw.com/court/spr-jud-crt-mas-suf/1896955.html)). Any reallocation that disadvantages the inactive founders must run through scrupulously fair process — which our design provides — and [c. 156C §63(b)](https://malegislature.gov/Laws/GeneralLaws/PartI/TitleXXII/Chapter156C/Section63) lets the operating agreement expand or restrict duties, though how far is unsettled.
3. **LLC-phase equity should be profits interests or phantom units, not casual "percent promises."** Profits interests granted for services are non-taxable at grant under [Rev. Proc. 93-27 / 2001-43](https://www.irs.gov/pub/irs-drop/rp-01-43.pdf) if liquidation value at grant is zero; capital interests for services are taxable compensation at FMV — which argues for doing the retroactive settlement **now, while FMV is low**, with 83(b) elections within the hard 30-day window ([Carta 83(b) explainer](https://carta.com/learn/equity/stock-options/taxes/83b-election/) [S]). Unit-holders generally become K-1 partners and lose W-2 status ([IRS practice unit](https://www.irs.gov/pub/fatca/int_practice_units/self-employment-tax-partners.pdf) [S]) — a real cost for the ~10 employees that shapes the instrument choice (II.11).
4. **Investors will expect a Delaware C-corp with a clean, frozen cap table.** VC funds generally can't or won't hold LLC interests; SAFEs presuppose corporations ([YC legal mechanics, F-mirror]; law-firm consensus [S]); QSBS §1202 requires C-corp stock, and after the July 2025 OBBBA the exclusion is tiered **50%/75%/100% at 3/4/5 years** with a **$15M cap** for post-7/4/2025 issuances — and **the QSBS clock starts at conversion, not LLC formation** ([verified §1202 practitioner reference](https://raw.githubusercontent.com/openaccountants/openaccountants/main/packages/us-co/us-section-1202-qsbs.md) [F-mirror]; [Holland & Knight on partnership-to-QSBS conversions](https://www.hklaw.com/en/insights/publications/2025/08/conversion-of-partnership-and-llc-interests-into-qualified) [S]), which pushes toward converting **sooner** once the ledger's heaviest accrual is done.

---

# Part II — The design

## II.0 Architecture at a glance

```
Phase 0 (Days 0–60):    Wage-law remediation begins; Agreement signed;
                        Retroactive Settlement window runs (II.3)
Phase 1 (Quarters 1–N): Contribution Ledger accrues (II.2);
                        Founder Commitment Reserve vests quarterly (II.4);
                        Board of Managers + CEO govern (II.7)
Crystallization (II.9): earlier of qualified financing, sustained breakeven,
                        30 months, or 75% vote →
                        percentages FREEZE → Delaware C-corp conversion →
                        standard cap table + option pool + forward vesting
Phase 2:                Conventional NVCA-compatible company
```

Three instruments make up fully-diluted ownership at Crystallization:

| Bucket | Size | Who |
|---|---|---|
| Contribution Pool | 100% − (B) − (C) — never less than ~72% | Everyone — founders, employees, and (optionally) the professor, on **identical terms** |
| (B) Founder Commitment Reserve | ≤ 5.0 pp per founder; ≤ 25 pp total; **unearned portions cancel into the Contribution Pool** | Founders only (fixed requirement #1) |
| (C) Advisor Grant | 1.0 pp fixed | The professor (II.6) |

## II.1 First principles (derived from Part I)

1. **Pay for verified contribution at market rates, not for titles or history** (I.1, I.3).
2. **Procedural transparency is a feature requirement, not a nicety** — published formula, published rates, monthly statements, appeal rights (I.2, I.7).
3. **Time-bound the dynamism.** The ledger must bake into a boring cap table before investors see it (I.4, I.6, I.8-4).
4. **No entrenchment anywhere.** Every role is elected or appointed, every role is losable, including CEO and including founder status benefits (I.5).
5. **Legality first.** No equity mechanism may be presented as a substitute for wages (I.8-1).

## II.2 The Contribution Ledger

The heart of the system. It is deliberately a bounded adaptation of Slicing Pie (I.4): we keep the well-formula and multipliers, and add the things practitioners fault it for lacking — a hard freeze date, evidence standards, hour caps, and a committee whose only power is verification, not discretion.

### II.2.1 The formula

Every Participant `p` (founder, employee, or enrolled advisor — same rules, per fixed requirement #2) accrues **Contribution Points (CP)** monthly:

```
CP(p, month) =  VerifiedHours(p, m) × Rate(p) × 2.0          — unpaid labor
             +  (Rate(p) − PaidRate(p)) × VerifiedHours × 2.0 — partially paid labor gap
             +  CashIn(p, m) × 4.0                            — cash contributed
             +  ApprovedUnreimbursedExpenses(p, m) × 4.0
             +  FMV(pre-approved equipment or IP) × 2.0
Share(p) at any time = ΣCP(p) / ΣCP(all participants)
```

Multipliers follow the Slicing Pie norm (non-cash ×2, cash ×4), which functions simultaneously as risk compensation and as the basis of fair buyout pricing at separation ([Slicing Pie multipliers](https://slicingpie.com/the-magic-of-mutipliers/) [S], corroborated ×2 [F-mirror]). Once a participant is paid full market cash compensation, their labor accrues zero CP — the system self-extinguishes as the company becomes able to pay, which is exactly the property that makes it investor-explainable.

### II.2.2 The rate table (Schedule A of the operating agreement)

- `Rate(p)` = the **50th percentile Boston-market total cash compensation** for `p`'s role and level, from a named benchmark source [**bracketed choice for founders: Carta Total Comp | Pave | Radford; public fallback: BLS OEWS Boston–Cambridge–Nashua**, e.g. the May 2023 metro table at [bls.gov/oes](https://www.bls.gov/oes/2023/may/oes_71650.htm)], divided by 2,080 hours.
- Levels are assigned by the Board on hiring/role change using the benchmark source's published level definitions; level assignments and the whole rate table are **visible to every participant** (I.2).
- Rates reset each January 1 from the then-current benchmark. No individually negotiated rates — *the benchmark is the negotiation*. This is what makes the professor's premium legible (II.6) and what makes founders and employees genuinely identical (fixed requirement #2): a founder doing senior-engineer work and an employee doing senior-engineer work earn CP at the same rate.
- Illustrative only (must be replaced with benchmark pulls at adoption): junior SWE ≈ $52/hr, mid ≈ $72/hr, senior ≈ $87/hr, engineering manager ≈ $105/hr, ML advisory (professor-grade) ≈ $350/hr.

**Role-spanning work (coding vs. management vs. vision):** hours are logged against the role actually performed that day, at that role's rate. "Vision/strategy" work earns CP only through artifacts — decision memos, roadmap documents, fundraising materials, customer-discovery writeups — logged as hours in the strategy/management role. There is deliberately **no "idea premium" and no impact multiplier**: raw ideas carry a 0× multiplier in canonical Slicing Pie, the founder literature finds idea premia are small (~10–15pp) and contested [S], and any subjective impact factor would reopen exactly the politics the objective system exists to close. Skill differences are already priced through the rate table; output differences are handled through acceptance (II.2.3), role/level assignment, and — for persistent underperformance — role change or termination (II.8), not through score-fiddling.

### II.2.3 Verification (the anti-gaming layer)

Evidence, not opinion, per I.3:

1. **Logging.** Hours logged weekly in a shared system; every entry must reference at least one work item (commit/PR, design doc, meeting with agenda+notes, support ticket, recruiting pipeline entry, decision memo). Unreferenced entries are ineligible.
2. **Caps.** Creditable hours capped at **60/week and 12/day** (guards against log-inflation races; generous enough for real crunch).
3. **Monthly attestation.** Each participant signs their log; the responsible functional lead counter-signs that the referenced work items exist and were accepted.
4. **The Contribution Committee** (3 members, elected annually by all participants, **at least one non-founder**; no member reviews their own entries) audits a random ≥20% sample monthly and any challenged entry. Its only powers are to **verify or disallow against the written evidence standard** (Schedule B) — it cannot scale, bonus, or discount. Knowingly false entries: the entry is voided and that month's CP for the filer is forfeited (first offense); repeat = Cause (II.8).
5. **Transparency.** Every participant receives a monthly statement: their CP, total CP, and their current percentage. (Peer visibility of totals is itself a loafing deterrent — I.3.)
6. **Appeals** go up the dispute ladder (II.12), with the arbitrator confined to applying Schedule B.

## II.3 The Retroactive Settlement (the unpaid Year 0)

The past year is scored **through the identical formula**, reconstructed under evidence rules, and settled once, permanently:

1. **Window.** 60 days from signing. Each person (all five founders, all ~10 employees, the professor if he elects the Ledger) files a monthly reconstruction of hours, role, cash, and expenses.
2. **Evidence tiers** (Schedule B): **Tier A** — directly documented (git/PR history, authored docs, calendar-verifiable meetings, bank records for cash): credited 100%. **Tier B** — estimated but corroborated in writing by two other participants: credited 85%. **Tier C** — uncorroborated self-report: credited 50%, and capped at 15 hours/week. Cash and expenses require bank/receipt records — no records, no credit (the ×4 multiplier is too gameable otherwise).
3. **Review.** The Contribution Committee, assisted by a **neutral outside facilitator** [bracketed: a mediator or fractional-CFO firm], scores all filings under the same rubric in one pass, then publishes the full retroactive ledger to all participants simultaneously. Objections go to the facilitator, then the dispute ladder.
4. **Result.** Year-0 CP goes into the same well as future CP. A founder who carried the company for a year keeps every point of that; a founder who stopped showing up in month 3 keeps exactly what three months of verified work earned; an employee who out-contributed a founder holds more CP than that founder, by construction — which is precisely what the founders' own informal agreement promised.
5. **Legal character.** The settlement is a compensatory equity grant for past services — taxable at today's (low) FMV, which is why it happens now, with valuations and 83(b)s per counsel ([IRC §83 mechanics](https://www.thetaxadviser.com/issues/2025/mar/the-complex-simplicity-of-partnership-interests-exchanged-for-services/) [S]) — and it is **expressly not a payment of, or waiver of, wages** (I.8-1; II.10).

## II.4 The Founder Commitment Reserve (fixed requirement #1, made real)

Each founder may earn up to **5.0 percentage points** of the fully-diluted Crystallization cap table, on top of whatever their CP earns them:

- **Schedule:** 16 equal quarterly tranches of 0.3125 pp over 4 years from the Effective Date, with a **4-quarter cliff** (quarters 1–4 credit only if the founder is in Active Status at the end of Q4). Mirrors the market-standard 4-year/1-year-cliff shape ([NVCA term sheet, F-mirror]; [Fenwick guide, F-mirror]; [YC/Seibel on why cliffs exist](https://www.ycombinator.com/library/LP-co-founder-equity-mistakes-to-avoid) [S]).
- **Active Founder Status** for a quarter = **≥ [260] Ledger-verified hours in that quarter** (≈20 hrs/week average), or holding an officer or Board seat in good standing with ≥ [195] verified hours. The test is mechanical and runs off the same verified ledger — no committee judgment call.
- **Use it or lose it:** a missed quarter's tranche is **permanently cancelled and its percentage points flow back into the Contribution Pool**, where everyone's CP — founder and employee alike — absorbs them pro rata. One protected quarter per 4-year period for documented medical/family leave [bracketed] pauses (not forfeits) the schedule; counsel should conform this to leave-law obligations.
- **Not retroactive.** Year 0 earns CP only. The reserve rewards *forward* founder commitment; the past is already fully priced by II.3. (This is also the cleanest reading of the founders' own requirement that the reserve "must be earned.")
- **Why a founder-only layer at all, given identical-terms?** It is a fixed requirement; our job was to make it earned and bounded. At ≤25pp maximum — achieved only if all five founders sustain four full years of active work — it is comparable to the differential a conventional founders/employees split would produce anyway, while being the only non-identical element in the system, fully visible, and self-liquidating when unearned. Expect most of it *not* to be earned: on the base rates in the literature, half of founder-CEOs are gone by year three ([Wasserman 2008](https://hbr.org/2008/02/the-founders-dilemma)).

## II.5 Inactive founders — every dimension

The design never needs to litigate "who is a real founder." It prices them:

| Dimension | Outcome for an inactive founder | Mechanism |
|---|---|---|
| Past contribution | **Kept, in full, at identical rates** — verified Year-0 work becomes CP like anyone's | II.3 |
| Future equity | ~Zero accrual while inactive | II.2 (no hours → no CP) |
| Reserved 5% | Forfeits quarter-by-quarter into everyone's pool | II.4 |
| Governance | No automatic seat or veto; board seats are elected annually; voting power = current Ledger share, which decays *relatively* as others keep contributing | II.7 |
| Title | "Founder" as historical designation persists; carries no rights | OA Art. II |
| Exit | May resign as Good Leaver (keeps CP, subject to repurchase option at fair value); if they simply linger inactive, nothing accrues and nothing needs to be done | II.8 |
| Dignity/process | Same statements, same appeal rights, same buyout formula as everyone — the fairness-perception literature says process is what prevents this from turning litigious | I.2; counsel note on Donahue/Allison in II.13 |

No punitive clawback of genuinely earned past contribution is proposed: it is unnecessary (relative decay does the work), it would poison perceived justice (I.2), and it would maximize fiduciary-duty litigation risk in Massachusetts (I.8-2).

## II.6 The professor

**Offer (both components together):**

1. **Fixed Advisory Grant: 1.0 pp** (fully-diluted at Crystallization) — the top of the FAST grid for an Expert-tier advisor at an idea/startup-stage company [F-mirror] — vesting monthly over 24 months with a [3-month] cliff, under a written advisor agreement with 10-day no-fault termination and auto-termination after 6 months of inactivity (FAST-standard mechanics [F-mirror]). This honors "a decent share" at the ceiling of documented market practice, and we would show him the grid.
2. **Open Ledger enrollment on identical terms:** for defined engagements pre-approved by the Board (annual cap [300] hours), he accrues CP exactly like everyone else at `Rate = benchmark ML-advisory market rate` [illustrative ≈ $350/hr — several multiples of a senior engineer's rate]. **His "higher rate" is thus honored precisely to the extent the market documents it** — explained dispersion, which the evidence says teams tolerate; not an unexplained privilege, which they don't (I.7).
3. **Conditions precedent (counsel-drafted):** (a) written confirmation of Yale COI disclosure/approval and consistency with the one-day-per-week and no-management-role limits [S]; (b) IP-provenance representation, and where any contribution draws on Yale resources or falls under the Yale Patent Policy, a **license from Yale** rather than a personal assignment [S]; (c) no board seat — he chairs a non-governing Scientific Advisory Board; (d) standard confidentiality/assignment agreement for non-Yale IP.
4. **Expectation management, scripted with data:** the FAST grid caps famous-advisor norms near 1%; more than that is earned on the same ledger as everyone else, at a rate that already prices his eminence. If "decent share" meant multiple points for part-time association, the honest answer is that no documented market practice supports it, and unexplained dispersion is the one variety the fairness literature flags as corrosive (I.7).

## II.7 Governance

**Form: manager-managed LLC** (converting later to a standard corporate board) with a **3-seat Board of Managers**:

| Seat | Held by | How |
|---|---|---|
| 1 | CEO (ex officio) | Appointed & removable by Board majority; confirmed annually |
| 2 | Elected Manager | Annual election, all participants voting current Ledger shares |
| 3 | Elected Manager | Annual election; **must be a non-founder participant** [bracketed — alternative: second at-large seat] |

- **Why this shape:** a real monitoring body with an odd number and no permanent chairs implements "involvement without entrenchment" (I.5); the non-founder seat operationalizes the identical-terms culture and the peer-evaluation evidence (I.3) — and it **sunsets at the first qualified financing**, when the board reconstitutes on the NVCA pattern (investor designee(s), common designee, CEO, independent) so that investors meet a structure they recognize (I.6).
- **CEO.** One person, full-time, selected by the Board through a written process (criteria: forward commitment, execution record on the Ledger itself, fundraising capability). Explicitly **not** co-CEOs (Krause inverted-U, I.5), **not** rotating (evidence too thin, I.5), **not** entitled to the seat by founder status (Wasserman control-discount, I.5). The CEO holds no supervoting rights and can be removed by the two elected managers acting together — the system's answer to "what if the leader is the problem."
- **Shared leadership, where the evidence supports it:** functional DRIs with published ownership areas; significant decisions recorded in short decision memos (reversible decisions: DRI decides after consultation; hard-to-reverse: Board); rotating facilitation of leadership meetings (harmless, mildly evidence-backed — Erez et al.); quarterly all-hands review of company metrics and the Ledger.
- **Decision-rights matrix (Schedule C):**

| Tier | Examples | Decided by |
|---|---|---|
| 1 — Ordinary course | Product, hiring within budget, spend < $[25k] | CEO / DRIs |
| 2 — Significant | Budget adoption, officer hire/fire, debt > $[50k], IP licensing, litigation, rate-table annual reset | Board majority |
| 3 — Fundamental | Amend OA; admit non-Ledger members; sale/merger/dissolution; C-corp conversion terms; **any change to the Ledger formula, multipliers, or Schedule B**; related-party transactions | Members ≥ 66⅔% of voting units; Ledger-formula changes additionally require majority of **non-founder** participants' units [bracketed] — the promise of identical terms should not be amendable by founders alone |

- **Voting units.** One CP = one vote, per the most recent quarterly statement. Power tracks contribution continuously — the governance analog of the equity principle, and the reason inactive founders fade from control without anyone firing them.

## II.8 Departures (leaver framework, Schedule D)

Adapted from Slicing Pie's recovery framework [S] with Massachusetts-fiduciary softening:

| Event | Non-cash CP (time) | Cash CP (×4) | Founder Reserve |
|---|---|---|---|
| Resignation **without** Good Reason, or termination **for Cause** | Company **option to repurchase at 1× unmultiplied imputed value** (hours × rate, multiplier stripped), payable over [36] months | Treated as an interest-free loan; repaid when [cash permits / at Crystallization] | Unvested tranches cancel |
| Termination **without** Cause, resignation **for** Good Reason, death, disability | **Kept**; converts at Crystallization with everyone else | Kept at full ×4 | Vested tranches kept; unvested cancel |

- "Cause" and "Good Reason" get tight, conventional definitions from counsel; the Ledger's own records (verified fraud, sustained non-performance against accepted work items) feed the Cause determination.
- We deliberately convert Moyer's outright forfeiture into a **priced repurchase option**: it produces the same dead-equity hygiene investors need ([dead equity as a diligence red flag — practitioner compilation, F-mirror]), while a formula price paid over time is far more defensible against an "utmost good faith and loyalty" challenge than confiscation (I.8-2 — counsel to pressure-test).
- Post-Crystallization, all crystallized holdings are earned/vested; **forward** grants (refresh options from the pool) carry standard 4/1 vesting, and founders should expect investors to ask for partial re-vesting at the round as the NVCA term sheet contemplates [F-mirror].

## II.9 Crystallization and conversion

**Trigger — earliest of:** (i) a qualified priced financing ≥ $[1,000,000]; (ii) two consecutive cash-flow-positive quarters *(the Slicing Pie "bake" events — financing or breakeven — made contractual)*; (iii) **[30] months** from the Effective Date *(hard backstop so the dynamism cannot run forever — the single biggest practitioner criticism of open-ended dynamic splits [S][F-mirror])*; (iv) 75% member vote.

**At Crystallization:**
1. The Ledger runs one final month and freezes. Final shares = CP shares × Contribution Pool size; plus earned Founder Reserve; plus vested Advisor Grant.
2. The company **converts to a Delaware C-corporation** (Massachusetts side via the c. 156D Part 9 conversion provisions or merger into a new Delaware corporation — pathway and member-vote threshold for counsel, [c. 156D §9.50](https://malegislature.gov/Laws/GeneralLaws/PartI/TitleXXII/Chapter156D/Section9.50) [S]; Delaware side [8 Del. C. §265](https://law.justia.com/codes/delaware/title-8/chapter-1/subchapter-ix/section-265) [S]; tax-free under §351 in the standard forms, with the §357(c)/negative-capital-account traps flagged [S]).
3. Frozen percentages become **one class of common stock** (plus a new **[12–15]% option pool** for future work, within the 10–20% norm [F-mirror ×3]); 83(b)s filed where applicable within 30 days [S]; QSBS clock starts at conversion under the post-OBBBA tiered rules [F-mirror] — counsel to weigh conversion timing against the FMV-basis step-up trade-off ([Holland & Knight](https://www.hklaw.com/en/insights/publications/2025/08/conversion-of-partnership-and-llc-interests-into-qualified) [S]).
4. Governance reconstitutes on the NVCA-standard pattern (I.6). SAFEs, if any are ever contemplated, are signed **only after** conversion [F-mirror; S].

**If a term sheet arrives before the backstop date:** Crystallization is defined to complete *immediately prior to* the financing, so no investor ever holds a moving cap table. What investors see at diligence: one class, no dead equity, standard vesting, wage-clean payroll, IP assigned, 83(b)s on file — each item on that list is a named diligence red flag we designed out (I.6, I.8).

## II.10 Wage-law remediation (urgent; runs before and parallel to everything)

Not optional, and not curable by this equity plan (the statutes void waivers — I.8-1):

1. **Immediately** (week 1): counsel engaged; stop accruing new violations — either start compliant payroll (≥ MA minimum wage, weekly/biweekly, for all non-owner workers), or formally suspend non-owner work until payroll is funded, or (counsel-gated) restructure genuine partners as bona fide members with real ownership and management roles.
2. **Quantify** the ~10 employees' accrued exposure (3-year lookback; treble; personal liability of managing officers) and remediate through a counsel-designed back-pay/settlement program. Budget for this **before** any fundraise — it is a diligence red flag of the first order.
3. The Ledger is documented everywhere as an **ownership/upside program that supplements lawful wages** — never as wage replacement. Once payroll starts, CP accrues only on the gap between market rate and cash actually paid (II.2.1), which is the lawful and canonical form of "sweat equity."

## II.11 Instrument choice at the LLC stage (recommended default; counsel decides)

- **Founders/members:** Year-0 settlement as re-set capital-account percentages now (taxable at today's low FMV — get a valuation), ongoing accrual as quarterly **profits-interest** grants with $0 liquidation threshold at grant and protective 83(b)s ([Rev. Proc. 93-27/2001-43](https://www.irs.gov/pub/irs-drop/rp-01-43.pdf); [profits-interest FAQ](https://rsmus.com/insights/services/business-tax/frequently-asked-questions-about-profits-interests.html) [S]).
- **Employees:** because unit-holding employees become K-1 partners (lose W-2 status, self-employment tax) [S], hold their Ledger balances as **contractual phantom units** that convert to real stock at Crystallization, *or* use a tiered holdco, *or* accelerate the C-corp conversion — a three-way structural choice for counsel with the trade-offs written out in the counsel list (II.13). The *economics* — the CP formula and shares — are identical under all three; only the wrapper differs. **[Open decision point.]**

## II.12 Dispute resolution

1. **Ladder:** direct negotiation (15 days) → mediation, JAMS/AAA Boston (30 days) → **binding arbitration** (AAA Commercial, single arbitrator, Boston; FAA expressly governing; clause binds the company and every member/participant; carve-outs for injunctive IP relief and non-waivable statutory claims) — drafting points per the ABA guide ([Gattuso, *Business Law Today*](https://apps.americanbar.org/buslaw/blt/2009-03-04/gattuso.shtml) [S]).
2. **Ledger appeals** are confined to applying Schedule B (the arbitrator verifies evidence, never re-weights the formula).
3. **Deadlock.** The 3-seat board plus CP-weighted member voting makes true deadlock structurally rare (no 50/50 anywhere). If a Tier-3 matter fails twice over two consecutive quarters with the company being damaged, any ≥10% holder may trigger **appraised fair-value buy-sell**: an independent appraiser [bracketed: baseball-style dual appraisal] sets fair value; the continuing group buys out the triggering/blocking minority over [24–36] months. We specifically **rejected shotgun clauses**: they auction the company to the wealthier party rather than the righter one (practitioner critique [F-mirror]), and in Massachusetts a shotgun deployed against a minority invites an utmost-good-faith challenge ([shotgun enforceability discussions](https://www.pecklaw.com/business-owner-rights/shotgun-buy-sell-option-agreements/) [S]; I.8-2).
4. The drafted alternative to all of this is the statutory default nobody wants: judicial dissolution when the business is "not reasonably practicable" to carry on ([M.G.L. c. 156C §44](https://malegislature.gov/Laws/GeneralLaws/PartI/TitleXXII/Chapter156c/Section44)) — Massachusetts gives members no default buyout right, so the contract has to.

## II.13 Consolidated counsel list (flag, don't resolve — fixed requirement #4)

1. Wage Act remediation design and quantification; who among the five founders is a bona fide exempt owner (20%+/management test).
2. How far c. 156C §63(b) permits tailoring Donahue/Allison duties; fairness-process papering for the Retroactive Settlement and the leaver repurchase (the two provisions most exposed to a freeze-out claim by an inactive founder).
3. Instrument wrapper for employees (phantom vs. profits interests vs. tiered holdco vs. early conversion) and 409A/constructive-receipt review of any legacy "we'll pay you later" promises.
4. Valuation for the Retroactive Settlement; 83(b) logistics; §351/§357(c) conversion analysis; QSBS timing (post-OBBBA tiered clock vs. FMV-basis step-up).
5. Conversion pathway (c. 156D Part 9 vs. merger) and required member-vote threshold.
6. Yale: license vs. assignment for any professor IP; COI plan; conforming his role to the one-day/no-management limits; conditioning the grant on university clearance.
7. Enforceability review of: CP-weighted voting in an LLC, the repurchase-option leaver terms, the arbitration clause (FAA/derivative claims), and the appraisal buy-sell.
8. Massachusetts QSBS conformity check at conversion [F-mirror flags state conformity variance].

---

# Part III — Worked example, limitations, and what would change our mind

## III.1 Worked example (illustrative numbers, Year-0 only, showing the spreadsheet is real)

Assumptions: rates from II.2.2's illustrative table; at Crystallization the earned Founder Reserve is F1 5.0, F2 5.0, F3 1.25, F4 2.5, F5 0.0 (=13.75pp), Advisor Grant 1.0pp ⇒ Contribution Pool = 85.25pp.

| Person | Verified profile (Year 0) | CP (thousands) | % of CP | Pool % | + Reserve | **Total** |
|---|---|---:|---:|---:|---:|---:|
| F1 (EM/CEO-track) | 2,750h × $105 × 2 + $20k cash × 4 | 657.5 | 21.9% | 18.7% | 5.00 | **23.7%** |
| F2 (senior SWE) | 2,500h × $87 × 2 | 435.0 | 14.5% | 12.4% | 5.00 | **17.4%** |
| F3 (senior, active 6 mo) | 1,200h × $87 × 2 | 208.8 | 7.0% | 5.9% | 1.25 | **7.2%** |
| F4 (mid, ~20h/wk) | 1,000h × $72 × 2 | 144.0 | 4.8% | 4.1% | 2.50 | **6.6%** |
| F5 (inactive from ~mo 2) | 200h × $72 × 2 | 28.8 | 1.0% | 0.8% | 0.00 | **0.8%** |
| E1 (senior, 9 mo) | 1,700h × $87 × 2 | 295.8 | 9.9% | 8.4% | — | **8.4%** |
| E2 (mid, 12 mo) | 2,000h × $72 × 2 | 288.0 | 9.6% | 8.2% | — | **8.2%** |
| E3 (junior, 6 mo) | 1,000h × $52 × 2 | 104.0 | 3.5% | 3.0% | — | **3.0%** |
| E4–E10 (aggregate) | various | 840.0 | 28.0% | 23.9% | — | **23.9%** |
| Professor | Fixed advisory grant | — | — | — | — | **1.0%** |
| | | **3,001.9** | 100% | 85.25 | 13.75 | **100%** |

Note what the system does without anyone deciding anything: E1 and E2 each hold more than founders F3, F4, and F5 — because they contributed more, which is the founders' own stated intent; F5, the inactive founder, lands at 0.8%, earned honestly and kept honestly; and every number above is an auditable formula over verifiable inputs.

## III.2 Honest limitations

- **No direct causal evidence exists for the full system.** Dynamic contribution-tracked equity has never been RCT'd; our support is a lattice of causal lab evidence (Kagan; Karau & Williams), correlational field studies (Hellmann & Wasserman; Mueller & Hennicke), and practitioner convention (Slicing Pie; FAST; NVCA). We rate the *directional* case strong and the *specific parameters* (2×/4×, 60h caps, 30-month backstop) as convention-plus-judgment, clearly labeled.
- **The governance recommendation runs against a live academic disagreement.** Shared-leadership meta-analyses would tolerate a flatter design than we chose; we weighted the co-CEO inverted-U result, investor-preference evidence, and the founder-control discount more heavily. Reasonable people could design a flatter company; we think the evidence, on net, does not favor it at fundraising time.
- **Measurement bias is real.** Hour-based systems undercount taste, judgment, and leverage (the 10× architecture decision logs the same hours as routine work). Our mitigations — role-based rates, artifact requirements, acceptance standards — bound but do not eliminate this. The 30-month crystallization also bounds it: after the bake, conventional performance-based refresh grants take over.
- **Verification asymmetry.** Because of the sandbox egress policy, a minority of load-bearing sources were verified at [S] (live search-index confirmation) rather than full-text fetch; all are flagged per-source in `plan-9-references.md`, and none of the design's central choices rests on a single [S] source.

## III.3 What would change our mind

If the founders' benchmark pull showed the professor's true market advisory rate near an engineer's, component 2 of II.6 loses its premium automatically — the design self-corrects. If counsel concludes MA fiduciary doctrine cannot tolerate the leaver repurchase even at formula price, the fallback is Moyer-canonical retention of slices with loss of multipliers only. If all five founders re-engage fully, the Reserve simply pays out as designed and the system converges toward the near-equal outcome YC recommends for committed teams — the design does not presume any founder stays inactive; it prices whatever they do.
