# plan-7 — Amended & Restated Operating Agreement (Business-Terms Draft)
### [Company Name], LLC — a Massachusetts limited liability company

**Status:** business-terms draft for counsel. Square brackets `[...]` mark open decision points for the founders or drafting/validation items for counsel. This document encodes the design in `plan-7-design.md`; where the two diverge, the design document's rationale governs intent. Statutory drafting, tax execution, and enforceability review are counsel's.

---

## Article I — Formation, Purpose, Definitions

1.1 Continuation of the existing Massachusetts LLC under M.G.L. c.156C; principal office [address]; registered agent [name].
1.2 Purpose: any lawful business, presently [describe software business].
1.3 Key defined terms (economic definitions; counsel to formalize):
- **Effective Date:** the date this Agreement is signed by all Members.
- **Contribution Ledger, Contribution Units, Rate Table, Multipliers (M_noncash = [2.0], M_cash = [4.0]), Active Founder Standard ([80] accepted hours/month), Bands (E1 $[40]/hr, E2 $[66.50]/hr, E3 $[105]/hr, B1 $[66.50]/hr, X1 $[400]/hr):** as defined in Exhibit A (the Equity Engine), which restates design Parts 3–4.
- **Freeze Event:** earliest of (a) closing of a priced equity financing with gross proceeds ≥ $[1,000,000]; (b) the Conversion (Art. XIII); (c) [3] consecutive months of cash-flow breakeven with all service providers paid at least fair-market cash compensation; (d) a Sale of the Company approved under Art. IX.
- **Fundamental Decision:** the matters listed in §9.3.
- **Neutral Arbiter:** the standing arbitrator engaged under §12.3.

## Article II — Members; Units; Classes

2.1 Single economic class: **Class A Units** ("Earned Units"). One vote per Unit. No Member has rights by virtue of "founder" status except the Founder Reserve (Art. V).
2.2 Founders and non-founder Members hold Units on identical terms (identical engine, Rate Table, vesting logic, transfer restrictions, information rights).
2.3 Admission of new Members pre-Freeze: Board approval (Significant Decision); each new Member joins the Engine on the same terms; signs this Agreement + PIIA.
2.4 [Counsel: mechanism for Members who cannot accept K-1 partner status — parallel **phantom-unit plan** mirroring the Engine's arithmetic, cash-settled or converted at the Freeze Event; §409A compliance required.]

## Article III — Capital; No Required Contributions

3.1 No Member is obligated to contribute capital. Cash contributions and approved unreimbursed expenses earn Contribution Units at M_cash per Exhibit A; committed-but-unspent cash earns nothing until spent.
3.2 No interest on capital; no return of capital except through distributions/liquidation.
3.3 [Counsel: maintain capital accounts per Treas. Reg. §1.704-1(b); target allocations.]

## Article IV — The Equity Engine (Exhibit A operative provisions)

4.1 **Allocation:** 25% of fully diluted Units constitute the aggregate Founder Reserve (Art. V); 75% constitute the Contribution Pool, allocated in proportion to cumulative Contribution Units per the formula: `Units(i,m) = Hours(i,m,activity) × Rate(activity) × M_noncash + CashOut(i,m) × M_cash + accepted FMV of other property × M_noncash`, less any cash compensation actually paid (which reduces at-risk time value before multiplication).
4.2 **Logging & acceptance:** weekly logging; [30]-day admissibility limit; monthly acceptance by the Ledger Administrator; challenges → Board → Neutral Arbiter; 60-day silence = acceptance.
4.3 **Transparency:** the complete Ledger and all Members' running percentages are distributed to all Members monthly. This §4.3 may be amended only by Fundamental Decision.
4.4 **Rate Table re-anchor:** annually and mechanically to the then-current BLS OEWS software-developer percentiles (E1 = 10th, E2 = median, E3 = 90th, ÷ 2,000); Band X1 re-anchored to [SEAK expert-fee survey median]. Band assignments per person per activity set annually by the Board; appealable to the Neutral Arbiter.
4.5 **Retroactive Year-1 allocation:** conducted once, per Exhibit B (claims → blind peer banding using the [2,000/1,500/1,000/500/100/0]-hour bands → artifact reconciliation → Arbiter for gaps > one band → entry as opening Ledger balances). Signing this Agreement ratifies the resulting allocation and supersedes all prior informal equity understandings. [Counsel: scope of enforceable release — Wage Act claims are presumptively NOT privately releasable; carve out accordingly.]
4.6 **Tax execution [counsel/CPA]:** opening-balance Units issued as capital interests at grant-date FMV supported by an independent valuation; go-forward accrual documented as profits interests intended to qualify under Rev. Proc. 93-27 and 2001-43 (hurdle = grant-date FMV); protective §83(b) elections within 30 days of each grant; K-1 consequences disclosed in writing to each Member.

## Article V — Founder Reserve

5.1 Each of the five Founders is allocated a reserve of Units equal to 5.0% of fully diluted Units at the Freeze Event, vesting **1/48th per month for 48 months from the Effective Date**, subject to §5.2.
5.2 **Earn-to-vest:** a monthly tranche vests only if the Founder met the Active Founder Standard ([80] accepted hours) that month. An unvested tranche for a non-qualifying month is **permanently forfeited** and its Units revert to the Contribution Pool.
5.3 **Retroactive credit:** at the Effective Date, one tranche vests for each pre-Effective-Date month in which the Founder's Exhibit-B band evidences at least half-time involvement (max [12] tranches).
5.4 Unvested reserve terminates on the Founder ceasing to provide services; [bracketed: on death or Disability, up to [6] additional tranches vest].
5.5 The Reserve carries no separate voting or economic preference; reserve Units when vested are ordinary Class A Units.

## Article VI — Members' Meetings; Voting

6.1 Annual meeting each [month]; special meetings on call of the Board or Members holding ≥ [10]% of Units.
6.2 Voting is by Units (one Unit, one vote). Quorum: Members holding > 50% of Units.
6.3 Except where this Agreement requires a Fundamental Decision or Board action, Member action requires > 50% of Units present.
6.4 Action by written consent permitted at the same thresholds.

## Article VII — Advisors; the [Professor] Agreement

7.1 Advisory (non-employee, non-Member-service) participants may join the Engine at Band X1 only under a written Advisor Agreement approved by the Board, containing: integration clause superseding all prior oral promises; IP assignment [with university-policy carve-out drafted by counsel]; confidentiality; termination at will by either party (accrued Units retained; accrual stops).
7.2 **Aggregate advisor cap:** all advisory participants' combined interests shall not exceed [2.0]% of fully diluted Units except by Fundamental Decision.
7.3 **[Open decision — milestone top-up for [Professor]:** additional grant of up to [0.5]% subject to achievement of [named technical milestone] as certified by the Board; recommended only if his continued engagement genuinely requires more than Engine accrual.]
7.4 [Counsel diligence items for [Professor]: Yale external-activity time cap compliance; no officer/manager role; Yale COI disclosure confirmation; Yale Ventures IP position on any inventive contributions (see *Fenn v. Yale*); §148B classification.]

## Article VIII — Board of Managers

8.1 The Company is manager-managed by a **Board of [3] Managers**.
8.2 **Election:** annually by the Members, Units-weighted; any Member eligible. [Open decision: cumulative voting, so a ≥25% bloc can seat one Manager.] [Open decision: designate seat 3 for a non-Member independent when the Board nominates and Members elect one.]
8.3 Removal of a Manager: Members holding > 50% of Units, with or without cause. Vacancies filled by remaining Managers until the next election.
8.4 Board acts by majority ([2] of [3]); no unanimity requirements. Meetings at least [monthly]; written minutes required (investor-diligence discipline).
8.5 **Powers (Significant Decisions):** annual budget; hiring/compensation policy; Band assignments; Ledger challenge rulings (subject to Arbiter appeal); admitting Members; expenditures off-budget > $[25,000]; litigation; for-Cause determinations (§10.3); engaging auditors/valuation firms.
8.6 The Board appoints and removes Officers, including the **Chief Executive Officer** (removal by Board majority at any time). The CEO manages day-to-day business within the budget and role charter; the Board may not manage day-to-day operations collectively.
8.7 **Sunset:** this Article terminates automatically at the Freeze Event, replaced by the governance provisions of the financing/conversion documents (expected: NVCA-model voting agreement).

## Article IX — Decision Taxonomy

9.1 **Operational:** CEO (within budget/charter).
9.2 **Significant:** Board majority (§8.5).
9.3 **Fundamental (≥ [66⅔]% of all Units, and, where an amendment would reduce a Member's already-earned Units or accrued Ledger balances, that Member's written consent):
(a) Sale of the Company, merger, dissolution;
(b) amendment of this Agreement, the Engine (Exhibit A), the Multipliers, this taxonomy, or §4.3 (transparency);
(c) creation of any new class of Units or any issuance outside the Engine;
(d) indebtedness > $[100,000] aggregate;
(e) the Conversion, except as pre-authorized by Art. XIII;
(f) increasing the aggregate advisor cap (§7.2);
(g) any transaction between the Company and a Member/Manager > $[10,000] [interested party abstains].**

## Article X — Transfers; Buy-Sell

10.1 No transfers without Board consent, except to a Member's estate/revocable trust. Company right of first refusal, then Members pro rata, on any permitted transfer.
10.2 **Tag-along** for all Members on any transfer > [10]% of Units; **drag-along** on a Sale approved as a Fundamental Decision (all Members must sell on identical per-Unit terms).
10.3 **Departure & recovery:** on any cessation of services, earned Units are retained; unvested reserve and future accrual cease. On termination for **Cause** (narrow definition: fraud; felony conviction related to the Company; material breach of PIIA; willful and continued failure to perform after written notice and [30]-day cure), the Company holds a [12]-month option to repurchase the departed Member's Units at fair value per independent appraisal [open decision: minus a [20]% illiquidity discount — counsel: test against *Wilkes/Donahue*]. Contested Cause findings require Neutral Arbiter confirmation.
10.4 **Voluntary buyout offer:** the Company may offer (never compel) any inactive Member a buyback at appraised fair value.
10.5 [Counsel: 17200-style spousal consents; MA community-property N/A but obtain spousal acknowledgments where applicable.]

## Article XI — Distributions; Tax

11.1 Tax distributions: to the extent of available cash, the Company shall distribute annually at least each Member's [assumed combined rate 40]% × allocated taxable income [counsel/CPA: standard tax-distribution clause; profits-interest holders included].
11.2 Other distributions pro rata to Units, when and as the Board declares (subject to c.156C §35 solvency limits).
11.3 Partnership tax status until Conversion; Partnership Representative: [name]; [CPA: §704 allocations, §754 election policy].

## Article XII — Dispute Resolution

12.1 **Ladder:** written dispute notice → principals meeting within [10] days → Board (where applicable) → mediation within [30] days ([JAMS/AAA], Boston) → binding arbitration.
12.2 **Arbitration:** single arbitrator, [AAA Commercial / JAMS] rules, seat Boston, Massachusetts law; discovery limited; award enforceable in any court. [Counsel: carve-outs for injunctive IP relief.]
12.3 **Neutral Arbiter (standing):** a pre-engaged neutral [retired judge / experienced startup counsel / CPA panel] with a fast-track (≤ [30]-day) written procedure deciding: Exhibit-B banding disputes, Ledger challenges, Band-assignment appeals, and contested Cause findings. Fees borne by the Company [open decision: loser-pays for frivolous challenges].
12.4 **Last-resort buy-sell (shotgun):** only for a Fundamental-tier deadlock persisting > [90] days after the §12.1 ladder is exhausted: any Member(s) holding ≥ [20]% may serve a single-price offer; recipients elect to buy or sell at that price within [45] days; closing within [60] days. [Counsel: financing-fairness mechanics; the design intends this as deterrent — see Brooks/Landeo/Spier evidence that such clauses are rarely triggered.]

## Article XIII — Pre-Authorized Delaware Conversion

13.1 The Members, by signing, **pre-authorize** the Board to effect conversion of the Company into a Delaware corporation upon or in anticipation of a Freeze Event, provided: (a) each Member receives stock in proportion to Units (vesting schedules carried over); (b) an independent valuation supports the conversion-date FMV (QSBS basis under §1202(i); 409A consistency); (c) intended §351 non-recognition [counsel: §357(c) liabilities check]; (d) a [12.5]% post-conversion option pool is authorized; (e) customary NVCA-form documents.
13.2 [Counsel: mechanism — DGCL §265 conversion vs. c.156C §§59–63 merger; MA filings; whether pre-authorization satisfies fiduciary standards given *Allison v. Eriksson* — unanimous execution of this Agreement is the intended safe harbor.]

## Article XIV — IP; Confidentiality; Restrictive Covenants

14.1 Every Member, Officer, employee, and advisor executes the Company's PIIA (present assignment of Company-related IP; confidentiality; [counsel: MA Noncompetition Agreement Act limits — garden-leave/consideration requirements; prefer non-solicit over non-compete]).
14.2 Company-related IP created during the unpaid Year 1 is assigned and ratified via the Exhibit-B process signatures. [Counsel: confirm chain of title for all pre-Agreement work, including any contribution by [Professor] — see §7.4 Yale issues.]

## Article XV — Miscellaneous

15.1 **Wage-law compliance [CRITICAL — counsel]:** contemporaneously with execution, the Company adopts a compensation plan intended to comply with M.G.L. c.149/§151 (minimum cash wages; pay-frequency) for all persons properly classified as employees; nothing in this Agreement defers, waives, or substitutes equity for wages required by law; [counsel: remediation plan for accrued exposure; classification review under §148B for every service provider].
15.2 Fiduciary duties per c.156C §63 [open decision: retain default duties (recommended, given close-company dynamics) vs. contractual tailoring; no elimination of good faith/fair dealing].
15.3 Amendment: Fundamental Decision only (§9.3(b)).
15.4 Governing law: Massachusetts (until Conversion). Counterparts; electronic signature.
15.5 Entire agreement; **supersedes all prior oral or informal equity understandings**, including any pre-Agreement founder split understandings and the informal advisor promise addressed by Art. VII.
15.6 [Counsel: securities-law exemption for Unit issuances to ~[16] persons — federal (e.g., Rule 701/Reg D as applicable to LLC interests) and MA blue sky.]

---

### Exhibit A — The Equity Engine
[Restates design Parts 3.2–3.7 verbatim as operative text: formula, Rate Table with re-anchor mechanics, multipliers, logging/acceptance/transparency rules, Freeze mechanics, worked example as interpretive aid.]

### Exhibit B — Year-1 Retroactive Process
[Restates design Part 4: claim form; bands (2,000/1,500/1,000/500/100/0 annualized hours); blind peer-banding procedure; artifact classes (VCS history, documents, calendars, receipts); reconciliation rule (settle at [lower of claim and peer median / peer median] within one band; Arbiter beyond); ratification and release language (subject to §4.5 carve-outs).]

### Exhibit C — Form of PIIA · Exhibit D — Form of Advisor Agreement · Exhibit E — Initial Rate Table & Band Assignments · Exhibit F — Initial Members & Opening Ledger Balances
[Counsel to draft C–D; Board to complete E–F upon Exhibit-B completion.]
