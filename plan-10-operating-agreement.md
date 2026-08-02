# plan10 — Operating Agreement: Article-by-Article Business Terms

**Status:** Business-terms term sheet for counsel. This is not a legal instrument. Every section states the intended business deal; bracketed items `[...]` are open decision points for the founders or drafting questions for counsel. Statutory mechanics, tax boilerplate, and securities compliance are deliberately left to counsel — flagged where we know they exist.

**Instrument:** Amended & Restated Operating Agreement of [Company] LLC, a Massachusetts limited liability company (M.G.L. ch. 156C), to be adopted by unanimous written consent of all current members, superseding all prior oral or informal understandings.

---

## Article I — Formation, Purpose, Definitions

1.1 **Continuation.** The Company continues as a Massachusetts LLC under ch. 156C. [Counsel: confirm the certificate of organization matches the manager-managed structure adopted below; amend if needed.]

1.2 **Purpose.** Any lawful business, with the current business described in Exhibit A.

1.3 **Defined terms** (business meanings; counsel to formalize):
- **Unit** — a fractional membership interest; the Company maintains a single ledger of Units. Percentages always mean percentage of all Units outstanding.
- **Contribution Pool** — the 75% of initial Units distributed solely under the Contribution Ledger (Article IV).
- **Founder Reserve** — the 25% of initial Units reserved 5% to each Founder, earned under Article V.
- **Contribution Points (CP)** — the unit of measured contribution defined in Article IV.
- **Ledger** — the Company's CP accounting system.
- **Crystallization Event** — defined in Article IX.
- **Fair Value** — value determined by an independent appraiser under Article XI, without minority or marketability discounts. [Counsel: define appraisal standard precisely.]

1.4 **Entire agreement / supersession.** This Agreement supersedes all prior equity understandings, including the founders' original equal-split understanding, the informal reserved-allocation agreement, and the informal promise of "a decent share" to the Advisor (addressed in Article VI). Each member signs a mutual release of equity-related claims arising from pre-signing promises, conditioned on receiving the retroactive settlement in Article IV. [Counsel: releases must be drafted carefully; Wage Act claims CANNOT be released this way — see Article XII.]

---

## Article II — Members, Units, Capital

2.1 **Members.** All persons holding Units. Current signatories: five Founders, [~10] contributors, and the Advisor upon satisfaction of Article VI conditions.

2.2 **Classes.** A single class of voting Units. No separate founder class, no super-voting rights, no golden shares. [Rationale: multi-class founder-control structures measurably depress private-company valuations and complicate financing; see design doc §3.]

2.3 **Units from the two sources only.** Initial equity comes exclusively from (a) the Contribution Pool and (b) the Founder Reserve. No other grants, side letters, or verbal promises create equity.

2.4 **Capital contributions.** No member is obligated to contribute capital. Cash actually contributed enters the Ledger as CP (Article IV) rather than as a capital account claim senior to others. [Counsel: reconcile with ch. 156C capital-account and tax capital-account mechanics.]

2.5 **New members.** Admission requires Board approval plus the standard joinder; equity only via the Ledger (or an option/profits-interest plan the Board adopts on Ledger-consistent terms).

2.6 **No employment rights.** Units confer no right to employment or engagement, and holding a role confers no right to Units except as the Ledger provides.

---

## Article III — Governance

3.1 **Manager-managed.** The Company is manager-managed. Authority sits with a **Board of Managers** of **three (3)** natural persons.

3.2 **Board composition and election.**
- Elected annually by members voting Units (one Unit = one vote), by cumulative voting. [Cumulative voting lets a cohesive minority — e.g., employee-contributors — elect one manager; open point: straight vs. cumulative.]
- At least **one seat must be held by a non-Founder** at all times.
- Any member holding at least [1]% of Units is eligible to stand.
- Managers serve one-year terms; no term limits; removable with or without cause by majority of Units.
- Vacancies filled by remaining managers until the next election.

3.3 **CEO.** The Board appoints one **CEO** (a single individual — no co-CEOs), sets the CEO's authority, and may remove the CEO at any time by majority of the Board. The CEO need not be a Founder. The CEO runs day-to-day operations and appoints other officers/leads.

3.4 **Decision matrix.** Three tiers:

| Tier | Examples | Decided by |
|---|---|---|
| Ordinary course | hiring/termination of contributors, spending within budget, product decisions, signing contracts < $[25,000] | CEO (or delegate) |
| Significant | annual budget, contracts ≥ $[25,000], borrowing, opening payroll, adopting/adjusting the Rate Card, admitting members, settling litigation, appointing/removing CEO | Board majority |
| Fundamental | amending this Agreement, changing the Ledger formula or Founder Reserve terms, merger/sale/dissolution, conversion (Article IX), issuing Units outside Articles IV–VI, related-party transactions over $[10,000], removing a member for cause | Members: ≥ 66⅔% of Units, **plus** for any change to Article IV, V, or VI formulas: a majority of Units held by non-Founders |

3.5 **Meetings and records.** Board meets at least monthly; minutes kept; decision memos required for Significant and Fundamental actions (proposal, options considered, decision, dissents). Members receive quarterly financials and the full Ledger (Article IV transparency).

3.6 **Fiduciary duties.** Managers and members owe the duties Massachusetts law imposes on closely held entities; this Agreement does not waive them. Related-party transactions require disclosure and approval by disinterested managers or disinterested members. [Counsel: MA courts apply close-corporation "utmost good faith and loyalty" standards to LLC members; the procedural-fairness machinery here is deliberate — do not weaken it.]

---

## Article IV — The Contribution Ledger (the 75% Pool)

*One system, identical terms for every participant — founder, employee, or advisor. The only individualized input is the market rate for the role actually performed, taken from a published Rate Card.*

4.1 **Principle.** Until Crystallization, each participant's share of the Contribution Pool at any time = that participant's CP ÷ all CP ever awarded. Percentages therefore float as work accrues ("dynamic equity") and freeze at Crystallization.

4.2 **The formula.** For each calendar month, for each participant:

> **CP = Σ over activities [ verified hours × Rate Card hourly rate for the role performed ] × k_noncash + (unreimbursed cash and FMV of property actually contributed) × k_cash**

- **k_noncash = 2.0** (uncompensated labor bears roughly double risk weight)
- **k_cash = 4.0** (out-of-pocket cash is the scarcest, highest-risk contribution)
- [Open point: keep the practitioner-standard 2×/4× or tune (e.g., 1.5×/3×). These multipliers are convention, not science — see design doc §4.4. Whatever is chosen must be identical for everyone.]
- If and when the Company pays cash compensation for work, the paid portion earns **no** CP (no double-dipping); partial pay earns CP only on the unpaid gap.

4.3 **Rate Card.**
- A published table of hourly rates by role and seniority, set from named external benchmarks (e.g., Carta/Pave/BLS Boston-market data for the role), adopted and adjusted annually by the Board (Significant action).
- The rate attaches to the **work actually performed that month**, not the person's title. A founder doing junior QA logs QA hours at the QA rate; an employee doing engineering-management logs at the EM rate.
- Specialist rates (e.g., an ML-professor-level scientific advisor) are permitted **only** if supported by verifiable external evidence of that person's market rate (e.g., their documented consulting rate to third parties, or published academic-consulting benchmarks). Same rule for everyone — this is how a "higher rate" can be honored objectively (Article VI).
- Rate Card changes are prospective only.

4.4 **Verification (what counts as "verified hours").**
- Hours are logged monthly in the Ledger, each entry linked to evidence: commits/PRs, documents, tickets, meeting records, or a deliverable.
- Caps: max [60] logged hours/week per person; entries older than [60] days are not accepted.
- A three-person **Ledger Committee** — elected annually by members, at least one non-Founder, no more than one Board member — audits entries. It verifies evidence; it has **no discretion to re-weight** anyone's contribution beyond the formula. Challenges: any member may challenge an entry within 30 days of the monthly ledger publication; the Committee rules; appeals go to arbitration (Article XI).
- The full Ledger (hours, roles, rates, CP, evidence links) is visible to all members. [Transparency is load-bearing: identifiability suppresses free-riding and perceived procedural justice protects the team — design doc §4.5.]

4.5 **Retroactive settlement of Year One (one-time).**
- The same formula applies to the pre-signing period, with evidence tiers:
  - contemporaneous records (commits, docs, calendars): **100%** of computed CP;
  - no contemporaneous record but corroborated in writing by ≥ 2 other members: **[85]%**;
  - uncorroborated self-report: **[50]%**, capped at [20] hours/week.
- Cash and property contributed during Year One enter at documented amounts × k_cash.
- Each person submits a Year One statement within [45] days of signing; the Ledger Committee (first committee elected at signing) audits; the settled Year One CP schedule is attached as Exhibit B and ratified by ≥ 66⅔% of Units **and** a majority of non-Founder Units, then is final and unappealable except for fraud.
- Units for Year One CP are granted **at signing, while fair market value is low**, with protective 83(b) elections where applicable. [Counsel: characterize as profits interests vs. capital interests; retroactive capital interests for past services are taxable compensation — structure and value carefully. See Article XII.]

4.6 **Ongoing operation.** Monthly cycle: log → publish → 30-day challenge window → quarterly Board ratification (ministerial — the Board confirms process was followed; it cannot adjust individual CP). Quarterly, accrued CP converts into Units so the cap table always reflects the Ledger.

4.7 **Departure.**
- **Voluntary departure or termination without cause:** keeps all Units from verified CP (work performed is work owned); simply stops accruing.
- **Termination for cause** (fraud on the Ledger, material breach, conduct defined in Exhibit C): forfeits [50–100]% of Units derived from CP in the trailing [12] months, by Fundamental member vote excluding the affected member; affected member may demand arbitration. [Counsel: forfeiture provisions in MA closely held entities are fiduciary-sensitive; draft the cause definitions tightly and the procedure fairly.]
- No mandatory buyback of earned Units. The Company holds an optional right of first refusal on transfers (Article VIII) and an optional Fair Value buyout on death/disability [open point: also on departure? Investors dislike broad dead equity, but forced buyouts are cash-draining and fiduciary-sensitive].

---

## Article V — The Founder Reserve (5% × 5, earned)

5.1 **Grant.** Each of the five Founders is allocated a reserve of **5.0%** of initial Units (fixed requirement). The reserve is **entirely unvested at signing** and is earned only as follows.

5.2 **Earning schedule.** 16 equal quarterly tranches (0.3125% each) over 4 years, starting from the Agreement date. A tranche vests only if, for that quarter, the Founder satisfies the **Activity Test**:
- ≥ [20] hours/week average of Ledger-verified contribution, **or**
- a Board-approved quarterly deliverable plan certified complete by the Board (for founders whose work is lumpy).

5.3 **Credit for Year One.** Founders who satisfy the Activity Test retroactively (same evidence tiers as §4.5) are credited up to 4 already-vested tranches. Founders who were inactive receive credit only for quarters they actually meet the test. [This is the "use it or lose it" requirement applied evenly to the past.]

5.4 **Missed tranches.** A tranche whose quarter's Activity Test is failed is **permanently forfeited** and its Units return to the Contribution Pool (benefiting all Ledger participants pro rata) — not to the other founders specifically. Two consecutive failed quarters suspend the reserve; reinstatement of *future* tranches requires Board approval.

5.5 **Acceleration.** [Open point: single-trigger acceleration is investor-hostile; recommend **double-trigger only** (change of control + termination without cause), 50–100% of remaining reserve. Decide percentage.]

5.6 **No other founder privileges.** Outside this Article, Founders hold no rights different from any member: same Ledger, same Rate Card discipline, same vote-by-Units.

---

## Article VI — The Advisor (the professor)

6.1 **Supersession.** The informal promise of "a decent share" is replaced in full by this Article; the Advisor's signature (with release) is a condition of any grant.

6.2 **Fixed advisory grant.** [0.5–1.0]% of initial Units — top-of-market for a part-time advisor at this stage per the FAST framework and market data — vesting monthly over 24 months, no cliff, contingent each month on continued service under a written advisor agreement (scope, deliverables, minimum [X hours/month]).

6.3 **Ledger participation.** In addition, the Advisor may participate in the Contribution Ledger on **identical terms** to everyone else. His "higher rate" is honored the only defensible way: through the Rate Card's specialist-rate rule (§4.3) at his **documented external consulting rate** [requires evidence: engagement letters/invoices to third parties; otherwise the published academic-ML-consulting benchmark rate applies].

6.4 **Conditions precedent** (no Units vest until all are met):
1. Written advisor agreement (services, confidentiality, IP assignment of work done for the Company).
2. **Yale conflict-of-interest disclosure/approval** as his faculty obligations require; written confirmation that his Company work is within permitted outside-activity limits.
3. IP provenance certification: nothing contributed was created with university resources or is subject to university/Bayh-Dole claims; where his prior academic IP is needed, a license from Yale, not an informal contribution. [Counsel: this is a diligence landmine for future investors; paper it now.]

6.5 **Board/consultant status.** The Advisor is not a manager and holds no board seat by virtue of this Article. [Open point: a Scientific Advisory Board title is fine; governance power is not part of "a decent share."]

---

## Article VII — Distributions, Allocations, Tax

7.1 **Distributions** pro rata to Units, when and as the Board declares; mandatory tax distributions to cover members' pass-through tax on allocated income [standard assumed-rate formula — counsel drafts].

7.2 **Profits interests.** Ongoing CP-based Units are intended to be **profits interests** (Rev. Proc. 93-27 / 2001-43 safe harbors) with threshold values set at grant; protective 83(b) elections filed within 30 days of each grant. [Counsel: confirm safe-harbor eligibility given quarterly conversion mechanics; consider an annual grant cadence if monthly is unworkable.]

7.3 **Year One settlement units:** [Counsel decision: profits-interest structuring where possible; to the extent any grant is a capital interest for past services it is compensation income at FMV — obtain a contemporaneous low-FMV valuation now.]

7.4 **Members are not W-2 employees** for tax purposes once admitted; K-1s and self-employment tax follow. [Counsel/CPA: brief every participant before signing; this interacts with the Wage Act remediation in Article XII.]

7.5 **83(b) discipline.** The Company collects proof of filing for every unvested grant.

---

## Article VIII — Transfers

8.1 No transfers without Board consent, except estate-planning transfers to revocable trusts.
8.2 Company right of first refusal, then pro-rata member ROFR, on any permitted sale.
8.3 Tag-along on any Founder sale ≥ [5]% of Units; drag-along on a Board-approved plus ≥ 66⅔%-of-Units-approved sale of the Company, on identical per-Unit terms. [Drag-along is an investor-readiness feature; counsel drafts minority protections.]
8.4 No pledges/encumbrances without Board consent.

---

## Article IX — Crystallization and Conversion (investor readiness)

9.1 **Crystallization Event** — the earliest of:
1. Board approval of a priced equity financing of ≥ $[1,000,000];
2. Board + Fundamental-vote decision to convert;
3. [36] months after signing.

9.2 **At Crystallization:** the Ledger freezes (final month closes, challenges resolved), percentages become fixed, and the dynamic system **ends permanently**. Unvested Founder Reserve tranches continue on their existing schedule as time-based vesting of fixed shares.

9.3 **Conversion.** Upon a qualified financing (or earlier by Fundamental vote), the Company converts to a **Delaware C-corporation** (statutory conversion or merger — counsel selects the tax-efficient route; Rev. Rul. 84-111 framework), with:
- each member receiving stock pro rata to Units;
- a new employee **option pool of [12–15]%** (post-conversion) for future hires;
- standard 4-year/1-year-cliff vesting for future grants;
- all members signing customary IP assignment and confidentiality agreements to cure diligence gaps.
- [Counsel: QSBS §1202 planning — the 5-year (or post-July-2025 tiered) holding clock and basis step at conversion make timing consequential; model conversion earlier if value is accreting fast.]

9.4 **Cooperation covenant.** Every member pre-agrees to execute conversion documents that preserve their pro-rata economics (subject to the option pool), so no individual holdout can block investor-required restructuring. [Counsel: enforceability of advance consent in MA; consider power-of-attorney mechanics.]

---

## Article X — Information Rights, Confidentiality, IP

10.1 All members: quarterly financials, annual budget, full Ledger access, K-1s on time.
10.2 Every member signs a confidentiality and **present-assignment IP agreement** covering all work for the Company (retroactive confirmation for Year One work — a diligence must-have). [Counsel: MA has statutory limits on non-competes (2018 Act — garden-leave/consideration rules); recommend nonsolicit + confidentiality + assignment, and only targeted noncompetes if any.]
10.3 No member may use Company confidential information for outside work; the Advisor's academic publishing rights are governed by the advisor agreement [open point: publication review window, e.g., 30 days].

---

## Article XI — Disputes and Deadlock

11.1 **Ladder:** (1) good-faith negotiation between principals [14 days]; (2) mediation in Boston (JAMS/AAA) [30 days]; (3) final binding **arbitration** in Boston, single arbitrator, [AAA Commercial Rules], fee-shifting at arbitrator's discretion; carve-outs for injunctive relief (IP/confidentiality) in court.
11.2 **Ledger appeals** follow §4.4 then this ladder; the arbitrator applies the formula — no equitable re-slicing.
11.3 **Deadlock** (Board or Fundamental-vote deadlock persisting [60] days on a matter threatening operations): either side may trigger **appraised Fair Value buyout** mediation; explicitly **no shotgun/Russian-roulette clause** [rationale: shotgun clauses favor the cash-rich party and are fiduciary-fraught in MA close entities — design doc §7].
11.4 Governing law: Massachusetts (pre-conversion). [Counsel: choice of forum; interaction of arbitration with Wage Act claims — some claims are non-arbitrable or arbitrable only with care.]

---

## Article XII — Compliance Remediation (urgent, precedes everything)

*Not an equity term — a gating legal-risk item counsel must drive. The equity design assumes it is fixed.*

12.1 **Massachusetts Wage Act.** ~10 non-owner workers have been unpaid for up to a year. MA law: no volunteering for a for-profit; wages cannot be waived or replaced with equity; violations carry **mandatory treble damages, 3-year lookback, and personal liability for officers/managers**. The Company must, with counsel, immediately either (a) put workers on lawful payroll (≥ MA minimum wage, overtime as applicable), (b) convert genuine partners into bona fide equity members with counsel-blessed documentation, or (c) pause non-member work. Back-wage exposure must be quantified and remediated; Units do NOT settle it.
12.2 **Misclassification.** MA's strict ABC test (ch. 149 §148B) likely makes these workers employees, not contractors. Counsel to assess.
12.3 **Securities.** ~15+ equity recipients: counsel to select exemptions (e.g., §4(a)(2)/Reg D; note Rule 701 is unavailable to LLCs in the usual form), file any MA blue-sky notices, and paper investment representations.
12.4 **Prior promises.** Inventory all informal equity promises (beyond the Advisor's) and clean them up with the release/supersession mechanics of §1.4.
12.5 **Insurance/agreements hygiene:** D&O when affordable; IP assignments (§10.2); employment documentation as payroll starts.

---

## Signature mechanics

Adoption requires **unanimous** signature of all five Founders and all current contributors receiving Year One settlements [unanimity is the clean path: it moots most freeze-out/fiduciary attacks on the reallocation; if unanimity fails, counsel must advise on the ch. 156C amendment path and its litigation risk before proceeding].
