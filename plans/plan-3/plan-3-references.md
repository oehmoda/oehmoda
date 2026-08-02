# Plan-3 — Annotated Bibliography

**Team plan-3.** Every source below supports specific claims in `plan-3-design.md` and `plan-3-one-pager.md`.

**Verification disclosure (honesty note):** This research environment's outbound network policy blocked *direct* fetches of external URLs (all HTTPS fetches returned a gateway policy denial). Each URL below was instead verified as live through current web-search index results that returned the URL together with matching page-content excerpts at research time (2026-08-01). None of these citations is from model memory alone; however, direct click-through verification was not possible, and a small number of URLs may have moved. Where a claim rests on a paywalled academic paper, we cite the publisher or SSRN landing page.

**Evidence-strength scale used throughout:**
- **P** — primary legal source (statute, regulation, revenue procedure, case law)
- **PR-C** — peer-reviewed, causal or quasi-causal identification
- **PR-X** — peer-reviewed, correlational/descriptive
- **D** — large-sample practitioner/industry data (Carta, Index, etc.)
- **L** — law-firm / accounting-firm practitioner guidance
- **O** — practitioner opinion / framework / anecdote

**Isolation attestation:** We did not read, check out, diff, or browse any other team's branch or files at any point. We listed remote branch *names* once, solely to choose an unused plan number.

---

## Section A. LLC equity instruments & taxation

**A1. Rev. Proc. 93-27, 1993-2 C.B. 343 (IRS).**
Full text reproduced at https://www.bradfordtaxinstitute.com/Endnotes/Rev_Proc_93-27.pdf (and restated in Rev. Proc. 2001-43, A2).
*Supports:* the design's use of profits interests as the tax-free-at-grant LLC equity instrument; definition of capital vs. profits interest (hypothetical liquidation-at-FMV test); the three safe-harbor exclusions (predictable income stream; disposition within 2 years; publicly traded partnership).
*Strength:* **P**.

**A2. Rev. Proc. 2001-43, 2001-2 C.B. 191 (IRS).**
https://www.irs.gov/pub/irs-drop/rp-01-43.pdf
*Supports:* unvested profits interests are tested at grant, vesting is not a taxable event, provided the holder is treated as a partner from grant (K-1s from day one) and no deduction is taken. Basis for the design's quarterly-vesting profits-interest units with protective 83(b) filings.
*Strength:* **P**.

**A3. ES NPA Holding, LLC v. Commissioner, T.C. Memo. 2023-55 (May 3, 2023), via Proskauer Rose analysis.**
https://www.proskauer.com/blog/tax-court-decision-interprets-profits-interest-safe-harbor-under-irs-rev-proc-93-27/ ; opinion PDF: https://www.skadden.com/-/media/files/publications/2023/05/tax-court-holds-indirect-grant-of-profits-interest/es-npa-decision.pdf
*Supports:* broad reading of "services to or for the benefit of" the partnership — comfort that retroactive-period service (including pre-formalization work) can support profits-interest grants.
*Strength:* **P** (case law) via **L** analysis.

**A4. Morse LLP (Waltham, MA), "Explaining Profits Interests and Their Tax Consequences."**
https://www.morse.law/news/profits-interests/
*Supports:* the dual-status consequence — a profits-interest recipient becomes a K-1 partner, W-2 status ends, SE tax and estimated taxes begin; and the practical warning that small grants to many employees may not be worth the compliance burden. Basis for the design's decision to weigh profits interests vs. phantom units for employees and to accelerate C-corp conversion.
*Strength:* **L** (Massachusetts firm — locally relevant).

**A5. Foley & Lardner, "Unlocking the Power of Equity-Based Incentive Compensation: Basics of Profits Interests" (Oct. 2024).**
https://www.foley.com/insights/publications/2024/10/equity-based-incentive-compensation-profits-interests/
*Supports:* threshold-value/distribution-hurdle mechanics (hurdle ≥ current FMV so liquidation value at grant is $0); Rule 701 exemption applies to compensatory LLC grants; time- and performance-vesting of profits interests.
*Strength:* **L**.

**A6. The Tax Adviser (AICPA), "Profits interests: The most tax-efficient equity grant to employees" (Jan. 2025).**
https://www.thetaxadviser.com/issues/2025/jan/profits-interests-the-most-tax-efficient-equity-grant-to-employees/
*Supports:* hurdle and catch-up-provision mechanics; why capital interests (ordinary income at grant on FMV) and options on LLC units (NQSO-like spread income plus partner-flip at exercise) are avoided.
*Strength:* **L** (professional journal).

**A7. Armstrong Teasdale, "Equity-Based Compensation for Corporations, Partnerships and LLCs" (Apr. 2020).**
https://www.armstrongteasdale.com/thought-leadership/equity-based-compensation-for-corporations-partnerships-and-llcs/
*Supports:* the instrument menu (profits interests, phantom units, unit appreciation rights); §409A applies to LLC phantom/UAR/option arrangements (FMV strike needed — the "409A-analog" valuation discipline); phantom/UAR keeps recipients on W-2.
*Strength:* **L**.

**A8. Rev. Rul. 69-184 dual-status rule — Cherry Bekaert, "Dual Partner-Employee Tax Status: Structuring Solutions"; Grant Thornton, "Key considerations for dual-status taxpayers" (2022).**
https://www.cbh.com/insights/articles/dual-partner-employee-tax-status-structuring-solutions/ ; https://www.grantthornton.com/insights/alerts/tax/2022/key-considerations-for-dual-status-taxpayers
*Supports:* one cannot be both a partner and a W-2 employee of the same partnership (including through disregarded subsidiaries per 2016 regulations); consequences (guaranteed payments on K-1, loss of §125/fringe benefits); blocker/phantom workarounds.
*Strength:* **L** (interpreting **P**, Rev. Rul. 69-184).

**A9. The Tax Adviser (AICPA), "Missed Sec. 83(b) elections: Partnership and LLC special issues" (Dec. 2023).**
https://www.thetaxadviser.com/issues/2023/dec/missed-sec-83b-elections-partnership-and-llc-special-issues/
*Supports:* protective 83(b) elections within a rigid 30-day window for unvested profits interests; why they are filed even though Rev. Proc. 2001-43 makes them technically unnecessary; Notice 2005-43 regime never finalized.
*Strength:* **L** (professional journal).

**A10. SEC Rule 701, 17 C.F.R. § 230.701 (text via Cornell LII) + Carta explainer.**
https://www.law.cornell.edu/cfr/text/17/230.701 ; https://carta.com/learn/startups/equity-management/rule-701/
*Supports:* compensatory-grant registration exemption is available to LLCs; 12-month caps (greatest of $1M / 15% of assets / 15% of class); enhanced disclosure above $10M in 12 months; natural-persons-only limit. State blue-sky must be checked separately (flagged for counsel).
*Strength:* **P** + **D**.

## Section B. Entity strategy & investability

**B1. IRC § 1202 (text via Cornell LII), as amended by the One Big Beautiful Bill Act (enacted July 4, 2025); Mintz alert (July 9, 2025); Holland & Knight; Davis Wright Tremaine.**
https://www.law.cornell.edu/uscode/text/26/1202 ; https://www.mintz.com/insights-center/viewpoints/2906/2025-07-09-qsbs-benefits-expanded-under-one-big-beautiful-bill-act ; https://www.hklaw.com/en/insights/publications/2025/07/one-big-beautiful-bill-act-increases-tax-benefits-for-qualified-small ; https://www.dwt.com/blogs/startup-law-blog/2025/07/qsbs-big-beautiful-bill-tax-code-upgrades
*Supports:* QSBS is C-corp-only; post-July-4-2025 stock: $15M (or 10× basis) per-issuer cap, $75M gross-asset ceiling, tiered 50%/75%/100% exclusion at 3/4/5-year holding. Central to the design's conversion-timing recommendation.
*Strength:* **P** + concurring **L** alerts.

**B2. Mintz, "Considering Converting an LLC into a Corporation? Here Are the QSBS Issues…" (Aug. 22, 2023); Holland & Knight, "Conversion of Partnership and LLC Interests into Qualified Small Business Stock" (Aug. 2025).**
https://www.mintz.com/insights-center/viewpoints/2906/2023-08-22-considering-converting-llc-corporation-here-are-qsbs ; https://www.hklaw.com/en/insights/publications/2025/08/conversion-of-partnership-and-llc-interests-into-qualified
*Supports:* QSBS clock starts at conversion, not LLC formation; §1202(i)(1)(B) basis = FMV at conversion (pre-conversion appreciation excluded from the exclusion but enlarges the 10× cap); convert-early-vs-late tension presented honestly in the design.
*Strength:* **L**.

**B3. Delaware Division of Corporations conversion filings (DGCL § 265); M.G.L. c. 156C § 69 (mergers/consolidations).**
https://corp.delaware.gov/conversions09/ ; https://malegislature.gov/Laws/GeneralLaws/PartI/TitleXXII/Chapter156C/Section69
*Supports:* mechanics of the MA-LLC → DE-C-corp statutory conversion (Certificate of Conversion + Certificate of Incorporation in DE, MA-side filings); merger-into-new-DE-corp alternative; ~$220 DE filing fee, practitioner-estimated $3k–$7k legal cost and 30–60-day timeline (cost figures are practitioner estimates, not statutory).
*Strength:* **P** (mechanics) / **O** (cost estimates).

**B4. Cooley GO C-corporation glossary & Delaware incorporation package; Baker Tax Law, "SAFEs in LLCs."**
https://www.cooleygo.com/glossary/c-corporation/ ; https://www.cooleygo.com/documents/incorporation-package-delaware/ ; https://mbakertaxlaw.com/safes-in-llcs/
*Supports:* why VC funds avoid pass-throughs (UBTI for tax-exempt LPs, ECI for foreign LPs, K-1 burden, standardized preferred-stock stack); the YC SAFE is drafted only for Delaware C-corps and an LLC issuing an unmodified SAFE creates partnership-interest tax ambiguity.
*Strength:* **L**.

**B5. Carta data via PitchBook, "Startups aren't abandoning Delaware — yet" (2025); Delaware Division of Corporations 2024 Annual Report.**
https://pitchbook.com/news/articles/startups-arent-abandoning-delaware-yet ; https://corp.delaware.gov/stats/2024-annual-report/
*Supports:* >90% of companies on Carta's platform are corporations; ~88% of C-corp startups on Carta incorporated in Delaware (late 2024). Grounds the design's claim that Delaware C-corp at first priced round is the overwhelming market norm.
*Strength:* **D**.

**B6. Practitioner syntheses on LLC-until-priced-round timing: Flux Law; SeedLegals US; My Startup Lawyer.**
https://www.flux.law/blog/convert-llc-to-delaware-c-corp ; https://seedlegals.com/us/resources/convert-llc-or-create-new-c-corp/ ; https://mystartuplawyer.com/blog/llc-for-startups-pros-cons-and-conversion-to-a-corporation/
*Supports:* pros/cons of staying an LLC pre-raise (pass-through losses vs. QSBS-clock cost, K-1 burden with many profits-interest holders, SAFE incompatibility, rushed-conversion risk); convert 30–60+ days ahead of a raise.
*Strength:* **O** (directionally consistent across firms).

---

## Section C. Dynamic / contribution-based equity & departed-founder handling

**C1. Slicing Pie official materials — "The Magic of Multipliers"; "Learn the Slicing Pie Model"; Grunt Fund Cheat Sheet (Mike Moyer).**
https://slicingpie.com/the-magic-of-mutipliers/ ; https://slicingpie.com/learn-slicing-pie-model/ ; https://slicingpie.com/wp-content/uploads/2017/02/Slicing-Pie-Grunt-Fund-Cheat-Sheet.pdf
*Supports:* the design's core formula skeleton — contributions valued at adjusted fair market value; **non-cash × 2, cash and unreimbursed expenses × 4**; founder hourly rate = (fair-market salary × 2) ÷ 2,000 hours; equity % = your slices ÷ all slices; the pie stays dynamic until breakeven or a funding event, then freezes — a trigger Moyer advises writing into the operating agreement in advance.
*Strength:* **O** (model author; no empirical validation — see C4).

**C2. Slicing Pie recovery framework — "How to Fire a Co-founder"; "Slices that Can Survive Separation."**
https://slicingpie.com/how-to-fire-a-cofounder/ ; https://slicingpie.com/slices-that-can-survive-separation/
*Supports:* the design's leaver matrix: bad leaver (for-cause termination or resignation without good reason) loses non-cash slices and gets cash back at 1×; good leaver (terminated without cause / resigns for good reason) keeps accrued slices, diluted only by others' future contributions.
*Strength:* **O**.

**C3. Critiques of dynamic equity — Equity Matrix "Slicing Pie problems"; Vestd "Slicing Pie: a tasty way to share equity?".**
https://equitymatrix.io/blog/slicing-pie-problems ; https://equitymatrix.io/blog/slicing-pie-guide ; https://www.vestd.com/blog/slicing-pie-a-tasty-way-to-share-equity
*Supports:* why the design imposes a hard **Freeze Event**: VCs require fixed cap tables; spreadsheet cap tables hurt credibility; continuous adjustment creates tax friction in corporations (works better in LLCs); bookkeeping burden; the model sets no forward expectations. *Bias note:* both critics sell competing equity tooling.
*Strength:* **O**.

**C4. Advocate counter-view — Sentient Law "The Truth about Slicing Pie"; Fairsquare LLP "Investors and Slicing Pie"; Forbes Legal Council "Overcoming the Misconceptions of Dynamic Equity" (2017).**
https://www.sentientlaw.com/dynamic-equity-slicing-pie/ ; https://www.fairsquarellp.com/investors-and-slicing-pie/ ; https://www.forbes.com/sites/forbeslegalcouncil/2017/12/12/overcoming-the-misconceptions-of-dynamic-equity/
*Supports:* the presented disagreement about investor reception of dynamic equity (advocates report multi-round raises without objection; Sentient claims ~50% of conventional-split teams hit an equity dispute needing legal intervention — unaudited, from own practice).
*Strength:* **O / anecdote** (advocates with commercial stakes). **Honesty note:** we found *no peer-reviewed empirical evaluation of Slicing Pie or any ex-post dynamic equity model* — a genuine evidence gap that the design acknowledges and manages by freezing before any financing.

**C5. Frank Demmler, "Founders' Pie Calculator" (Carnegie Mellon).**
https://www.andrew.cmu.edu/user/fd0n/35%20Founders'%20Pie%20Calculator.htm ; https://www.cmu.edu/swartz-center-for-entrepreneurship/assets/Connect%20Spring%202017/Frank%20Demmler%20-%20Equity%20Pie/Founders_Pie_Final.pdf
*Supports:* the alternative one-time weighted-factor negotiation (Idea, Business Plan, Domain Expertise, Commitment & Risk, Responsibilities; equity % = Σ(weight × score) ÷ team total) — considered and rejected in the design as too subjective for this team's "identical, objective terms" requirement; also documents the idea-premium doctrine (weight 7/10) that Slicing Pie rejects.
*Strength:* **O**.

**C6. Hellmann & Wasserman, "The First Deal: The Division of Founder Equity in New Ventures," Management Science 63(8) 2017; NBER w16922; SSRN 1805427.**
https://pubsonline.informs.org/doi/10.1287/mnsc.2016.2474 ; https://www.nber.org/papers/w16922 ; https://papers.ssrn.com/sol3/papers.cfm?abstract_id=1805427
*Supports:* the empirical premise of the whole design — 1,476 founders / 511 ventures; teams heterogeneous in idea generation, experience, or capital are less likely to split equally; **quick, un-negotiated equal splits correlate with lower first-financing valuations**; ≈10% of firm equity (~$450K NPV) at stake from wrongly agreeing to an equal split.
*Strength:* **PR-X** (large-sample, careful about causality).

**C7. Hervé Lebret, "Equity in Startups" (SSRN working paper).**
https://papers.ssrn.com/sol3/papers.cfm?abstract_id=3063860
*Supports:* long-run distribution of equity among founders/employees/investors across 400+ (mostly IPO) startups — context for what static splits produce.
*Strength:* **PR-X** (working paper, descriptive).

**C8. Sweat-equity valuation — Corporate Finance Institute; ICanPitch "Sweat Equity Guide" (2026); LegalClarity.**
https://corporatefinanceinstitute.com/resources/valuation/sweat-equity/ ; https://www.icanpitch.com/blog/sweat-equity-guide ; https://legalclarity.org/how-to-calculate-sweat-equity-formula-and-tax-rules/
*Supports:* retroactive Year-1 crediting method — sweat equity $ = hours × market rate + unreimbursed expenses, with a risk uplift of 1.5×–3× on foregone salary (design uses 2×, the Slicing Pie mid-point); tax warning that stock for past services is compensation at FMV (flagged for counsel).
*Strength:* **O**.

**C9. Clerky, "Customary stock vesting terms for startup founders"; Cooley GO, "Founder's Stock, Vesting and Founder Departures."**
https://help.clerky.com/article/1736-what-are-customary-stock-vesting-terms-for-startup-founders ; https://www.cooleygo.com/founder-basics-founders-stock/
*Supports:* the mainstream alternative for retroactive credit — backdating the vesting commencement date up to ~1 year where work is demonstrable; deemed-vesting credit at Series A re-vesting. The design uses this for the founder set-asides.
*Strength:* **L/D** (customary-terms description by top formation platforms).

**C10. Noam Wasserman, "Is Dead Equity Crippling Your Company?" (Inc.com).**
https://www.inc.com/noam-wasserman/the-dead-equity-problem.html
*Supports:* dead-equity magnitude (733 tech startups; average dead equity tripled ~$480K → >$1.5M, 2008–2011) and the 65%-of-failures-from-people-problems figure; grounds the design's use-it-or-lose-it forfeiture into the active pool.
*Strength:* **D** (descriptive, by an academic, non-peer-reviewed venue).

**C11. Carta co-founder departure data via SaaStr, "The Brutal Math of Co-Founder Breakups" (22,352 founders, Q1 2016–Q2 2023).**
https://www.saastr.com/carta-co-founder-break-ups-are-accelerating
*Supports:* departure base rates justifying vesting machinery: ~23% of co-founders gone by year 3, ~30% by year 5, ~40% by year 8; danger zone years 2.5–4.
*Strength:* **D** (platform-selected sample, secondary reporting).

**C12. Carta Founder Ownership Reports 2025/2026 & equity-split trends 2024.**
https://carta.com/data/founder-ownership/ ; https://carta.com/data/founder-ownership-2026/ ; https://carta.com/data/founder-equity-split-trends-2024/
*Supports:* benchmark cap-table shapes (median founding-team ownership 56.2% post-seed, 36.1% post-Series A; 45.9% of two-founder teams split equally in 2024, up from 31.5% in 2015; in 3–5-founder teams the lead founder typically holds ≥10 pp more than the next founder). Presented in the design as the **tension** with C6: equal splits correlate with worse outcomes yet are increasingly common.
*Strength:* **D**.

**C13. Investor view of dead equity — ISA Ventures; Equity Matrix "Dead Equity: The Silent Killer of Startups."**
https://isaventures.substack.com/p/dead-equity-on-your-cap-table-is ; https://equitymatrix.io/blog/dead-equity-kills-startups ; https://equitymatrix.io/resources/dead-equity
*Supports:* the ~10%-dead-equity red-flag rule of thumb (folklore, not measured — labeled as such in the design) and the prescription of universal vesting + pre-agreed buybacks.
*Strength:* **O**.

**C14. Leaver-provision machinery — Osborne Clarke; Ashfords; Goodvernance; OpenForest.**
https://www.osborneclarke.com/insights/vc-focus-uk-term-sheets-explained-founders-leaver-provisions-and-founders-interests ; https://www.ashfords.co.uk/insights/blog/leaver-provisions-balancing-founder-fairness-and-company-protection ; https://www.goodvernance.com/goodfounders/good-leaver-vs-bad-leaver ; https://www.openforest.co/articles/co-founder-exit-shareholder-agreement
*Supports:* good-leaver/bad-leaver definitions (good: keep vested or FMV buyback; bad: repurchase at nominal/cost incl. vested in aggressive versions; unvested always forfeits) and shotgun-clause mechanics — the design adopts the leaver matrix but rejects shotguns (see G-section fairness critique).
*Strength:* **L**.

**C15. Idea premium & contribution-type valuation — HBR "The Founder's Dilemma" (Wasserman, Feb. 2008) + practitioner surveys (ICanPitch, Failory, Cleveroad, UX Continuum).**
https://hbr.org/2008/02/the-founders-dilemma ; https://learn.icanpitch.com/blog/equity-split-technical-vs-business-cofounder/ ; https://www.failory.com/blog/how-to-split-equity ; https://www.cleveroad.com/blog/technical-co-founder-equity/ ; https://uxcontinuum.com/blog/startup-cto/startup-cto-equity-what-is-fair-2026
*Supports:* the observed 10–15 pp "idea premium" (Wasserman data) vs. Slicing Pie's deliberate zero-premium stance; practitioner claims of ~5–10 pp premiums for scarce technical depth (soft, partly inconsistent with Carta's equal-split data — labeled soft in the design). The design's resolution: price the work at market rates, no idea premium, and present this as an explicit doctrinal choice.
*Strength:* **PR-X** (HBR/Wasserman) / **O** (blogs).

## Section D. Employee & advisor equity benchmarks; academic-advisor issues

**D1. Carta, "How much equity should I give early employees?"**
https://carta.com/learn/startups/compensation/employee-equity/
*Supports:* hire-order medians (fully diluted, 4y/1y-cliff): #1 1.50% (IQR 0.50–4.00%), #2 0.85%, #3 0.50%, #4 0.44%, #5 0.33%, #6–10 ≤~0.3%; median grants to the first 10 hires consume <5% of the cap table. Anchors the design's check that the Contribution Pool is generous relative to market.
*Strength:* **D**.

**D2. SaaStr, "How Much Equity to Give Your First Employees: The Real Data from 50,000 Startups" (Carta Winter-2025 State-of-Seed data).**
https://www.saastr.com/how-much-equity-to-give-your-first-employees-the-real-data-from-50000-startups
*Supports:* corroboration of D1's curve from the 50,000-startup dataset.
*Strength:* **D** (secondary).

**D3. Index Ventures, "Rewarding Talent" handbook + OptionPlan tool (20,000+ grants, 1,650+ startups).**
https://www.indexventures.com/rewarding-talent/ ; https://www.indexventures.com/rewarding-talent/allocation-considerations-and-benchmarks ; https://www.indexventures.com/rewarding-talent/option-grants-at-series-a ; https://www.indexventures.com/optionplan/
*Supports:* ESOP trajectory (~12% at Series A → 16% by Series C for successful European startups; US all-hires-get-options norm); VP-level 0.3–0.8% at Series A.
*Strength:* **D**.

**D4. Holloway Guide to Equity Compensation, "Typical Employee Equity Levels" (+ Leo Polovets, "Analyzing AngelList Job Postings, Part 2").**
https://www.holloway.com/g/equity-compensation/sections/typical-employee-equity-levels ; https://www.codingvc.com/p/analyzing-angellist-job-postings-part-2-salary-and-equity-benchmarks
*Supports:* hires #1–5 ≈0.5–2%, #6–20 ≈0.1–0.5%; first engineer median ~1%. (2014-era AngelList data — cross-checked against D1 for currency.)
*Strength:* **D** (moderate sample, dated).

**D5. Carta, "Option Pool: How to Size Your Employee Option Pool."**
https://carta.com/learn/startups/equity-management/option-pool/
*Supports:* median seed option pool ~12.5% (Q4 2023); Series A refresh toward ~10% unallocated (15–20% total); the folk "10–20%" band's empirical center is lower than 20%. Basis for the design's 12% Future Pool.
*Strength:* **D**.

**D6. Carta, "State of Startup Compensation" H1 2025 / H2 2025 + AI-engineer deep-dive.**
https://carta.com/data/startup-compensation-h1-2025/ ; https://carta.com/data/startup-compensation-h2-2025/ ; https://carta.com/data/q2-compensation-ai-engineers/
*Supports:* current trend data — median IC initial equity +11% over two years; AI/ML engineer median initial grant +31% (Jan 2024–Feb 2026); relevant to retaining this team's engineers.
*Strength:* **D**.

**D7. Pave — Market Data Lite / VCECS executive-compensation report.**
https://www.pave.com/products/market-data-lite ; https://www.pave.com/blog-posts/unpacking-paves-vcecs-executive-compensation-report
*Supports:* founding senior engineer equity in US Tier-1 markets: median 0.33%, p75 0.62%, p90 1.24% (figures via secondary reporting — confirm in-tool).
*Strength:* **D** (with caveat).

**D8. Founder Institute FAST agreement (v2 matrix; v3 June 2026).**
https://fi.co/fast ; https://fi.co/insight/the-founder-institute-s-standard-advisor-agreement-for-startups-fast
*Supports:* the normative advisor matrix — 0.15%–1.00% by stage × engagement (Expert/~20 hrs-mo at startup stage: 0.80%; Strategic/~10 hrs-mo: 0.40%), 2-year monthly vesting (v3: 3-month cliff). Anchor for the professor's grant.
*Strength:* **O** (normative template, hugely adopted).

**D9. Carta, "Startup Advisors: How to Build Your Advisory Board" (H1 2024 benchmarking).**
https://carta.com/learn/startups/founding-team/advisor/
*Supports:* *measured* advisor medians are far below FAST norms — pre-seed 0.21%, seed 0.12%, Series A 0.05%; only ~10% of pre-seed advisors get ≥1%; 24-month monthly vesting, no cliff, single-trigger acceleration common. The design presents the FAST-vs-Carta disagreement openly.
*Strength:* **D** (medians via secondary aggregation — confirm on final open).

**D10. Holloway Guide, "Typical Startup Advisor Equity Levels."**
https://www.holloway.com/g/equity-compensation/sections/typical-startup-advisor-equity-levels
*Supports:* 0.2%–1.0% band; ~1% justified only for "highly desired candidates with strong track records" — the marquee-name case.
*Strength:* **O**.

**D11. Bruce Booth (Atlas Venture), "Biotech Scientific Advisory Boards: What Works, What Doesn't" (2012).**
https://lifescivc.com/2012/09/biotech-scientific-advisory-boards-what-works-what-doesnt/
*Supports:* professor-advisor norms — $2,500–$5,000/day cash + 0.1%–0.3% equity typical; marquee academics command more but sub-1% remains the norm at funded companies. (2012 — cash rates need re-anchoring; equity band stable per D9/D12.)
*Strength:* **O** (credible domain expert).

**D12. Advisor-benchmark aggregators (2025–26): Equity Matrix; Pitching Angels.**
https://equitymatrix.io/blog/how-much-equity-for-advisors ; https://pitchingangels.com/2021/08/09/startup-advisor-compensation/
*Supports:* corroboration that 0.15–1% and 24-month/no-or-short-cliff vesting remain current practice.
*Strength:* **O**.

**D13. Yale University Conflict of Interest Policy (Provost's COI Committee; COI Office).**
https://research-support.yale.edu/research-compliance-regulatory-affairs/conflict-of-interest-office/policies-procedures-guidance ; policy PDF: https://research-support.yale.edu/sites/default/files/2025-03/coi_policy_0.pdf ; https://provost.yale.edu/committees/conflict-interest-committee
*Supports:* the professor's obligations — annual disclosure (mandatory for >50% appointments), ad hoc updates, Provost prior approval before board seats (esp. where the startup involves his IP), management plans.
*Strength:* **P** (institutional policy).

**D14. Yale External Professional Activities Guidance (Faculty Handbook § XX.E).**
https://provost.yale.edu/policies/external-professional-activities-guidance
*Supports:* the **one-day-in-seven consulting cap** — the professor's total advisor commitment must fit inside it; no salaried outside employment while full-time at Yale. Hard constraint on his role design.
*Strength:* **P**.

**D15. Yale Patent Policy + 2022 royalty-sharing changes (Yale Ventures).**
https://ventures.yale.edu/sites/default/files/2023-03/Yale_Patent_Policy.pdf ; https://ventures.yale.edu/yale-technologies/patent-policy-for-faculty ; https://provost.yale.edu/news/important-changes-patent-royalty-sharing-practices
*Supports:* inventions in the professor's Yale research scope belong to Yale (license, don't assign); tiered inventor royalty share (50%/40%/30%); equity in spinouts negotiated through Yale startup licenses. Grounds the design's narrow IP-assignment scoping.
*Strength:* **P**.

**D16. Yale Ventures Consulting Guidance + Innovation & Commercialization Primer.**
https://ventures.yale.edu/programs/consulting-guidance ; https://ventures.yale.edu/innovation-and-commercialization-primer
*Supports:* "Faculty as Advisors" model (advisor, not operating executive); Yale Ventures reviews consulting-agreement IP clauses; publication rights stay with the university.
*Strength:* **P**.

**D17. Northwestern COI guidelines for faculty startups + use-of-students memo (comparator best practice).**
https://www.northwestern.edu/coi/policy/guidelines-for-navigating-coi-issues-when-faculty-start-up-companies-engage-in-university-research.html ; https://www.northwestern.edu/coi/docs/use-of-students-in-startups-and-consulting.pdf
*Supports:* the design's rule that no Yale students may work for the company without written university-approved agreements (Northwestern requires signed Student-Faculty Agreements with annual verification).
*Strength:* **P** (comparative policy).

**D18. Cooley GO, "Engaging Advisors from Universities and Research Institutes" + "Advisors' Concerns: IP."**
https://www.cooleygo.com/engaging-advisors-from-universities-and-research-institutes-what-you-should-know/ ; https://www.cooleygo.com/advisors-concerns-ip/
*Supports:* narrow present-assignment IP language scoped to non-university work; expect university rider terms; verify the advisor's disclosure was actually made; two-way contamination risk (company CI into the lab; university IP into the company breaking chain of title at diligence).
*Strength:* **L**.

**D19. Academic Entrepreneurship for Medical and Health Sciences (open-access, peer-reviewed): COI chapter + IP chapter.**
https://academicentrepreneurship.pubpub.org/pub/r71twlze ; https://academicentrepreneurship.pubpub.org/pub/4lgr8i84
*Supports:* structural COI categories for faculty advisors (financial, research-steering, trainee conflicts); disclosure + management plans, not prohibition, as the standard mitigation.
*Strength:* **PR-X**.

**D20. Peer-reviewed role-conflict literature: Nature Humanit. Soc. Sci. Commun. (2025) role conflicts of academic entrepreneurs; Bae et al. (2026); Higher-education systematic review (2021).**
https://www.nature.com/articles/s41599-025-04800-4 ; https://doi.org/10.1177/23409444261456302 ; https://www.tandfonline.com/doi/full/10.1080/03075079.2021.1896805
*Supports:* publication-norms-vs-confidentiality as the most consistent tension; role separation (which a well-scoped advisor agreement operationalizes) as the effective coping strategy.
*Strength:* **PR-X**.

**D21. University publication-clause norms — UT System checklist; Harvard OSP; Stanford openness policy.**
https://www.utsystem.edu/offices/general-counsel/intellectual-property/intellectual-property-checklists/pub-clause-checklist-sponsored-researchand-clinical-trial-agreements ; https://osp.finance.harvard.edu/publications-0 ; https://doresearch.stanford.edu/policies/research-policy-handbook/conduct-research/openness-research
*Supports:* the design's publication terms for the professor: 30–60-day pre-submission review, patent-filing delay ≤90 additional days (≤180 total), excision of company confidential information only — never a veto.
*Strength:* **P** (institutional templates).

## Section E. Massachusetts law

**E1. M.G.L. c. 156C, § 63 (duties expanded/restricted by operating agreement).**
https://malegislature.gov/Laws/GeneralLaws/PartI/TitleXXII/Chapter156c/Section63
*Supports:* the operating agreement may "expand or restrict" member/manager duties (no Delaware-style "eliminate" language); good-faith-reliance safe harbor. Foundation of the design's tailored-duties article.
*Strength:* **P**.

**E2. M.G.L. c. 156C, §§ 24–25 (management), § 36 (resignation).**
https://malegislature.gov/Laws/GeneralLaws/PartI/TitleXXII/Chapter156c/Section24 ; https://malegislature.gov/Laws/GeneralLaws/PartI/TitleXXII/Chapter156c/Section36
*Supports:* member-management default; manager exclusivity when managers exist; **non-waivable member resignation on ≥6 months' written notice** (agreement controls only the economics of exit); **no statutory expulsion mechanism** — expulsion exists only if the operating agreement creates it. Directly drives the design's dissociation/expulsion article.
*Strength:* **P**.

**E3. M.G.L. c. 156C, § 40 (charging orders), § 44 (judicial dissolution).**
https://law.justia.com/codes/massachusetts/part-i/title-xxii/chapter-156c/section-40/ ; https://codes.findlaw.com/ma/part-i-administration-of-the-government-ch-1-182/ma-gen-laws-ch-156c-sect-44/
*Supports:* creditor rights limited to assignee status; § 44 "not reasonably practicable" dissolution as the deadlock end-state the design's dispute ladder is built to avoid.
*Strength:* **P**.

**E4. Donahue v. Rodd Electrotype Co., 367 Mass. 578 (1975).**
https://law.justia.com/cases/massachusetts/supreme-court/1975/367-mass-578-2.html
*Supports:* "utmost good faith and loyalty" among close-entity owners; equal-opportunity rule for insider repurchases — why the design's buyback provisions must be uniform across members.
*Strength:* **P** (landmark SJC).

**E5. Pointer v. Castellani, 455 Mass. 537 (2009).**
https://caselaw.findlaw.com/court/ma-supreme-judicial-court/1501060.html
*Supports:* freeze-out via termination of a member's employment is actionable; legitimate-business-purpose + less-harmful-alternative test — governs how the design handles removing inactive founders from roles.
*Strength:* **P** (SJC).

**E6. Allison v. Eriksson, 479 Mass. 626 (2018).**
https://caselaw.findlaw.com/court/spr-jud-crt-mas-suf/1896955.html ; https://www.massbar.org/publications/ejournal/ejournal-article/section-review-2019-may-june-2019/em-allison-v.-eriksson-em-remedies-available-to-minority-llc-members-in-freeze-out-mergers
*Supports:* Donahue duties reach closely held LLCs; equitable remedies beyond appraisal for freeze-out mergers; courts enforce operating-agreement-expanded duties.
*Strength:* **P** (SJC).

**E7. Boston Bar Association, "Fiduciary Duties in Massachusetts and Delaware Closely Held Corporations"; Romano Law waiver explainer.**
https://bostonbar.org/journal/fiduciary-duties-in-massachusetts-and-delaware-closely-held-corporations/ ; https://www.romanolaw.com/can-fiduciary-obligations-be-waived-in-massachusetts/
*Supports:* MA permits expansion/restriction with specificity but blanket elimination is untested-to-doubtful (vs. 6 Del. C. § 18-1101(c)); why the design *restricts* duties for defined competitive activities rather than attempting elimination.
*Strength:* **L**.

**E8. M.G.L. c. 149, §§ 148, 150 (Wage Act).**
https://malegislature.gov/Laws/GeneralLaws/PartI/TitleXXI/Chapter149/Section148 ; https://codes.findlaw.com/ma/part-i-administration-of-the-government-ch-1-182/ma-gen-laws-ch-149-sect-150/
*Supports:* the design's top-priority legal flag — weekly/bi-weekly pay requirement, same-day pay on discharge, personal liability of officers/agents with management authority, void "special contracts," mandatory treble damages + fees, 3-year lookback, AG filing prerequisite.
*Strength:* **P**.

**E9. Reuter v. City of Methuen, 489 Mass. 465 (2022).**
https://law.justia.com/cases/massachusetts/supreme-court/2022/sjc-13121.html
*Supports:* treble damages = 3× the late wages themselves, strict liability, no good-faith or cure defense — late back-pay does not erase exposure.
*Strength:* **P** (SJC).

**E10. Segal v. Genitrix, LLC, 478 Mass. 551 (2017).**
https://law.justia.com/cases/massachusetts/supreme-court/2017/sjc-12291.html ; https://www.morse.law/news/board-members-investors-found-not-liable-under-ma-wage-act/
*Supports:* Wage Act personal liability turns on functional management authority (president/treasurer/managing officers or agents), applies to LLCs; passive board members/investors not liable — informs which founders carry personal exposure.
*Strength:* **P** (SJC).

**E11. Stanton v. Lighthouse Financial Services, 621 F. Supp. 2d 5 (D. Mass. 2009) + MBA deferred-comp survey; Steffans Legal on LLC equity-holder employees.**
https://www.gordonllp.com/blog/agreements-to-defer-salary-violate-the-wage-act/ ; https://www.massbar.org/publications/section-review/section-review-article/section-review-2021-november-december-2021/the-pandemic-wages-and-deferred-compensation-a-survey-of-applicable-law ; https://www.steffanslegal.com/blog/shareholder-of-massachusetts-llc-permitted-to-bring-claim-under-massachusetts-wage-act
*Supports:* salary-deferral agreements are void; a founder-president is a protected employee; equity promises don't extinguish wage obligations; an LLC equity holder in an employee role can still sue under the Wage Act.
*Strength:* **P** (federal district court) + **L**.

**E12. M.G.L. c. 149, § 148B (ABC test) + AG Advisory 2008/1.**
https://mass.gov/info-details/massachusetts-law-about-independent-contractors ; https://www.mass.gov/doc/attorney-generals-advisory-on-the-independent-contractor-law/download
*Supports:* presumption of employment; prong B (outside the usual course of business) makes "contractor" labels fail for core-work contributors — the design does not use contractor relabeling.
*Strength:* **P**.

**E13. M.G.L. c. 151, § 1 ($15.00/hr minimum wage); 454 CMR 27.00; no-volunteers-at-for-profits (DOL Fact Sheet 71; Skoler Abbott on MA interns).**
https://law.justia.com/codes/massachusetts/part-i/title-xxi/chapter-151/section-1/ ; https://www.mass.gov/regulations/454-CMR-2700-minimum-wage ; https://www.dol.gov/agencies/whd/fact-sheets/71-flsa-internships ; https://www.mondaq.com/unitedstates/employee-benefits-compensation/344354/massachusetts-law-on-interns-even-tougher-than-federal-rules
*Supports:* $15/hr floor with treble damages; there is no lawful volunteer status at a for-profit; MA trainee exemption effectively nonprofit-only — the "everyone unpaid" status violates c. 151 independent of § 148 timing.
*Strength:* **P** + **L**.

**E14. Practitioner synthesis on unpaid startup workers — masswagelaw.com (Gould P.C.); The Startup Law Blog "The Deferred Salary Trap."**
https://masswagelaw.com/startup-companies-and-unpaid-wages/ ; https://masswagelaw.com/delaying-or-deferring-wages-is-illegal/ ; https://www.thestartuplawblog.com/deferred-salary-trap/
*Supports:* the only compliant paths — pay minimum wage on schedule, or make the worker a bona fide member/partner (real ownership, real governance rights, distribution risk, no employee-type control); labels don't work. Basis of the design's "Member-Partner conversion" recommendation, flagged to counsel.
*Strength:* **L** (consistent across plaintiff- and company-side firms).

**E15. M.G.L. c. 149, § 24L (Massachusetts Noncompetition Agreement Act, 2018) + Beck Reed Riden guide + garden-leave ambiguity analyses.**
https://codes.findlaw.com/ma/part-i-administration-of-the-government-ch-1-182/ma-gen-laws-ch-149-sect-24l/ ; https://beckreedriden.com/the-massachusetts-noncompetition-agreement-act-massachusetts-general-laws-c-149-s-24l/ ; https://faircompetitionlaw.com/2025/08/25/massachusetts-noncompete-garden-leave/
*Supports:* garden leave (≥50% of highest 2-year salary) or mutually-agreed consideration; 12-month cap; unenforceable against non-exempt employees (which unpaid workers are); sale-of-business and nonsolicit/NDA exclusions — why the design uses nonsolicits + NDAs + forfeiture conditions, not noncompetes.
*Strength:* **P** + **L** (Beck was a principal drafter of the Act).

**E16. Miele v. Foundation Medicine, Inc., 495 Mass. 683 (SJC, June 13, 2025).**
https://caselaw.findlaw.com/court/ma-supreme-judicial-court/117388316.html ; https://bostonbar.org/journal/restrictive-covenants-and-forfeiture-provisions-after-miele-v-foundation-medicine-inc/
*Supports:* forfeiture tied to breach of a nonsolicit is outside § 24L — validating the design's equity-forfeiture-teeth approach. (Reporter cite as reported; counsel to confirm.)
*Strength:* **P** (SJC 2025).

**E17. SEC Rule 701 for LLC issuers (SEC small-business page; Pillsbury guide) — see also A10.**
https://www.sec.gov/resources-small-businesses/exempt-offerings/employee-benefit-plans-rule-701-0 ; https://www.pillsburylaw.com/a/web/4960/SecuritiesOfferingstoEmployeesConsultantsandAdvisorsUnderRule701.pdf
*Supports:* Rule 701 availability to LLCs for compensatory grants to employees, managers, and natural-person consultants/advisors; caps and $10M disclosure trigger; no state preemption.
*Strength:* **P** + **L**.

**E18. Massachusetts blue sky — M.G.L. c. 110A, § 402; 950 CMR 14.402(B)(13); Form D notice filing.**
https://malegislature.gov/Laws/GeneralLaws/PartI/TitleXV/Chapter110A/Section402 ; https://www.law.cornell.edu/regulations/massachusetts/950-CMR-14-402 ; https://blog.fincompliance.io/post/2025/04/15/sec-form-d-blue-sky-filing-requirements-and-fees-by-state
*Supports:* MA compensatory-plan exemption paralleling Rule 701 (covers consultants/contractors); Rule 506(b) covered-security preemption with Form D notice to MA within 15 days of first sale + $300 fee.
*Strength:* **P**.

## Section F. Founder equity splits, conflict, and vesting — outcome literature

**F1. Hellmann & Wasserman, "The First Deal: The Division of Founder Equity in New Ventures," Management Science 63(8): 2647–2666 (2017).** *(same study as C6; listed here with the outcome findings)*
https://pubsonline.informs.org/doi/10.1287/mnsc.2016.2474 ; https://www.nber.org/papers/w16922 ; free PDF: https://www.nber.org/system/files/working_papers/w16922/w16922.pdf ; HBS working-paper PDF: https://www.hbs.edu/ris/Publication%20Files/14-085_2bd67a49-bd41-4396-a69d-73a7f40829b8.pdf ; NBER Digest: https://www.nber.org/digest/aug11/division-founder-equity-new-ventures
*Supports:* ~⅓ of teams split exactly equally; equal splits — especially "quick handshake" splits negotiated in under a day — are associated with lower first-round pre-money valuations and lower fundraising likelihood; the authors attribute this to *selection* (teams that avoid the hard conversation are weaker), not causation. This is why the design forces a structured, criteria-based split process rather than banning equal outcomes.
*Strength:* **PR-X** (explicitly correlational/selection).

**F2. Wasserman, "The Throne vs. the Kingdom: Founder Control and Value Creation in Startups," Strategic Management Journal 38(2): 255–277 (2017).**
https://sms.onlinelibrary.wiley.com/doi/abs/10.1002/smj.2478 ; free PDF: https://msbfile03.usc.edu/digitalmeasures/nwasserm/intellcont/Wasserman-2017-Strategic_Management_Journal-1.pdf
*Supports:* 6,130 startups; each additional level of retained founder control (board and/or CEO) associated with 17.1–22.0% lower pre-money valuation — grounds for the design's non-founder-controlled board trajectory and independent seat.
*Strength:* **PR-X** (large sample; selection concerns acknowledged by author).

**F3. Wasserman, "Founder-CEO Succession and the Paradox of Entrepreneurial Success," Organization Science 14(2): 149–172 (2003).**
https://pubsonline.informs.org/doi/10.1287/orsc.14.2.149.14995 ; author PDF: https://www.noamwasserman.com/nwasserman/Founder-CEO_Succession-OrgScience.pdf
*Supports:* succession is structurally normal — replacement hazard rises after product completion and each financing round; most successions are board/investor-initiated. Why the design pre-agrees CEO evaluation and removal mechanics now.
*Strength:* **PR-X**.

**F4. Wasserman, The Founder's Dilemmas (Princeton UP, 2012) + "The Founder's Dilemma," HBR Feb. 2008 + "Splitting the Pie" (author blog, 2020).**
https://hbr.org/2008/02/the-founders-dilemma ; https://www.hbs.edu/faculty/Pages/item.aspx?num=42425 ; https://www.noamwasserman.com/splitting-the-pie-founding-team-equity-splits/ ; http://www.startuplessonslearned.com/2012/04/founders-dilemmas-equity-splits.html
*Supports:* ~10,000-founder dataset — 73% of teams split within the first month, mostly statically; ~65% of high-potential startup failures attributed to people problems (interpretive attribution, not causal; derivation opaque — treated as directional); <25% of founder-CEOs lead through IPO; ~50% of founders out of the CEO seat by year 3 (212-startup analysis); non-negotiated equal splitters ~3× more likely to be unhappy with their split.
*Strength:* **PR-X / D** (mixed; the 65% figure flagged as directional).

**F5. Breugst, Patzelt & Rathgeber, "How Should We Divide the Pie? Equity Distribution and Its Impact on Entrepreneurial Teams," Journal of Business Venturing 30(1): 66–94 (2015).**
https://www.sciencedirect.com/science/article/abs/pii/S0883902614000676
*Supports:* *perceived justice* of the split — not equality per se — drives positive/negative team interaction spirals (8 teams, 6 months, qualitative). Why the design invests in transparent process (published formula, peer certification, audit rights) as much as in the numbers.
*Strength:* **PR-X** (small-N, theory-building).

**F6. Ruef, Aldrich & Carter, "The Structure of Founding Teams," American Sociological Review 68(2): 195–222 (2003).**
https://journals.sagepub.com/doi/abs/10.1177/000312240306800202
*Supports:* teams form by homophily and strong ties, not complementary skills (representative PSED sample) — the structural reason friendly five-founder teams avoid hard conversations until they fester; argues for formalizing governance early.
*Strength:* **PR-X** (representative sample).

**F7. Hellmann & Thiele, "Contracting Among Founders," Journal of Law, Economics, & Organization 31(3): 629–661 (2015).**
https://academic.oup.com/jleo/article-abstract/31/3/629/808939 ; https://papers.ssrn.com/sol3/papers.cfm?abstract_id=1968696
*Supports:* the main theoretical justification for founder vesting: contingent contracts with vesting mitigate team-formation inefficiencies under skill uncertainty.
*Strength:* **PR** (formal theory, no data).

**F8. Hellmann, Schure, Tergiman & Vo, "Ownership Dynamics within Founder Teams: The Role of External Financing," Strategic Entrepreneurship Journal 13(3): 256–287 (2019).**
https://sms.onlinelibrary.wiley.com/doi/abs/10.1002/sej.1328
*Supports:* initial splits are sticky and get renegotiated mainly under financing pressure — why the design builds scheduled re-measurement (quarterly) into the system instead of relying on ad hoc renegotiation.
*Strength:* **PR-X**.

**F9. Hennicke & Mueller, "Unequal Implies Success? How Initial Ownership Split Impacts Team Entry and New Venture Performance," European Management Journal 42(3): 305–315 (2024).**
https://www.sciencedirect.com/science/article/abs/pii/S0263237322001785
*Supports:* 24,194 German startups; unequal-split ventures show ~24.5% better performance in mediation analysis, partly via openness to adding members. Presented alongside the YC/Carta counter-position (F10, C12) as a live disagreement.
*Strength:* **PR-X** (registry data; selection concerns).

**F10. Y Combinator, "How to Split Equity Among Co-Founders"; Michael Seibel, "Co-Founder Equity Mistakes to Avoid."**
https://www.ycombinator.com/blog/splitting-equity-among-founders ; https://www.ycombinator.com/library/LP-co-founder-equity-mistakes-to-avoid
*Supports:* the influential normative counter-position — default to (near-)equal splits because future execution dwarfs early contribution, paired with universal 4-year/1-year-cliff vesting (25% at month 12, 1/48 monthly) so early leavers "walk away with nothing." The design adopts YC's vesting mechanics while rejecting its equal-split default (the founders' own Fixed Requirements already reject it).
*Strength:* **O** (high-influence accelerator; normative, not data).

**F11. Cooley GO, "Founder's Stock, Vesting and Founder Departures"; CRV "Startup Equity Structure"; LTSE founder-allocation guide.**
https://www.cooleygo.com/founder-basics-founders-stock/ ; https://www.crv.com/content/startup-equity-structure ; https://ltse.com/insights/founders-guide-to-allocating-co-founder-equity
*Supports:* reverse-vesting mechanics (repurchase at cost lapsing over time), 83(b) timing, double-trigger acceleration as the investor-preferred norm, investors' expectation to (re-)impose vesting at Series A. **Honesty note:** no rigorous public statistic exists for the exact fraction of companies imposing founder vesting at incorporation — described as "expected/standard" by legal sources, not measured.
*Strength:* **L**.

**F12. CB Insights, "Why Startups Fail: Top Reasons" (483 post-mortems; recent edition 431 companies).**
https://www.cbinsights.com/research/report/startup-failure-reasons-top/ ; https://www.cbinsights.com/research/startup-failure-post-mortem/
*Supports:* the counterweight to Wasserman's 65%: founders' self-reported failure causes rank "no market need" 42% and "ran out of cash" 29% above "not the right team" 23% (multi-cause; self-report bias — founders under-report their own interpersonal failures). The design presents both and does not overclaim.
*Strength:* **D** (self-selected, self-reported).

## Section G. Governance, boards, leadership, deadlock

**G1. Garg, "Venture Boards: Distinctive Monitoring and Implications for Firm Performance," Academy of Management Review 38(1): 90–108 (2013).**
https://journals.aom.org/doi/10.5465/amr.2010.0193
*Supports:* venture boards are not mini public boards; the "principal problem" — investor-directors are interested parties; monitoring and advice functions interact on small boards. Informs the design's independent-seat rationale.
*Strength:* **PR** (theory).

**G2. Garg & Eisenhardt, "Unpacking the CEO–Board Relationship," Academy of Management Journal 60(5): 1828–1858 (2017).**
https://journals.aom.org/doi/10.5465/amj.2014.0599
*Supports:* effective venture CEOs manage boards as CEO–director dyads while retaining strategy control — practical guidance embedded in the design's CEO role description.
*Strength:* **PR-X** (inductive, small-N).

**G3. Krause, Priem & Love, "Who's in Charge Here? Co-CEOs, Power Gaps, and Firm Performance," Strategic Management Journal 36(13): 2099–2110 (2015).**
https://sms.onlinelibrary.wiley.com/doi/abs/10.1002/smj.2325
*Supports:* the single-CEO recommendation: among 71 public co-CEO pairs, performance rises with the *power gap* between co-CEOs (inverted-U) — "whatever benefits the co-CEO structure might offer likely lie outside the shared command paradigm."
*Strength:* **PR-X** (small N, public firms — external validity limited).

**G4. Feigen, Jenkins & Warendh, "Is It Time to Consider Co-CEOs?," HBR July–Aug 2022.**
https://hbr.org/2022/07/is-it-time-to-consider-co-ceos
*Supports:* the pro-co-CEO counter-evidence (87 public co-CEO firms averaged 9.5% vs. 6.9% annual shareholder return; ~60% outperformed) — presented as a disagreement with G3 and discounted for survivor/selection bias; even its success factors (clear decision rights, pre-agreed exit) concede pure shared command fails.
*Strength:* **D/O** (selection-biased sample, no controls).

**G5. Eisenhardt, "Making Fast Strategic Decisions in High-Velocity Environments," Academy of Management Journal 32(3): 543–576 (1989).**
https://journals.aom.org/doi/abs/10.5465/256434
*Supports:* the design's decision rule — "consensus with qualification": seek consensus; if it fails, the CEO decides with input. Fast deciders use more real-time information and more simultaneous alternatives.
*Strength:* **PR-X** (inductive small-N; speed→performance link propositional).

**G6. Amason & Sapienza, "The Effects of Top Management Team Size and Interaction Norms on Cognitive and Affective Conflict," Journal of Management 23(4): 495–516 (1997).**
https://journals.sagepub.com/doi/10.1177/014920639702300401
*Supports:* larger top teams generate more of *both* task conflict (useful) and personal conflict (harmful); norms of mutuality/openness tilt the balance — five founders is a large TMT and needs explicit process.
*Strength:* **PR-X**.

**G7. Haleblian & Finkelstein, "Top Management Team Size, CEO Dominance, and Firm Performance," Academy of Management Journal 36(4): 844–863 (1993).**
https://journals.aom.org/doi/abs/10.5465/256761
*Supports:* in turbulent environments larger teams do better and *dominant* CEOs do worse — the design's CEO is a tie-breaker and accountable executive, not an autocrat.
*Strength:* **PR-X**.

**G8. Klotz, Hmieleski, Bradley & Busenitz, "New Venture Teams: A Review," Journal of Management 40(1): 226–255 (2014).**
https://journals.sagepub.com/doi/abs/10.1177/0149206313493325 ; free PDF: https://www.hmieleski.com/Publications/Klotz_Hmieleski_Bradley_Busenitz_JOM_2014.pdf
*Supports:* synthesis: team composition affects outcomes through process (conflict, cohesion); equity splits and founder exits understudied — supports the design's process-heavy approach.
*Strength:* **PR** (review).

**G9. Eisenhardt & Schoonhoven, "Organizational Growth… U.S. Semiconductor Ventures, 1978–1988," Administrative Science Quarterly 35: 504–529 (1990).**
https://www.semanticscholar.org/paper/Organizational-Growth:-Linking-Founding-Team,-and-Eisenhardt-Schoonhoven/1446661cd44d1b75d90098453822e909395127a3
*Supports:* larger founding teams (4–5) with diverse experience and prior joint work built higher-growth firms — the good news for a five-founder company, conditional on managing conflict (G6).
*Strength:* **PR-X**.

**G10. Brooks, Landeo & Spier, "Trigger Happy or Gun Shy? Dissolving Common-Value Partnerships with Texas Shootouts," RAND Journal of Economics (2010).**
https://papers.ssrn.com/sol3/papers.cfm?abstract_id=1617988 ; working paper: https://sites.ualberta.ca/~econwps/2009/wp2009-01.pdf
*Supports:* the design's **rejection of shotgun clauses**: they are equitable only under symmetric information and symmetric financial capacity; a cash-poor founder is systematically exploitable (theory + lab experiments). Cash-poor founders are exactly this company's situation.
*Strength:* **PR-C** (formal theory + controlled experiments).

**G11. NVCA Model Legal Documents (+ Morgan Lewis 2024-update analysis).**
https://nvca.org/model-legal-documents/ ; https://www.morganlewis.com/pubs/2024/09/whats-new-in-the-nvca-model-legal-documents-and-whats-next
*Supports:* the reserved-matters vocabulary (protective provisions), Voting Agreement board-composition mechanics, drag-along — the template any future VC round will use; the design's internal reserved-matters list deliberately mirrors it.
*Strength:* **L** (market-standard documents).

**G12. Carta, "Board of Directors: What Founders Need to Know" (+ SaaStr seed-data summary; Glen Coyne board-composition guide).**
https://carta.com/learn/startups/private-companies/board-of-directors/ ; https://www.saastr.com/the-state-of-seed-today-10-key-learnings-from-cartas-latest-data/ ; https://www.glencoyne.com/guides/board-composition-control-terms
*Supports:* norm trajectory — seed board of 3 (2 founders + 1 investor), Series A 4–5 (2–2–1 with independent swing vote); independent directors get on average 0.78% at seed / 0.53% at Series A (Carta, March 2024).
*Strength:* **D**.

**G13. Feld, Blumberg & Ramsinghani, Startup Boards: A Field Guide (2nd ed., Wiley 2022) + Blumberg CEO-review template coverage.**
https://www.wiley.com/en-br/startup-boards-a-field-guide-to-building-and-leading-an-effective-board-of-directors-2nd-edition-p-9781119859284 ; https://tech.co/news/startup-ceo-matt-blumberg-2013-09
*Supports:* small boards weighted toward independents as companies grow; board-led CEO evaluation (annual self-assessment + 360 + objectives-based scoring with quarterly check-ins) — adopted as the design's CEO review process.
*Strength:* **O** (influential practitioner handbook).

**G14. Board observer rights — Law Insider clause library; Columbia Law Blue Sky commentary.**
https://lawinsider.com/clause/board-observer-rights ; https://clsbluesky.law.columbia.edu/2024/05/15/how-board-observers-are-improving-corporate-governance/
*Supports:* observer seats (attend + information rights, no vote, no fiduciary duties) as the tool for keeping off-board founders informed while the voting board stays small and odd.
*Strength:* **L/O**.

**G15. Conti, Jacobs & Leitess, "Deadlock-Breaking Mechanisms in LLCs — Flipping a Coin Is Not Good Enough, but Is Better Than Dissolution," ABA Business Law Today (Mar. 2017).**
https://www.americanbar.org/groups/business_law/resources/business-law-today/2017-march/deadlock-breaking-mechanisms/ ; mirror: https://businesslawtoday.org/2017/03/deadlock-breaking-mechanisms-in-llcs-flipping-a-coin-is-not-good-enough-but-is-better-than-dissolution/
*Supports:* the deadlock menu the design draws from — escalation → mandatory mediation (30–60 days) → binding arbitration; tie-breaker/casting-vote directors; deadlock-triggered put/call; rotating casting votes flagged as unsatisfying; anything beats judicial dissolution.
*Strength:* **L** (authoritative professional-body survey).

**G16. Final-offer ("baseball") arbitration — California DIR literature review; Monhait, Harvard J. Sports & Ent. Law; Coleman (1993), Industrial Relations.**
https://www.dir.ca.gov/chswc/basebalarbffinal.htm ; https://journals.law.harvard.edu/jsel/wp-content/uploads/sites/78/2013/06/Monhait.pdf ; https://onlinelibrary.wiley.com/doi/abs/10.1111/j.1468-232X.1993.tb01029.x
*Supports:* FOA's incentive for both sides to moderate and settle pre-hearing (theory strong; empirical convergence findings mixed — stated honestly); adopted for quantifiable disputes (rates, valuations, point tallies).
*Strength:* **PR-X / L** (mixed empirics, noted).

**G17. Founder-CEO vs. professional-CEO counter-literature — Lee, Kim & Bae, "Are Founder CEOs Better Innovators? Evidence from S&P 500 Firms" (Wharton Mack Institute working paper).**
https://mackinstitute.wharton.upenn.edu/wp-content/uploads/2016/03/Mahn-Lee-Joon-Kim-Jongsoo-and-Bae-Joonhyung_Are-Founder-CEOs-Better-Innovators.-Evidence-from-SP-500-Firms.pdf
*Supports:* the presented disagreement: founder-CEOs associated with higher innovation output — the literature is genuinely split on founder-vs-professional CEOs, though not on the value of outside governance. The design keeps founder-CEO by default with real board accountability.
*Strength:* **PR-X** (working paper).

**G18. Rödl & Partner, "M&A Vocabulary: Russian Roulette and Texas Shoot-Out"; Risky Business Law on Russian-roulette provisions.**
https://www.roedl.com/en/insights/ma-vocabulary-russian-roulette-and-texas-shoot-out/ ; https://www.riskybusinesslaw.com/post/what-are-russian-roulette-provisions-in-contracts-between-llc-members
*Supports:* mechanism definitions for the design's considered-and-rejected analysis of buy-sell shootouts.
*Strength:* **L**.

---

## Master honesty summary

1. **No peer-reviewed empirical validation exists for Slicing Pie or any ex-post dynamic-equity model.** Our contribution system rests on (a) the peer-reviewed finding that static handshake splits correlate with worse outcomes (F1), (b) peer-reviewed theory favoring contingent contracts (F7), and (c) practitioner mechanics (C1–C2). We manage the unvalidated part by freezing the dynamic system before any institutional financing.
2. **The equal-split literature genuinely disagrees** (F1/F9 vs. F10/C12). We do not resolve it; the founders' own fixed requirements already chose contribution-based allocation.
3. **The 65%-people-problems figure is directional, not precise** (F4 vs. F12).
4. **Founder-CEO vs. professional CEO is unresolved** (F2/F3 vs. G17). Our design is robust to either answer: founder-CEO by default, real removal machinery.
5. **Carta/Pave/Index figures are platform-selected samples**, not random samples of all startups; several specific medians arrived via secondary aggregation and are marked for confirm-on-open.
6. **URL verification was search-index-based, not click-through** (egress policy; disclosed at top).
7. **Legal citations are research, not legal advice**; reporter cites for the newest cases (e.g., Miele) need confirmation by counsel.
