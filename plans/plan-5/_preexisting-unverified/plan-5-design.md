# plan5 — Full Design: Governance & Equity Framework

**Team:** plan5 · **Branch:** `plan-5` · **Date:** August 1, 2026
**Isolation statement:** Produced on an empty orphan branch; no other team's branch or file was read, checked out, diffed, or browsed.

This document is the complete business-terms design. The article-by-article draft for counsel is in [`plan-5-operating-agreement.md`](plan-5-operating-agreement.md); the annotated bibliography with evidence-strength ratings is in [`plan-5-references.md`](plan-5-references.md).

---

## Part 0 — Sequencing: three moves, in a fixed order

The order below is driven by legal exposure and tax mechanics, not preference. Doing these out of order either compounds a wage-law violation or wastes a low-valuation tax window.

**Move 1 (immediately, weeks 0–4): Cure the Massachusetts Wage Act exposure.**
The company has ~10 unpaid employees. Under M.G.L. c. 149 §148, an employer that fails to pay wages is strictly liable for **treble damages plus attorneys' fees**, even if it later pays ([Reuter v. City of Methuen (2022); Holland & Knight](https://www.hklaw.com/en/insights/publications/2022/04/massachusetts-sjc-upends-existing-law-requires-treble-damages)). "Special contracts" in which an employee agrees to defer or waive wages for equity are **unenforceable** ([Mass. Wage Law on startups](https://masswagelaw.com/startup-companies-and-unpaid-wages/)). Liability is **personal** for the president, treasurer, and "officers or agents having the management" of the company ([Boston Bar Association](https://bostonbar.org/journal/director-liability-under-the-massachusetts-wage-act-the-supreme-judicial-court-clarifies-the-law-but-traps-may-remain-for-the-unwary/)) — which likely includes several founders individually. Note also that Massachusetts's independent-contractor statute uses the strictest "ABC" test, so relabeling employees as contractors does not work ([Bennett & Belfort](https://www.bennettandbelfort.com/practice/payment-wages-employee/)).

*Design decision:* every current unpaid contributor must, on counsel's advice, become either (a) a **bona fide member of the LLC** (an owner, not an employee — this is precisely what the Contribution Pool below does, and it is the recommended path for the current team), or (b) a paid employee at no less than minimum wage. The framework below assumes (a) for the existing 15 people; all *future* hires after the first financing are conventional salaried employees with option grants. **Counsel must bless the member-not-employee characterization for each person** (factors: genuine governance rights, profit share, no fixed "wage"); this is flagged in the operating agreement draft.

**Move 2 (weeks 2–8): The Retrospective Reckoning.**
A one-time, formula-driven allocation of Year 1 contributions under the ledger rules of Part 2, run *while the company's paper value is still low*. Tax reason: equity issued for past services is compensation; issuing capital interests (or, if counsel prefers, catch-up profits interests under [Rev. Proc. 93-27 / 2001-43](https://www.irs.gov/pub/irs-drop/rp-01-43.pdf)) at today's near-zero valuation minimizes ordinary-income exposure, whereas waiting until a financing makes the same grants expensive ([The Tax Adviser on profits interests](https://www.thetaxadviser.com/issues/2025/jan/profits-interests-the-most-tax-efficient-equity-grant-to-employees/)).

**Move 3 (weeks 8–16): Statutory conversion to a Delaware C-corporation.**
- **Investor expectation:** VCs overwhelmingly require a Delaware C-corp; conversion at the term-sheet stage adds cost and friction at the worst moment ([Startups.com](https://www.startups.com/lexicon/llc-vs-c-corp); [Flux Law conversion guide](https://www.flux.law/blog/convert-llc-to-delaware-c-corp)).
- **QSBS:** §1202 exclusion applies only to C-corp stock; LLC interests never qualify. Under the One Big Beautiful Bill Act (July 4, 2025), stock issued after that date carries a **$15M per-taxpayer exclusion cap** (up from $10M) and a tiered 50/75/100% exclusion at 3/4/5-year holds; the **holding period starts at conversion, not LLC formation** — so every month of delay is a month of lost QSBS clock ([Holland & Knight](https://www.hklaw.com/en/insights/publications/2025/08/conversion-of-partnership-and-llc-interests-into-qualified); [Millan & Co. §1202 guide](https://millancpa.com/insights/section-1202-qualified-small-business-stock-qsbs-tax-guide)). A subtle benefit of converting while cheap: the LLC's built-in appreciation at conversion counts toward §1202 basis rules in ways counsel should optimize now, not later ([FBT Gibbons](https://fbtgibbons.com/guide-to-converting-partnerships-into-c-corporation-issuers-of-qsbs-part-1/)).
- **Mechanics:** LLC units convert 1:1 into restricted common stock carrying the same earn-in/vesting overlays; recipients file **83(b) elections within 30 days**; post-conversion equity compensation runs under [Rule 701](https://www.cooleygo.com/why-private-companies-should-know-about-rule-701-options-rsas-and-rsus/) with 409A valuations.

*Why not stay an LLC?* The strongest pro-LLC argument is the tax-free flexibility of profits interests. It loses here because fixed requirement #3 (maximize investor attractiveness) is categorical, the team is 15+ people (LLC K-1s at that scale are a real cost), and the QSBS clock rewards early conversion. We say this to be honest that the LLC-longer path is *defensible* — some boutique counsel advocate it — but it is dominated on the founders' own stated priority.

---

## Part 1 — Governance

### 1.1 What the evidence says

The founders asked us not to assume a conventional answer, so we looked at the leaderless/shared/rotating options seriously. The literature splits cleanly along a line that is often missed:

- **Shared leadership as *behavior* is good.** Meta-analytically, shared leadership correlates with team effectiveness at ρ ≈ .34 across 42 samples ([Wang, Waldman & Zhang 2014](https://pubmed.ncbi.nlm.nih.gov/24188392/); confirmed with different measurement moderators by [D'Innocenzo, Mathieu & Kukenberger 2016](https://www.sciencedirect.com/science/article/abs/pii/S1048984314000691)). In new-venture top management teams specifically, *both* vertical (single-leader) and shared leadership predict revenue and employee growth, with shared leadership adding explanatory power *on top of* vertical leadership — not instead of it ([Ensley, Hmieleski & Pearce 2006](https://www.sciencedirect.com/science/article/abs/pii/S1048984306000051), samples of 66 Inc.-500 and 154 random startups).
- **Flat *structure* is bad for execution.** Using a large sample of game-development startups, Lee finds flat hierarchies improve novelty but cause "haphazard execution and commercial failure," overwhelming informal leaders and inducing power struggles ([Lee 2022, *SMJ*](https://sms.onlinelibrary.wiley.com/doi/abs/10.1002/smj.3333)). Five semi-active founders with no formalized authority is exactly the failure mode this paper describes.
- **Co-CEOs: intriguing but weak evidence.** The best-known result — 87 public co-CEO firms returning 9.5%/yr vs 6.9% for single-CEO peers ([Feigen, Jenkins & Warendh 2022, HBR](https://hbr.org/2022/07/is-it-time-to-consider-co-ceos)) — is a tiny, survivorship-biased sample of *large public companies*, not startups. We do not build on it.
- **Control-hoarding is costly.** Founders who kept both the CEO role and board control held equity stakes worth roughly half those of founders who ceded both ([Wasserman 2008, HBR "The Founder's Dilemma"](https://hbr.org/2008/02/the-founders-dilemma); [Wasserman, "Rich vs. King," Academy of Management 2006](https://www.noamwasserman.com/nwasserman/Rich_vs_King-Proceedings_with_abstract.pdf)). Correlational, but consistent with requirement #3.
- **Boards start founder-controlled and professionalize.** In a comprehensive dataset of VC-backed startup boards, formation-stage boards are entrepreneur-controlled; independents arrive around the second financing and play a documented *mediation* role in founder–investor conflict ([Ewens & Malenko, *J. Finance* 2025 / NBER w27769](https://www.nber.org/papers/w27769)). Building a conventional, expandable board now means no re-architecture at the term sheet.

**Honest limits:** everything above is correlational or qualitative; none of it is causal identification. The design therefore prefers *reversible* governance choices (annual mandates, elected seats) over irreversible ones.

### 1.2 The structure

**A single CEO with an annual, revocable mandate — merit-selected, not seniority-selected.**
- The Board appoints the CEO by majority vote after a structured internal process open to any member (founder or not). The mandate renews annually by board vote; the board may remove the CEO at any time by majority.
- The CEO is the single point of external accountability (investors, contracts, hiring within budget) and runs day-to-day operations.
- *Why not rotate?* Rotation re-imposes the coordination costs Lee (2022) documents, and signals to investors precisely the diffuse accountability that Hellmann & Wasserman associate with weaker financing outcomes. *Why not consensus?* Five founders with divergent activity levels already failed to formalize a simple agreement in a year; consensus governance has an empirical failure mode this team has personally demonstrated.

**Shared leadership, kept — at the operating level.**
A written **Decision Rights Matrix** (DACI-style) delegates domains to functional leads chosen by the CEO with board consent (e.g., product/architecture, engineering delivery, research, business development). Domain leads decide within their domain and budget; the CEO decides cross-domain conflicts; the board decides what the matrix reserves to it. This captures the measured benefits of shared leadership (Ensley et al. 2006) inside an accountable structure. The matrix itself is in the operating agreement draft, Art. V.

**Board of Managers (→ Board of Directors at conversion): 3 seats, none reserved by founder status.**
- Seat 1: the CEO, ex officio. Seats 2–3: elected annually by all members, one-unit-one-vote, plurality voting. Any member — founder or employee — may stand.
- At the first financing, expand to 5: add the investor seat the term sheet demands plus **one independent** (mediation function per Ewens & Malenko).
- *Why elected, not founder-reserved?* Requirement #2 puts founders and employees on identical terms for everything outside the 25% reserved pool; a founder-status board seat would rebuild the status hierarchy the founders decided to dismantle. It also directly mitigates the dead-equity/inactive-founder problem: authority follows current contribution and unit-weighted support, not history.
- One-unit-one-vote, no dual-class: supervoting founder shares at this stage are an investor red flag and inconsistent with requirement #2 ([Carta on founder shares](https://carta.com/learn/startups/equity-management/founder-shares/)).

**Reserved matters — supermajority of units (66⅔%):** amending the operating agreement; issuing equity outside the adopted pools/plan; changing the Rate Table or multipliers; merger, sale, or dissolution; related-party transactions above $10,000; conversion to C-corp terms (the conversion itself is pre-authorized in the OA at these terms); admitting new members outside the plan. **Board majority:** annual budget; hiring/removing officers; any expenditure > $25,000 outside budget; adopting the annual Decision Rights Matrix. **CEO:** everything else, within budget.

**Contribution Committee: 3 members — administers the ledger.**
Elected annually by unit vote; at least one seat must be held by a non-founder. Runs the quarterly ledger cycle (Part 2), rules on classification disputes, applies the impact kicker with recusal rules. Appeals go to the dispute ladder (§1.3).

### 1.3 Disputes and deadlock

Tiered, cheap-to-expensive, per standard closely-held-company practice:
1. **Notice + good-faith negotiation** (14 days).
2. **Mediation** — AAA or JAMS, Boston (30 days).
3. **Binding arbitration** — AAA Commercial Rules, Boston; internal-affairs governing law is Massachusetts now, Delaware after conversion (counsel to confirm forum interplay).
4. **Board deadlock** (only possible post-expansion with an even board or 40%+ unit-block impasse on reserved matters lasting >90 days): the independent director convenes a resolution conference; failing that, either bloc may trigger the **separation mechanism**.
5. **Separation mechanism — sealed-bid auction, not a shotgun.** Both sides submit sealed per-unit bids; the higher bidder buys the other out at the *higher* bid. We reject the classic shotgun/Texas-shootout deliberately: it systematically favors the party with more cash or information, a flaw documented across the business-divorce literature ([KPPB Law](https://www.kppblaw.com/can-shotgun-clauses-save-or-sink-your-llc-or-corporation-a-closer-look-at-this-legal-tool/); [Weiner Law](https://www.weiner.law/nj-law-blog/shotgun-agreements-and-other-methods-to-break-deadlock/)) — and in this company, cash positions are certain to be unequal. A sealed-bid auction preserves the price-discovery benefit while reducing the wealth-asymmetry weaponization. [Counsel: confirm enforceability and financing-window mechanics; consider an appraisal-based put/call as fallback.]

---

## Part 2 — Equity

### 2.1 Architecture (adds to 100%)

| Pool | Size | Who | Mechanism |
|---|---|---|---|
| Founder Reserved Pool | 25.0% | The 5 founders, 5% each cap | 16-quarter earn-in with activity gate (use-it-or-lose-it) |
| Advisor Pool | 1.0% | The professor + future advisors | FAST-benchmarked grants, 2-yr vest, 3-mo cliff |
| Contribution Pool | 74.0% | Founders AND employees, identical terms | Unit ledger: retroactive tranche + quarterly dynamic tranches until the Crystallization Event |

After the Crystallization Event (first priced financing ≥ $1M, or the C-corp conversion if the board so elects), the dynamic system freezes into fixed shares and the company moves to conventional compensation: salaries plus a new option pool sized to market (median seed pool ≈ 12.5% of post-money per [Carta data](https://carta.com/learn/startups/equity-management/option-pool/); pools of 10–15% are the U.S. norm). Sunsetting the dynamic model at the first financing is also the standard recommendation of the dynamic-equity literature itself ([Slicing Pie Handbook](https://slicingpie.com/wp-content/uploads/2016/09/Slicing-Pie-Handbook-FREE-SAMPLE.pdf)) and avoids the fixed-cap-table conversion problem practitioners flag ([Equity Matrix](https://equitymatrix.io/blog/slicing-pie-problems)).

### 2.2 The Founder Reserved Pool — earned, not granted

Each founder's 5% divides into **16 quarterly tranches of 0.3125%**, spanning 4 years from company formation (so four tranches are already in the past and are resolved in the Reckoning). A tranche is earned only if the founder met the **Activity Gate** in that quarter:

> **Activity Gate:** ≥ 390 verified contribution-hours in the quarter (≈30 h/week), **or** ledger points ≥ 75% of the median points of the five most active contributors (founder or employee) that quarter.

- A missed quarter's tranche **cancels permanently** and its equity reverts to the Contribution Pool. No make-ups, no banking. This is the fixed requirement "use it or lose it, not a guarantee," implemented at quarterly granularity so that a founder who is inactive for a year loses 1.25%, not everything and not nothing.
- Departure (voluntary or removal for cause) cancels all future tranches.
- The 4-year/quarterly structure mirrors the near-universal market vesting standard (4 years, cliff-style gating; ≥95% of cliffs are one year, and 4/1 is what investors expect to see — [Carta](https://carta.com/learn/equity/stock-options/vesting/), [Crowley Law](https://www.crowleylawllc.com/founder-equity-vesting-guide/)), so no investor re-education is needed.
- *Why time+activity rather than pure time?* Pure time-vesting would let an inactive founder collect the reserved pool by waiting — exactly the "dead equity" pattern VCs treat as a red flag when ≥10% of the cap table is held by non-contributors ([Perkins Coie](https://perkinscoie.com/insights/blog/dealing-dead-equity); [ISA Ventures](https://isaventures.substack.com/p/dead-equity-on-your-cap-table-is)).

### 2.3 The Contribution Pool — the ledger

**Design lineage and honesty about it.** The ledger adapts the Slicing Pie dynamic-equity model ([Moyer](https://slicingpie.com/wp-content/uploads/2016/09/Slicing-Pie-Handbook-FREE-SAMPLE.pdf)) — the most widely used practitioner framework for exactly this situation (bootstrapped, unpaid, unequal contributions). It has **no peer-reviewed outcome evidence**; our confidence in it rests on (a) the fairness-perception literature showing that perceived injustice in splits poisons teams ([Breugst et al. 2015](https://www.sciencedirect.com/science/article/abs/pii/S0883902614000676)) and dynamic transparent ledgers are engineered for perceived procedural justice, and (b) the finding that *negotiation effort and differentiation* in splits correlate with better outcomes than quick equal splits ([Hellmann & Wasserman 2017](https://pubsonline.informs.org/doi/10.1287/mnsc.2016.2474)). We also correct its documented weaknesses (gaming of multipliers, no performance floor, no legal wrapper — [Equity Matrix critique](https://equitymatrix.io/blog/slicing-pie-problems)) as noted inline.

**The formula.** For person *p* in quarter *q*:

```
points(p,q) = [ Σ verified_hours(p,q,category) × Rate(category) ] × RiskMult
            + cash_contributed(p,q) × 4.0
            + approved_expenses(p,q) × 2.0
then adjusted: points(p,q) × Kicker(p,q)         where Kicker ∈ [0.75, 1.25]

RiskMult = 2.0 while the person is unpaid; 1.0 for any period they draw ≥ 50% of the Rate in cash
Share of Contribution Pool = lifetime points(p) / Σ all lifetime points   (recomputed quarterly)
```

**The Rate Table** (anchored to public data, converted at 2,080 hr/yr; re-benchmarked annually by the Contribution Committee, changes require 66⅔% approval):

| Category of work (not job title) | Anchor | Rate |
|---|---|---|
| Software engineering | BLS OEWS May 2024 median for software developers, $133,080 ([BLS](https://www.bls.gov/ooh/computer-and-information-technology/software-developers.htm)) | $64/hr |
| Senior/staff-level engineering & architecture (Committee-certified scope) | +25% band | $80/hr |
| Engineering management; business planning; fundraising prep; technical vision | pegged to senior band | $80/hr |
| Specialized ML research | benchmark process, cap 2× base | ≤ $128/hr |
| Admin/ops | BLS all-occupations-anchored | $30/hr |

Design principles doing real work here:
- **The rate attaches to the *work*, not the person.** A founder and an employee writing the same code earn the same rate — this is fixed requirement #2, mechanized. A junior employee doing management work gets the management rate for those hours.
- **Vision and strategy get hours-at-a-rate, not a multiplier.** "Idea" premiums are the most-gamed and least-verifiable input (the critique literature's central warning). The idea-generation premium the academic evidence supports (idea generation predicts *unequal* splits and larger idea-holder shares — Hellmann & Wasserman 2017) is delivered instead through the bounded **Kicker**: the Contribution Committee may scale a person's quarterly points by 0.75–1.25× for demonstrated outsized (or deficient) impact, with written justification, recusal of the affected person, and publication to all members. Subjectivity capped at ±25%, on the record.
- **Cash multiplier (4×) applies only to board-approved capital calls** — this closes the documented gaming vector of writing small opportunistic checks to farm the highest multiplier.
- **Verification.** Going forward: contemporaneous logs in a shared system, submitted monthly, visible to all members (transparency is the mechanism the justice literature rewards), auditable against git/PR history, docs, and calendars; the Committee may reject unverifiable hours. Weekly cap of 60 loggable hours.

### 2.4 The Retrospective Reckoning (Year 1)

One-time application of the same formula to the founding year:
1. Each person submits a quarter-by-quarter reconstruction of hours by category, with evidence (commit/PR history, design docs, meeting records, calendars).
2. **Peer attestation:** each submission requires signatures from two other members with direct knowledge.
3. **Haircuts for uncertainty:** hours with documentary evidence count at 100%; attested-but-undocumented hours at 75%; contested hours at 50% pending Committee resolution. Retroactive weekly cap: 60 hours.
4. RiskMult = 2.0 applies to the whole unpaid year. The four past reserved-pool tranches are resolved against the same record (a founder who met the Activity Gate in 2 of 4 quarters has earned 0.625% and permanently lost 0.625%).
5. Output: the opening ledger, ratified by 66⅔% of units, then **issued as equity within 30 days** (Move 2 timing, for the tax reasons in Part 0) with 83(b) elections where applicable.

A founder who did high-level business planning all year and a senior employee who shipped the product are both handled by the same arithmetic — worked example:

| Person | Y1 verified hours (rate band) | Cash | Raw points | Illustrative pool share |
|---|---|---|---|---|
| Founder A (active, mgmt+eng) | 2,000 @ $80 | $20,000 | (160,000×2)+(80,000) = 400,000 | 400,000/Σ |
| Founder B (inactive since Q2) | 300 @ $64 | — | 38,400 | 38,400/Σ |
| Employee 1 (senior eng, full-time) | 2,200 @ $80 | — | 352,000 | 352,000/Σ |
| Employee 2 (eng, part-time) | 1,000 @ $64 | — | 128,000 | 128,000/Σ |

The intended and defensible result: **Employee 1 out-earns Founder B by ~9×** in the Contribution Pool, while Founder B keeps whatever reserved tranches they actually earned. That is the founders' stated bargain, made computable.

### 2.5 Inactive founders — the complete treatment

Every dimension, stated explicitly:
- **Earned equity (reserved tranches earned + ledger points):** kept in full. We deliberately do not claw back earned equity; forfeiture-of-earned provisions are both a fairness violation (with the team-poisoning consequences Breugst et al. document) and a litigation magnet.
- **Unearned reserved tranches:** lapse quarterly, automatically, forever (§2.2).
- **Future ledger points:** none unless they contribute — self-executing.
- **Governance:** no reserved board seat exists to lose; an inactive founder holds only their unit vote. Officer/committee roles require election or appointment.
- **On departure:** company **call option at fair market value** (independent appraisal now; 409A value post-conversion) on all units, exercisable for 180 days — the standard dead-equity cure ([Perkins Coie](https://perkinscoie.com/insights/blog/dealing-dead-equity)). Payable over up to 3 years to protect cash. Not mandatory: the board may leave a cooperative ex-member on the cap table.
- **Pre-committed investor re-vesting:** all members agree in advance (OA Art. VIII) to accept re-vesting of up to 25% of then-held equity over 2 years if the lead investor of the first priced round requires it — converting a common term-sheet fight into a signed pre-commitment.
- **Restrictive covenants:** confidentiality + 12-month non-solicit for everyone. **No noncompete by default:** under M.G.L. c. 149 §24L, an employee noncompete requires garden-leave pay of 50% of salary or other mutually-agreed consideration and is capped at 12 months ([Beck Reed Riden](https://beckreedriden.com/the-massachusetts-noncompetition-agreement-act-massachusetts-general-laws-c-149-s-24l/); [mass.gov](https://www.mass.gov/info-details/mass-general-laws-c149-ss-24l)) — expensive and, for an unpaid team, incoherent. [Counsel: §24L's application to LLC *members* (vs employees/contractors) is unsettled; advise whether member-status noncompetes tied to the sale-of-business exception are worth the complexity. Flagged, not resolved.]

### 2.6 The professor

Facts: informally promised "a decent share," expects an above-market personal rate, is part-time, and is presumably a full-time Yale faculty member.

**The rate question is answered by the system, not by status.** The Rate Table prices *work*; a person may petition for a premium rate only with **two independent written FMV benchmarks** for comparable work (e.g., documented ML-consulting engagements), Committee approval, and a **hard cap of 2× the base engineering rate (≤$128/hr)**. This rule is available to *everyone* — a star employee can invoke it too — so requirement #2 is preserved. What the professor cannot get is a rate premium *because he is a professor*.

**Recommended offer — two tracks, his choice:**
- **Track A (recommended): standard advisor grant.** 0.5% of fully-diluted equity, from the Advisor Pool, 2-year monthly vesting, 3-month cliff — squarely inside the FAST benchmark grid (strategic-level advisor at a post-idea-stage company: 0.3–0.5%; expert-level: up to 0.8% — [Founder Institute FAST](https://fi.co/fast), [FI overview](https://fi.co/insight/the-founder-institute-s-standard-advisor-agreement-for-startups-fast)). Uplift to 0.8% if he commits ≥10 hrs/month with named deliverables.
- **Track B: compete in the Contribution Pool** under identical ledger rules at his benchmarked rate. Realistic yield at 5 hrs/week × $128/hr: meaningful but modest — which is the honest price signal for part-time involvement.
- Either track is **conditioned on**: (1) a written agreement including a **release of all claims arising from the informal promise** — the oral "decent share" promise is a live promissory-estoppel/oral-contract risk that counsel must extinguish, not ignore; (2) **Yale COI clearance**: Yale caps consulting at one day per seven-day week, requires annual disclosure of external financial interests, and reviews faculty equity in startups under its COI policy, Appendix C ([Yale COI Policy](https://research-support.yale.edu/sites/default/files/2025-03/coi_policy_0.pdf); [Yale External Activities Guidance](https://provost.yale.edu/policies/external-professional-activities-guidance)); (3) **IP provenance reps**: Yale claims inventions made by its employees within employment scope or using Yale resources ([Yale Patent Policy](https://ventures.yale.edu/sites/default/files/2023-03/Yale_Patent_Policy.pdf)) — he must represent that his contributions use no Yale resources, students, or facilities, and assign all work product to the company. If his ML contributions are adjacent to his Yale lab's work, **counsel must clear provenance before any grant issues**; an unresolved Yale IP claim in the data room is a financing-killer.
- If he declines both tracks: the company should absorb the awkwardness now rather than carry an unpriced oral claim into diligence. Total advisor exposure is capped by the 1% pool regardless.

### 2.7 Investor-attractiveness checklist (requirement #3, consolidated)

Delaware C-corp with QSBS-eligible stock at a $15M/10× cap ([Millan & Co.](https://millancpa.com/insights/section-1202-qualified-small-business-stock-qsbs-tax-guide)) · clean single-class cap table, no dead equity ≥10% ([ISA Ventures](https://isaventures.substack.com/p/dead-equity-on-your-cap-table-is)) · everyone vested/earned with 83(b)s on file · pre-committed re-vesting · standard 4/1-shaped schedules ([Carta](https://carta.com/learn/equity/stock-options/vesting/)) · Rule 701 equity plan ([Cooley GO](https://www.cooleygo.com/why-private-companies-should-know-about-rule-701-options-rsas-and-rsus/)) · ROFR, drag-along, tag-along in place · no oral equity promises outstanding · Wage Act exposure cured and documented · IP assignments from every contributor including the professor · a board with an investor seat and independent seat pre-architected.

---

## Part 3 — Consolidated flags for counsel (decide-with-lawyer, not decided here)

1. Wage Act cure mechanism and member-vs-employee characterization for each of the 15 people; assess and, if needed, remediate accrued Year-1 exposure (M.G.L. c. 149 §148; strict liability; personal officer liability).
2. Independent-contractor ABC-test exposure for any non-member contributors.
3. Securities exemptions for LLC unit issuances now (§4(a)(2)/Reg D; Rule 701 is corporation-era) and blue-sky filings; 15+ holders.
4. Tax structuring of the Reckoning: capital interests vs. catch-up profits interests ([Rev. Proc. 93-27](https://www.irs.gov/pub/irs-drop/rp-01-43.pdf) line of authority); 83(b) timing; valuation support.
5. MA→DE conversion mechanics (M.G.L. c. 156C; [mass.gov LLC law page](https://www.mass.gov/info-details/massachusetts-law-about-limited-liability-companies-and-limited-liability-partnerships)) and §1202 qualification at conversion (asset test, active-business test, redemption look-backs — redemptions near stock issuance can taint QSBS; sequence the FMV call option accordingly).
6. §24L noncompete applicability to members; enforceability of the sealed-bid separation mechanism; arbitration clause scope for statutory wage claims (likely non-waivable).
7. The professor: release of the oral promise; Yale COI and patent-policy clearance; invention assignment; whether any Yale-affiliated IP is already embedded in the product.
8. 409A valuation cadence post-conversion; option plan adoption; Rule 701 disclosure thresholds if grants exceed $10M/12 months.

---

## Part 4 — Threats to validity (what would change our design)

- If the team will **never** raise institutional capital, the C-corp conversion loses its main justification and an LLC with profits interests becomes the better tax answer. The design assumes requirement #3 means venture-scale financing.
- The ledger's benefits depend on **administration actually happening** (monthly logs, quarterly cycles). If the team won't sustain that, a one-time negotiated split with standard 4/1 vesting — the boring answer — beats a decaying ledger. We rate this the single largest practical risk of our own design and mitigate it by sunsetting the ledger at the first financing.
- All leadership-structure evidence is correlational; if the elected-board/single-CEO structure produces a leader the team won't follow, the annual mandate and election cycle are the designed-in correction mechanism.
