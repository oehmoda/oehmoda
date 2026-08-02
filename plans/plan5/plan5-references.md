# plan5 — Annotated Bibliography

Every source cited in `plan5-design.md`, `plan5-one-pager.md`, or
`plan5-operating-agreement.md` appears here with: full citation, URL, what claim(s)
in our design it supports, and an honest evidence-strength rating on two axes —
**publication type** (peer-reviewed › university press › statute/case/regulator ›
major-firm or data-provider explainer › practitioner framework › anecdote) and
**inference type** (causal › quasi-causal › correlational › descriptive › pure theory).

## ⚠ Verification disclosure (read first)

Our research environment's network egress policy **blocked all direct page fetches**
(HTTP 403 policy denial at the gateway on every host tested, including a control
test of example.com and irs.gov/malegislature.gov/yale.edu). Server-side web search
**did** work and returns live snippets from the actual publisher pages. Accordingly:

- **No source below is cited from memory alone.** Every URL was confirmed to exist,
  with matching title/author/journal/section content, via live web-search results
  retrieved 2026-08-01 (marked **SEARCH-CONFIRMED**).
- **No source is marked "fetch-verified,"** because fetch verification was
  technically impossible here. None showed any sign of being dead or wrong in
  search results, but counsel and the founders should pull each URL directly
  before relying on it.
- Where a specific statistic could **not** be surfaced in accessible text, we say
  so in the entry and did not fill the gap from memory. These gaps are repeated in
  the entries below (e.g., overall corrected ρ in two meta-analyses).

We also confirm: **we did not read, check out, diff, or browse any other team's
branch or files at any point.** Our branch began as an empty tree and contains only
plan5 files.

---

## Part A — Peer-reviewed and scholarly sources

### A1. Hellmann & Wasserman (2017), "The First Deal: The Division of Founder Equity in New Ventures," *Management Science* 63(8): 2647–2666
- URLs: https://pubsonline.informs.org/doi/10.1287/mnsc.2016.2474 · NBER WP 16922: https://www.nber.org/papers/w16922 · digest: https://www.nber.org/digest/aug11/division-founder-equity-new-ventures — SEARCH-CONFIRMED.
- Sample: 1,476 founders in 511 US/Canadian tech & life-science ventures.
- Findings we rely on: **32% of teams split exactly equally; 42% settled the split in a day or less ("quick handshake"); quick-and-equal splitters obtain lower first-round pre-money valuations (~10% of equity ≈ ~$450K NPV at stake) and are less likely to raise outside financing**; heterogeneity in idea generation, prior founding experience, and capital reduces equal-splitting.
- Supports: our rejection of a static renegotiated split in favor of a deliberate, formula-driven process (design §2.1); the claim that the *process* of splitting is itself an investor signal.
- Strength: **peer-reviewed, top journal; correlational — the authors explicitly interpret the valuation penalty as selection (teams that avoid the hard conversation), not causation.** We use it accordingly: as evidence that avoiding structured negotiation is a bad sign, not that unequal splits cause higher valuations.

### A2. Breugst, Patzelt & Rathgeber (2015), "How should we divide the pie? Equity distribution and its impact on entrepreneurial teams," *Journal of Business Venturing* 30(1): 66–94
- URL: https://www.sciencedirect.com/science/article/abs/pii/S0883902614000676 — SEARCH-CONFIRMED (vol/pages via https://ideas.repec.org/a/eee/jbvent/v30y2015i1p66-94.html).
- Findings we rely on: in an 8-team, 6-month multiple-case study, **perceived justice of the equity split — not its equality — drives positive vs. negative team-interaction spirals**; even high-justice teams drifted negative under external threat.
- Supports: design §2.2 (why the split must be *procedurally* fair and transparent — published ledger, appeal rights), and §5 (why inactive founders keep what they earned: forfeiting delivered value reads as injustice and poisons the team).
- Strength: **peer-reviewed, top entrepreneurship journal; qualitative, N=8, theory-building — mechanism evidence only, no effect sizes.** We use it for mechanism, paired with A1/A10 for breadth.

### A3. Wasserman (2008), "The Founder's Dilemma," *Harvard Business Review* 86(2); and Wasserman (2012), *The Founder's Dilemmas*, Princeton University Press
- URLs: https://hbr.org/2008/02/the-founders-dilemma · https://press.princeton.edu/books/paperback/9780691158303/the-founders-dilemmas — SEARCH-CONFIRMED.
- Findings we rely on: from 212 startups — **by year 3, 50% of founders are no longer CEO; fewer than 25% lead their IPO; 4 of 5 departing founder-CEOs are forced out**; the rich-vs-king tradeoff (control-keeping founders build less valuable companies). From the book's ~10,000-founder dataset: **73% of teams split equity within a month of founding; ~half of founding teams include no dynamic elements (vesting/buyout) at all**; teams that quick-split equally are ~3× more likely to be unhappy with the split (book-derived multiplier via HBS coverage, https://www.hbs.edu/news/Pages/item.aspx?num=1292 — treat as descriptive).
- Supports: design §3.2 (CEO as a revocable, term-limited office, decoupled from equity — because founder-CEO replacement is the base-rate outcome and fighting it destroys value); §2.1 (dynamic elements are the exception in practice, which is why investors notice them).
- Strength: **HBR = practitioner outlet (not peer-reviewed) summarizing the author's peer-reviewed stream (A7); book = university press. Descriptive/correlational.**

### A4. Shared-leadership meta-analyses (three, with a flagged disagreement)
- **D'Innocenzo, Mathieu & Kukenberger (2016), *J. of Management* 42(7): 1964–1991** — https://journals.sagepub.com/doi/10.1177/0149206314525205 — SEARCH-CONFIRMED. 50 effect sizes, N=3,198 teams; positive overall shared-leadership→performance relation; aggregation-based subset weighted effect **.15 (95% CI [.08, .22])**, network-based measures larger; **task complexity moderated the relation negatively**. (Overall corrected ρ across all 50 effects: not surfaced in accessible text — not reported.)
- **Nicolaides et al. (2014), *The Leadership Quarterly* 25(5): 923–942** — https://www.sciencedirect.com/science/article/abs/pii/S1048984314000691 — SEARCH-CONFIRMED. Shared leadership predicts team performance **over and above vertical leadership** (complement, not substitute); mediated by team confidence; stronger under higher task interdependence. (Overall ρ: not surfaced — not reported.)
- **Wang, Waldman & Zhang (2014), *J. Applied Psychology* 99(2): 181–198** — https://pubmed.ncbi.nlm.nih.gov/24188392/ — SEARCH-CONFIRMED. 42 samples; **overall ρ ≈ .34 (shared traditional leadership ρ = .18; new-genre ρ = .34; cumulative ρ = .35)**; stronger for attitudes/processes than performance; **stronger when work is more complex**.
- **Disagreement flagged:** Wang et al. find shared-leadership effects *stronger* under complexity; D'Innocenzo et al. find them *weaker*; Nicolaides et al. emphasize interdependence instead. All three agree the average effect is positive (ρ ≈ .15–.35 depending on measurement). Supports design §3.1's hybrid: real distributed decision rights (DRIs) **plus** a single accountable vertical leader — the only structure consistent with all three.
- Strength: **peer-reviewed meta-analyses; correlational inputs; mostly non-founder teams (external-validity limit stated in design §3.1).**

### A5. Co-CEO evidence (two sources, opposite postures, asymmetric rigor)
- **Krause, Priem & Love (2015), "Who's in charge here? Co-CEOs, power gaps, and firm performance," *Strategic Management Journal* 36(13): 2099–2110** — https://sms.onlinelibrary.wiley.com/doi/abs/10.1002/smj.2325 — SEARCH-CONFIRMED. 71 public-company co-CEO pairs; **performance rises with the power gap between co-CEOs (inverted-U at extreme gaps)**; authors read it as supporting unity of command.
- **Feigen, Jenkins & Warendh (2022), "Is It Time to Consider Co-CEOs?," *HBR* 100(4)** — https://hbr.org/2022/07/is-it-time-to-consider-co-ceos — SEARCH-CONFIRMED. 87 public co-CEO companies; **9.5% avg annual shareholder return vs. 6.9% comparison; ~60% outperformed** — but non-peer-reviewed, no selection controls (co-CEO arrangements persist only where they work).
- Supports: design §3.1's rejection of co-CEO/rotating-CEO structures for this company; we weight the peer-reviewed source and treat the HBR result as upper-bound anecdata.
- Strength: **SMJ: peer-reviewed, correlational, small N. HBR: practitioner, descriptive, high selection-bias risk.**

### A6. Holmström (1982), "Moral Hazard in Teams," *Bell Journal of Economics* 13(2): 324–340
- URL (full-text mirror): https://people.duke.edu/~qc2/BA532/1982%20Rand%20Holmstrom%20team.pdf — SEARCH-CONFIRMED.
- Findings we rely on: the **1/N free-rider theorem** (each member bears full effort cost for 1/N of marginal output → effort undersupplied); impossibility of budget-balanced, efficient sharing; efficiency restored by an outside residual claimant.
- Supports: design §2.1 (why unconditional equal shares in a 15-person shop undermine effort; why pay-for-delivered-contribution dominates) and §4 (why outside investors/a board are efficiency-enhancing, not merely dilution).
- Strength: **foundational peer-reviewed theory (Nobel-cited); no empirics — used as mechanism only.**

### A7. Wasserman (2003), "Founder-CEO Succession and the Paradox of Entrepreneurial Success," *Organization Science* 14(2): 149–172
- URLs: https://pubsonline.informs.org/doi/10.1287/orsc.14.2.149.14995 · author PDF: https://www.noamwasserman.com/nwasserman/Founder-CEO_Succession-OrgScience.pdf — SEARCH-CONFIRMED.
- Findings: in 202 Internet firms, **completing product development and raising outside financing sharply increase the probability the founder-CEO is replaced**; succession is usually investor-initiated; middling performers keep the seat longest.
- Supports: design §3.2 — building CEO turnover into the constitution (12-month renewable terms) instead of letting investors force it traumatically later.
- Strength: **peer-reviewed; correlational event-history; single industry/era; 20% response rate.**

### A8. Garg (2013), "Venture Boards: Distinctive Monitoring and Implications for Firm Performance," *Academy of Management Review* 38(1): 90–108
- URL: https://journals.aom.org/doi/10.5465/amr.2010.0193 — SEARCH-CONFIRMED (note: DOI is amr.**2010**.0193; a commonly mistyped variant exists). Companions: Garg & Eisenhardt (2017) AMJ, https://journals.aom.org/doi/10.5465/amj.2014.0599; Garg (2017) SEJ, https://sms.onlinelibrary.wiley.com/doi/10.1002/sej.1258 — SEARCH-CONFIRMED.
- Findings: venture boards are small, milestone-focused, and combine monitoring with resource provision; VC directors' fund incentives can diverge from common holders.
- Supports: design §3.3 (a small working board now, structured to graft cleanly onto a standard VC board later).
- Strength: **peer-reviewed premier theory journal; propositions only, no empirical test.**

### A9. Dynamic vs. static founder contracting
- **Hellmann & Thiele (2015), "Contracting among Founders," *J. of Law, Economics, & Organization* 31(3): 629–661** — https://academic.oup.com/jleo/article-abstract/31/3/629/808939 (also SSRN 1968696) — SEARCH-CONFIRMED. Theory: upfront static contracts lock in ineffective founders; delayed contracting risks idea appropriation; **contingent contracts with vesting mitigate both**, and contingency is most valuable when founder-skill uncertainty is high.
- **Hellmann, Schure, Tergiman & Vo (2019), "Ownership dynamics within founder teams," *Strategic Entrepreneurship Journal* 13(3): 256–287** — https://sms.onlinelibrary.wiley.com/doi/abs/10.1002/sej.1328 — SEARCH-CONFIRMED. Longitudinal BC registry data: **equal-splitting teams exhibit "dynamic fairness preference" — they almost never adjust relative stakes even as contributions diverge**; stakes move mainly at financing events. (Exact N not surfaced — not reported.)
- Supports: the single most important design decision — §2.1's *automatic, formulaic* rebalancing. The 2019 paper shows voluntary renegotiation does not happen; the 2015 model shows contingent contracts are the fix; our ledger makes the contingency self-executing.
- Strength: **both peer-reviewed; 2015 = pure theory; 2019 = correlational longitudinal.**

### A10. Organizational justice
- **Colquitt (2001), *J. Applied Psychology* 86(3): 386–400** — https://pubmed.ncbi.nlm.nih.gov/11419799/ — SEARCH-CONFIRMED. Four distinct justice dimensions (distributive, procedural, interpersonal, informational) differentially predict commitment, rule compliance, authority evaluation, helping.
- **Colquitt, Conlon, Wesson, Porter & Ng (2001), "Justice at the millennium," *JAP* 86(3): 425–445** — https://pubmed.ncbi.nlm.nih.gov/11419803/ — SEARCH-CONFIRMED. Meta-analysis of 183 studies; each justice dimension adds incremental variance; procedural justice is a notably strong unique predictor of commitment and evaluations of authority. (Exact per-outcome coefficients sit in Tables 2–5 of the paper and were not surfaced in accessible text — not reported here.)
- Supports: design §2.2's process guarantees (published rules before outcomes, uniform rates, appeal rights, audit rights): fair process has payoff independent of the numbers.
- Strength: **peer-reviewed; meta-analytic but correlational inputs; workplace samples, not founder teams.**

### A11. de Wit, Greer & Jehn (2012), "The paradox of intragroup conflict: A meta-analysis," *J. Applied Psychology* 97(2): 360–390
- URL: https://pubmed.ncbi.nlm.nih.gov/21842974/ — SEARCH-CONFIRMED.
- Findings: 116 studies, 8,880 groups. **Relationship and process conflict are reliably negative for outcomes; task conflict is not negative overall and is most positive in top-management teams, when task conflict doesn't bleed into relationship conflict, and when the outcome is decision quality** (overturning De Dreu & Weingart 2003 — a live disagreement in the literature).
- Supports: design §3.4 (channeling disagreement into structured written proposals + disagree-and-commit: preserve task conflict, starve relationship conflict) and §7 (fast, impersonal dispute resolution).
- Strength: **peer-reviewed meta-analysis; correlational inputs; exact ρ values not surfaced — directions and moderators only.**

### A12. Wu, Cormican & Chen (2020), "A Meta-Analysis of Shared Leadership," *J. of Leadership & Organizational Studies* 27(1): 49–64
- URL: https://journals.sagepub.com/doi/10.1177/1548051818820862 — SEARCH-CONFIRMED.
- Most recent shared-leadership meta-analysis (antecedents + outcomes). Listed for completeness; we did not extract effect sizes and do not rest any claim on it.
- Strength: **peer-reviewed; not load-bearing in our design.**

---

## Part B — Statutes, cases, regulators, and institutional policies

*(Ratings here: statute/case = highest authority for what the law says; agency page =
authoritative guidance; firm memo = expert secondary. All SEARCH-CONFIRMED as
described in the disclosure above; counsel must pull primaries before acting.)*

### B1. Massachusetts Wage Act — M.G.L. c.149 §148
- https://malegislature.gov/Laws/GeneralLaws/PartI/TitleXXI/Chapter149/Section148 — SEARCH-CONFIRMED (official legislature site).
- Weekly/bi-weekly payment within 6 days of period close; discharged employee must be paid in full on the day of discharge.
- Supports: design §8.1 (the unpaid-worker problem is a live statutory violation, not a formality). **Statute.**

### B2. Mandatory treble damages — M.G.L. c.149 §150; *Reuter v. City of Methuen*, 489 Mass. 465 (2022)
- Opinion: https://law.justia.com/cases/massachusetts/supreme-court/2022/sjc-13121.html · firm summary: https://www.seyfarth.com/news-insights/no-quarter-sjc-mandates-treble-damages-for-any-late-payment-of-wages-even-honest-corrected-mistakes.html — SEARCH-CONFIRMED.
- Treble damages are **mandatory, strict-liability liquidated damages** — even for wages paid late before suit, regardless of intent.
- Supports: design §8.1's urgency framing. **SJC case + statute.**

### B3. Personal liability of LLC managers — *Cook v. Patient Edu, LLC*, 465 Mass. 548 (2013)
- http://masscases.com/cases/sjc/465/465mass548.html · https://foleyhoag.com/news-and-insights/publications/alerts-and-updates/2013/june/ma-highest-court-decides-that-managers-at-llcs-can-be-individually-liable-for-wage-act-violations/ — SEARCH-CONFIRMED.
- An LLC manager who "controls, directs, and participates to a substantial degree in formulating and determining policy" is personally (civilly and criminally) liable under §148.
- Supports: design §8.1 — the five founders are personally exposed. **SJC case.**

### B4. FLSA: no unpaid work at for-profits; equity is not wages
- DOL elaws: https://webapps.dol.gov/elaws/whd/flsa/docs/volunteers.asp ("employees may not volunteer services to for-profit private sector employers") — SEARCH-CONFIRMED. **Agency.**
- 29 C.F.R. §531.27 (wages payable in cash or equivalent, free and clear): https://www.law.cornell.edu/cfr/text/29/531.27 — SEARCH-CONFIRMED. **Regulation.**
- Foley & Lardner (Oct 2024), equity-only compensation violates the FLSA: https://www.foley.com/insights/publications/2024/10/equity-compensate-employees-violates-flsa/ — SEARCH-CONFIRMED. **Firm memo.**
- DOL Fact Sheet #56 (stock options and the regular rate): https://www.dol.gov/agencies/whd/fact-sheets/56-flsa-stock-options — SEARCH-CONFIRMED. **Agency.**
- Supports: design §8.1 — equity grants cannot cure the wage violation.

### B5. MA independent-contractor ABC test — M.G.L. c.149 §148B
- https://www.mass.gov/info-details/massachusetts-law-about-independent-contractors — SEARCH-CONFIRMED. Prong B (service outside the usual course of business) defeats reclassifying core engineers as contractors.
- Supports: design §8.1 (no contractor relabeling escape). **Statute + agency page.**

### B6. Massachusetts LLC Act — M.G.L. c.156C §§24, 63
- §24 (manager-managed option): https://malegislature.gov/Laws/GeneralLaws/PartI/TitleXXII/Chapter156c/Section24 — SEARCH-CONFIRMED.
- §63 (duties may be "expanded or restricted" — but, per commentary, not eliminated as in Delaware; implied covenant non-waivable): https://malegislature.gov/Laws/GeneralLaws/PartI/TitleXXII/Chapter156c/Section63 — SEARCH-CONFIRMED; gloss via https://www.romanolaw.com/can-fiduciary-obligations-be-waived-in-massachusetts/ (firm commentary — flagged for counsel).
- Supports: OA Articles VI & XIV (manager-managed structure; fiduciary-duty tailoring limits). **Statute; the modification-limit gloss is secondary.**

### B7. Delaware conversion — DGCL §265; MA-side mechanics
- Del. Code tit. 8 §265 via https://law.justia.com/codes/delaware/title-8/chapter-1/subchapter-ix/section-265 (official page https://delcode.delaware.gov/title8/c001/sc09/ could not be directly pulled) — SEARCH-CONFIRMED. "Other entity" includes a foreign (Massachusetts) LLC; converted corporation is deemed the same entity.
- MA-side: c.156C merger sections exist (e.g., §60: https://malegislature.gov/Laws/GeneralLaws/PartI/TitleXXII/Chapter156C/Section60 — SEARCH-CONFIRMED) but the exact outbound-conversion filing route is **conflicting in secondary sources** — flagged in OA 3.3 for counsel. Practitioner corroboration: https://answers.justia.com/question/2025/07/24/can-i-convert-a-ma-llc-to-a-de-c-corp-us-1069650 · https://www.nolo.com/legal-encyclopedia/converting-llc-corporation-s-corporation-delaware.html — SEARCH-CONFIRMED. **Statute (DE); MA route = lower confidence, expressly flagged.**

### B8. Conversion tax treatment — Rev. Rul. 84-111; IRC §351
- The Tax Adviser (AICPA): https://www.thetaxadviser.com/issues/2008/mar/holdingperiodandbasisconsiderationsofpartnershipconversions/ — SEARCH-CONFIRMED. Three blessed methods (assets-over, assets-up, interests-over), generally tax-free under §351, different basis/holding-period consequences.
- Supports: OA 3.3. **IRS revenue ruling as described by AICPA publication.**

### B9. QSBS — IRC §1202 including 2025 OBBBA changes
- Pre-change mechanics (stock issued ≤ July 4, 2025): 100% exclusion; greater of $10M or 10× basis; >5-year hold; C-corp; ≤$50M gross assets. Canonical text: https://www.law.cornell.edu/uscode/text/26/1202 (fetch blocked; substance corroborated by the firm memos below).
- **OBBBA (P.L. 119-21, July 4, 2025) changes for stock issued after July 4, 2025: tiered exclusion 50%/75%/100% at 3/4/5-year holds; cap $10M→$15M; gross-asset ceiling $50M→$75M (both indexed).** Perkins Coie: https://perkinscoie.com/insights/update/significant-changes-one-big-beautiful-bill-act-qualified-small-business-stock · Holland & Knight: https://www.hklaw.com/en/insights/publications/2025/07/one-big-beautiful-bill-act-increases-tax-benefits-for-qualified-small · Mintz: https://www.mintz.com/insights-center/viewpoints/2906/2025-07-09-qsbs-benefits-expanded-under-one-big-beautiful-bill-act — all SEARCH-CONFIRMED. **Firm explainers of enacted statute.**
- Conversion timing: QSBS clock starts **at conversion**; §1202(i) sets basis = FMV of contributed assets at conversion (so later conversion raises the 10× cap; earlier conversion starts the clock sooner and preserves gross-asset headroom). Fox Swibel: https://foxswibel.com/llc-to-c-corp-conversion-part-1-when-an-llc-to-c-corp-conversion-can-and-cannot-qualify-for-section-1202/ · Hanson Bridgett: https://www.hansonbridgett.com/publication/240301-7000-llcs-may-help-maximize-qsbs-benefits — SEARCH-CONFIRMED. **Specialist firm explainers.**
- Supports: design §1 and OA 3.3 (convert at/just before the raise; model both timings).

### B10. Profits interests — Rev. Proc. 93-27 & 2001-43; hurdles; conversion trap
- IRS Rev. Proc. 2001-43: https://www.irs.gov/pub/irs-drop/rp-01-43.pdf — SEARCH-CONFIRMED (irs.gov PDF). Safe harbor: profits-interest grant non-taxable unless predictable income stream, disposed within 2 years, or PTP interest; 2001-43 extends to unvested interests. **IRS primary.**
- Hurdle + protective 83(b): The Tax Adviser (Jan 2025): https://www.thetaxadviser.com/issues/2025/jan/profits-interests-the-most-tax-efficient-equity-grant-to-employees/ · RSM FAQ: https://rsmus.com/insights/services/business-tax/frequently-asked-questions-about-profits-interests.html · Proskauer on *ES NPA Holding*: https://www.proskauer.com/blog/tax-court-decision-interprets-profits-interest-safe-harbor-under-irs-rev-proc-93-27/ — SEARCH-CONFIRMED. **AICPA/firm explainers + Tax Court case note.**
- **Conversion trap:** profits interests convert to stock only above their hurdle; near-conversion grants can convert to nothing. Baker Tax Law: https://mbakertaxlaw.com/llc-conversions/ — SEARCH-CONFIRMED. **Specialist firm explainer.**
- Supports: OA 3.6's three-option bracket; design §2.4.

### B11. 83(b) elections — 30-day jurisdictional deadline; Form 15620
- IRS Form 15620: https://www.irs.gov/pub/irs-pdf/f15620.pdf (electronic filing opened July 2025) — SEARCH-CONFIRMED. Explainers: RSM: https://rsmus.com/insights/services/business-tax/section-83b-consideration-employees-receiving-stock-compensation.html · Carta: https://carta.com/learn/equity/stock-options/taxes/83b-election/ — SEARCH-CONFIRMED.
- Supports: OA 3.6, 11.4. **IRS primary + explainers.**

### B12. Securities exemptions & 409A
- Rule 701 (compensatory issuances; 12-month cap = greatest of $1M / 15% assets / 15% of class; enhanced disclosure >$10M): https://www.law.cornell.edu/cfr/text/17/230.701 · SEC release: https://www.sec.gov/rules-regulations/1999/02/rule-701exempt-offerings-pursuant-compensatory-arrangements · Cooley GO: https://www.cooleygo.com/why-private-companies-should-know-about-rule-701-options-rsas-and-rsus/ · Carta: https://carta.com/learn/startups/equity-management/rule-701/ — SEARCH-CONFIRMED. **Regulation + SEC + explainers.**
- Reg D 506(b): explainer-level corroboration only; counsel to cite 17 C.F.R. §230.506 directly — **flagged, lower confidence.**
- §409A: RSM valuation explainer: https://rsmus.com/insights/services/business-tax/general-equity-compensation-valuation-rules-for-private-entities.html · IRS Notice 2005-1 Q&A-7 (properly-structured profits interests outside 409A): https://www.irs.gov/pub/irs-drop/n-05-01.pdf — SEARCH-CONFIRMED. **IRS notice + firm explainer.**
- Supports: OA 2.3, 3.6, 11.5.

### B13. VC preference for Delaware C-corps; SAFEs are corporate paper
- Cooley GO, "Where Should You Incorporate?": https://www.cooleygo.com/where-should-you-incorporate/ — SEARCH-CONFIRMED.
- AngelList, "Schedule K-1 for VCs" (UBTI/K-1 rationale — most VC funds cannot hold pass-throughs): https://www.angellist.com/learn/schedule-k-1 — SEARCH-CONFIRMED.
- Frost Brown Todd on funds and QSBS: https://frostbrowntodd.com/private-equity-and-venture-capital-fund-investment-in-qualified-small-business-stock-a-guide/ — SEARCH-CONFIRMED.
- YC SAFE documents (Delaware-corporation forms): https://www.ycombinator.com/documents · Cooley GO SAFE generator ("intended only for US companies incorporated in Delaware"): https://www.cooleygo.com/documents/y-combinator-safe-financing-document-generator/ — SEARCH-CONFIRMED.
- Supports: design §1; OA Article III. **Firm/industry explainers; consistent across four independent sources.**

### B14. Reverse vesting & founder-stock repurchase as investor conditions
- Cooley GO, "Founder's Stock, Vesting and Founder Departures" (48-month/12-month-cliff standard; repurchase at lower of cost/FMV; vesting "may be imposed later as a condition of investment"): https://www.cooleygo.com/founder-basics-founders-stock/ · "Protecting Your Founder Equity": https://www.cooleygo.com/protecting-founder-equity/ — SEARCH-CONFIRMED.
- NVCA model documents suite: https://nvca.org/model-legal-documents/ — **the nvca.org page itself did not surface in results (lower confidence)**; suite's existence/contents corroborated via Foley & Lardner on the Oct 2, 2025 NVCA updates: https://www.foley.com/insights/publications/2025/10/breaking-down-the-nvca-what-founders-and-vcs-need-to-know/ — SEARCH-CONFIRMED.
- Supports: OA 3.5, 10.2, 13.2. **Firm explainers + industry-standard forms.**

### B15. MA Noncompetition Agreement Act — M.G.L. c.149 §24L
- https://www.mass.gov/info-details/mass-general-laws-c149-ss-24l · annotation: https://beckreedriden.com/the-massachusetts-noncompetition-agreement-act-massachusetts-general-laws-c-149-s-24l/ — SEARCH-CONFIRMED. Garden leave (≥50% of highest annualized base over prior 2 years) or other mutually-agreed consideration; 12-month cap; unenforceable vs. non-exempt employees and no-cause terminations; NDAs/non-solicits excluded.
- Supports: OA 11.3. **Statute + state page.**

### B16. Foreign qualification after conversion — M.G.L. c.156D §15.03
- https://malegislature.gov/Laws/GeneralLaws/PartI/TitleXXII/Chapter156D/Section15.03 · https://www.sec.state.ma.us/divisions/corporations/filing-by-subject/corporations/corporations-domestic-foreign.htm — SEARCH-CONFIRMED. Registration within 10 days of commencing business in MA; MA corporate excise continues.
- Supports: OA 3.3 flag. **Statute + state agency.**

### B17. Yale policies (the professor)
- Yale Conflict of Interest policy: https://research-support.yale.edu/research-compliance-regulatory-affairs/conflict-of-interest-office/policies-procedures-guidance · PDF https://research-support.yale.edu/sites/default/files/2025-03/coi_policy_0.pdf — SEARCH-CONFIRMED. Annual disclosure; Provost's Committee review for complex cases.
- External-activities time limit: https://provost.yale.edu/policies/external-professional-activities-guidance — SEARCH-CONFIRMED. **≤ one day per seven-day week on average**; ownership/management of private enterprises subject to review and limitation.
- Yale Patent Policy (university owns inventions made within employment scope or with more-than-minimal use of university resources; inventor royalty share up to 30% top tier): https://ventures.yale.edu/sites/default/files/2023-03/Yale_Patent_Policy.pdf · https://ventures.yale.edu/yale-technologies/patent-policy-for-faculty — SEARCH-CONFIRMED.
- Faculty-in-startups practice (advisor/consultant roles preferred; COI Committee review; Yale may take board rights where it holds equity): https://ventures.yale.edu/yale-technologies/frequently-asked-questions — SEARCH-CONFIRMED.
- Federal disclosure (NSF current-and-pending / NIH other support) via university research-office guidance: https://ora.stanford.edu/resources/disclosure-resources/national-science-foundation-nsf/nsf-current-and-pending-support · https://ras.mit.edu/grant-and-contract-administration/sponsor-information/nsf/national-science-foundation-disclosure-guidance — SEARCH-CONFIRMED.
- Supports: design §6; OA Article VIII. **Primary institutional policies + agency-derived guidance.**

---

## Part C — Industry data and practitioner frameworks

### C1. Slicing Pie (Mike Moyer) — the dynamic-equity framework we adapt
- URLs (all SEARCH-CONFIRMED): model overview: https://slicingpie.com/learn-slicing-pie-model/ · multipliers: https://slicingpie.com/the-magic-of-mutipliers/ (the "mutipliers" typo is in the real URL) · FMV rules: https://slicingpie.com/fair-market-value/ and https://slicingpie.com/the-fair-market-value-of-a-relationship/ · separation rules: https://slicingpie.com/slices-that-can-survive-separation/ and https://slicingpie.com/how-to-fire-a-cofounder/ · rebuttal page: https://slicingpie.com/my-lawyer-says-slicing-pie-wont-work/
- Mechanics we rely on: a "slice" = fair-market value of an at-risk contribution × a risk multiplier; **% = your slices ÷ all slices**, recalculated continuously; **non-cash multiplier 2×, cash multiplier 4×**; FMV = what the contribution would fetch from a payer who could pay; the split **freezes at breakeven or a large raise (typically Series A)**; separation rules: terminated-for-cause / resign-without-good-reason loses non-cash slices and the 4× on cash; terminated-without-cause / resign-for-good-reason keeps slices at full value. FMV of "the" founding idea = revenue royalty; relationships = standard commission/finder's fee.
- Supports: the architecture of design §2 and OA Article IV. Note where we deliberately deviate (design §2.5): we keep the multipliers and freeze logic but replace the loses-everything separation rule with earned-is-kept + FMV call options, and we do not adopt idea royalties.
- Strength: **practitioner framework, canonical primary source; no outcome data.** Criticisms (all SEARCH-CONFIRMED): Sentient Law (implementation perils; US legal/tax framework not geared to dynamic equity): https://www.sentientlaw.com/dynamic-equity-slicing-pie/ · Equity Matrix (tax gaps in the book; **but LLCs can adjust ownership percentages without the taxable events corporations face** — key for us; Google-Sheet cap tables underwhelm investors): https://equitymatrix.io/blog/slicing-pie-problems · Fairsquare (companies on the model have raised through multiple rounds): https://www.fairsquarellp.com/investors-and-slicing-pie/ · neutral explainer: https://www.vestd.com/blog/slicing-pie-a-tasty-way-to-share-equity

### C2. FAST agreement (Founder Institute) — advisor-equity benchmark
- URLs: https://fi.co/fast (matrix corroborated via FI's Medium mirror https://medium.com/@founding/the-founder-institutes-standard-advisor-agreement-for-startups-fast-6f99e2762a3c and https://fi.co/insight/the-founder-institute-s-standard-advisor-agreement-for-startups-fast; explainer https://eqvista.com/fast-agreement-everything-you-need-to-know/) — SEARCH-CONFIRMED.
- FAST v2 matrix: Standard 0.25/0.20/0.15%, Strategic 0.50/0.40/0.30%, Expert 1.00/0.80/0.60% (idea/startup/growth stage); advisor vesting 2 years, monthly, 3-month cliff. **A claimed "FAST v3" (June 2026, two-tier, 0.50% standard) rests on a single secondary source and is UNCONFIRMED — we cite v2 only.**
- Supports: design §6 (the professor's realistic advisor-market range: expert advisor at startup stage ≈ 0.80%; our 2.0% cap is ~2.5× that ceiling).
- Strength: **practitioner template; self-reported wide adoption; no outcome data.**

### C3. Carta cap-table data (multiple studies)
- Founder splits: https://carta.com/data/founder-equity-split-trends-2024/ · https://carta.com/data/how-co-founders-split-equity/ · https://carta.com/data/two-founder-teams/ — SEARCH-CONFIRMED. **45.9% of two-founder teams split equally in 2024 (up from 31.5% in 2015); equal splits fall with team size — 27.3% of three-founder, 16.7% of four-founder teams**; dataset ≈ 45,000+ startups incorporated 2015–2024.
- Option pools & ownership: https://carta.com/learn/startups/equity-management/option-pool/ · https://carta.com/data/founder-ownership/ · https://carta.com/data/founder-ownership-2026/ — SEARCH-CONFIRMED. **Median pool ≈ 12.1% at seed, 15% at Series A; median founding-team ownership 56.2% post-seed, 36.1% at Series A.**
- Vesting: https://carta.com/learn/equity/stock-options/vesting/ · role medians via Carta's Peter Walker: https://www.linkedin.com/posts/peterjameswalker_cartadata-advisors-boardmembers-activity-7077314329678594048-Hx85 — SEARCH-CONFIRMED. **4-year/1-year-cliff is the standard; where a cliff exists, ≥95% are at one year; advisors: median 2-year vesting, no cliff.** (No corroborated figure for "% of all grants exactly 4-year" — not claimed.)
- Advisor grant sizes: https://carta.com/data/linkedin-startup-advisor-equity-cheatsheet/ · https://carta.com/data/linkedin-preseed-advisor-equity-h1-2023/ — SEARCH-CONFIRMED. **Median advisor grant: pre-seed ≈ 0.25%, seed 0.10%, Series A 0.07%.** Notably below FAST — we present the tension in design §6.
- Dead equity: **no Carta dead-equity dataset could be corroborated — none is cited.**
- Supports: design §§2.3, 2.6, 5, 6; OA 3.4.
- Strength: **large-sample platform data (strongest class of industry evidence); descriptive, platform-selection caveats apply.**

### C4. Y Combinator / Michael Seibel — the strongest counterargument to contribution-based splits
- URLs: https://www.michaelseibel.com/blog/how-to-split-equity-among-founders · https://www.ycombinator.com/library/5x-how-to-split-equity-among-co-founders · https://www.ycombinator.com/library/LP-co-founder-equity-mistakes-to-avoid — SEARCH-CONFIRMED.
- Position: split **equally or near-equally** because "all the work is ahead of you" (7–10 years); "more equity equals more motivation"; founder equity should always carry **4-year/1-year-cliff vesting** and "giving away founder equity is not something that should be innovated on."
- Supports: design §2.1 presents this view *against* our approach and explains why the founders' fixed requirements (and this team's actual divergence history) put the company outside YC's assumed fact pattern; YC's vesting dictum supports OA 3.5.
- Strength: **practitioner opinion from the highest-profile accelerator; informed by thousands of companies but published as argument, not data.**

### C5. Investor writing on founder vesting and dead equity
- Fred Wilson (USV), "Founder Vesting": https://avc.com/2018/03/founder-vesting/ · "Employee Equity: Vesting": https://avc.com/2010/11/employee-equity-vesting/ — SEARCH-CONFIRMED. Founder stock should vest over ~4 years; replacement-cost logic (a replacement CEO grant runs **2.5–7.5%**).
- Brad Feld, "Term Sheet: Vesting": https://feld.com/archives/2005/05/term-sheet-vesting/ — SEARCH-CONFIRMED. Canonical explainer of why VCs require founder reverse vesting.
- ISA Ventures, "Dead equity on your cap table is a major red flag": https://isaventures.substack.com/p/dead-equity-on-your-cap-table-is — SEARCH-CONFIRMED. Defines dead equity as **an uninvolved holder of >5% at early stage**; a departed co-founder holding 25% can kill a round. Corroborating: Pulley, https://pulley.com/guides/part-iii-is-your-cap-table-broken-mistakes-to-avoid-the-startup-founders-guide-to-equity
- Supports: design §5 (inactive founders), OA 9.2/9.6. Strength: **single-firm investor practitioners; the >5% threshold is one fund's rule of thumb, labeled as such.**

### C6. Employee equity benchmarks
- Index Ventures, *Rewarding Talent* / OptionPlan: https://www.indexventures.com/rewarding-talent/ · https://www.indexventures.com/optionplan/ · https://www.indexventures.com/rewarding-talent/allocation-considerations-and-benchmarks · https://www.indexventures.com/rewarding-talent/calculating-initial-grants-at-series-a — SEARCH-CONFIRMED. Dataset: **20,000+ grants, 1,650+ startups.**
- Holloway Guide, "Typical Employee Equity Levels": https://www.holloway.com/g/equity-compensation/sections/typical-employee-equity-levels — SEARCH-CONFIRMED. Post-A: **lead engineer 0.5–1%; senior 0.33–0.66%**; by hire number (Polovets): **#1: 2–3%, #2–5: 1–2%, #6–7: 0.5–1%, #8–14: 0.4–0.8%**; unsalaried/seed hires warrant more.
- Supports: design §2.6's sanity check that our worked example lands employees in or above market ranges (they were unsalaried, so above-market is correct).
- Strength: **VC-compiled dataset + curated practitioner guide.**

### C7. Decision-making frameworks (provenance sources)
- Apple DRI: Adam Lashinsky, *Inside Apple* (2012), https://www.hachettebookgroup.com/titles/adam-lashinsky/inside-apple/9781611130966/ — SEARCH-CONFIRMED. **Journalistic single-firm account — the standard citation; no Apple primary source exists.**
- Amazon Type 1/Type 2 doors: Bezos 2015 shareholder letter, https://s2.q4cdn.com/299287126/files/doc_financials/annual/2015-Letter-to-Shareholders.PDF — SEARCH-CONFIRMED. **Primary source.**
- Disagree-and-commit: Bezos 2016 letter, https://www.aboutamazon.com/news/company-news/2016-letter-to-shareholders — SEARCH-CONFIRMED. **Primary source.**
- RAPID: Bain, https://www.bain.com/insights/rapid-decision-making/ and Rogers & Blenko, "Who Has the D?," *HBR* Jan 2006 — SEARCH-CONFIRMED. Single accountable "D" per decision.
- Supports: design §3.4; OA 6.4–6.6. Strength: **primary corporate sources (Amazon) > consultancy framework (Bain/HBR) > journalism (Apple).** These are provenance citations for mechanisms, not outcome evidence.

### C8. Deadlock and buy-sell mechanics
- Peckar & Abramson, "Shotgun Buy/Sell Option Agreements": https://www.pecklaw.com/business-owner-rights/shotgun-buy-sell-option-agreements/ · LegalClarity, "Texas Shootout Clause": https://legalclarity.org/texas-shootout-clause-how-it-works-risks-and-tax-rules/ · ABA Business Law Today (Mar 2017), "Deadlock-Breaking Mechanisms in LLCs": https://www.americanbar.org/groups/business_law/resources/business-law-today/2017-march/deadlock-breaking-mechanisms/ · Florida Mediation Group, "Dutch Auctions and Texas Shoot-Outs": https://www.uww-adr.com/blog/dutch-auctions-and-texas-shoot-outs/ · Aaron Hall, "Legal Solutions for Deadlock in LLC Operating Agreements": https://aaronhall.com/legal-solutions-for-deadlock-in-llc-operating-agreements/ — all SEARCH-CONFIRMED.
- Mechanics: shotgun ("I cut, you choose") is self-policing on price but **documented to favor the deeper-pocketed party**; Texas shootout = simultaneous sealed bids, highest must buy; med-then-arb tiers (30–60-day mediation, then binding arbitration) are the common contractual ladder; all beat judicial dissolution.
- **Honesty note: no reputable source was found pairing "baseball arbitration" specifically with LLC deadlock clauses.** Our use of final-offer arbitration for *valuation* disputes (OA 12.4) is a design choice borrowed from general commercial ADR practice, flagged for counsel rather than presented as an LLC-market standard.
- Supports: design §7; OA Article XII. Strength: **law-firm/bar-association explainers; mechanics only, no incidence data.**

### C9. Co-founder conflict as a failure cause
- Wasserman, *The Founder's Dilemmas* (2012) — **65% of high-potential startup failures driven by people problems/co-founder conflict** (book's underlying HBS dataset; secondary confirmation: https://www.entrepreneur.com/leadership/harvard-business-school-professor-says-65-of-startups-fail/370367 — SEARCH-CONFIRMED). **Large-sample academic study.**
- CB Insights, "The Top 20 Reasons Startups Fail": https://s3-us-west-2.amazonaws.com/cbi-content/research-reports/The-20-Reasons-Startups-Fail.pdf — SEARCH-CONFIRMED. 101 post-mortems (multi-cause): **"not the right team" 23%; "disharmony among team/investors" 13%.** **Small self-reported sample — weaker; both presented.**
- Supports: design §7's premise that governance-failure risk rivals product risk.

### C10. Market-rate compensation benchmarks (pricing unpaid work)
- Levels.fyi, Software Engineer data: https://www.levels.fyi/t/software-engineer — SEARCH-CONFIRMED. **US senior SWE median total comp ≈ $312K (2025), up 4.2% from $300K (2024)**; startup cash comp runs far below big-tech total comp.
- Carta, "State of Startup Compensation, H2 2025": https://carta.com/data/startup-compensation-h2-2025/ — SEARCH-CONFIRMED. New-hire engineer/PM salaries ≈ **$189K average**; startup salaries +~5% 2024→2025.
- Supports: design §2.3's Rate Table (we price contribution hours at *startup-market cash* benchmarks per Carta, not big-tech total comp — the choice and its rationale are explained there).
- Strength: **large-sample data providers; levels.fyi is crowdsourced/verified-offer; Carta is payroll-platform data.**

---

## Items we looked for and could NOT support (kept honest)

1. **A Carta "dead equity" dataset** — does not appear to exist; the >5% threshold comes from a single fund (C5) and is labeled a rule of thumb.
2. **"FAST v3" (2026)** — single secondary source; unconfirmed; we cite the v2 matrix.
3. **Baseball arbitration as an LLC-deadlock standard** — no reputable pairing found; our OA 12.4 use is flagged as a design choice.
4. **Exact overall corrected ρ** for D'Innocenzo et al. (2016) and Nicolaides et al. (2014), and the per-outcome coefficient tables of Colquitt et al. (2001) and de Wit et al. (2012) — behind paywalls; directions and moderators only.
5. **Peer-reviewed outcome studies of Slicing Pie or any dynamic-split framework** — none found; the model's empirical support is indirect (A1, A9) and its direct support is practitioner-anecdotal (C1). Our design treats it accordingly: we adopt its arithmetic, not its untested claims.
6. **Any causal evidence on governance structure → startup performance** — the leadership literature is correlational or theoretical throughout (A4–A8); the design says so wherever it leans on it.
