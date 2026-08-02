# plan10 — Full Design Document: Governance & Equity for a Five-Founder Massachusetts LLC

**Optimization target (fixed):** maximize attractiveness to future investors. Every design choice below is scored against that target first; fairness, harmony, and tax efficiency are instrumental — they matter because their absence destroys fundability.

**Companion documents:** `plan-10-one-pager.md` (summary) · `plan-10-operating-agreement.md` (article-by-article business terms for counsel) · `plan-10-references.md` (annotated bibliography with evidence-strength ratings).

---

## 1. The situation, restated as an investor would see it

A diligence team looking at this company today would find: five founders with an oral equal split later orally amended; diverged and partly abandoned founder involvement; ~10 workers unpaid for a year in a state with mandatory treble wage damages and personal officer liability; an unwritten promise of "a decent share" to a part-time Yale professor whose IP may belong to Yale; an LLC (the wrong vehicle for venture money); and no vesting, no IP assignments, no board. Each item is a known, named red flag in investor practice — dead equity risk, undocumented ownership, wage claims, encumbered IP, entity friction (refs: Techstars dead-equity screening [S1]; Carta/AngelList diligence red-flag lists [S2][S4]; Kruze/YC on entity choice [S18][S21]).

The design therefore has two jobs: **(a)** convert a year of informal history into a clean, documented, formula-driven cap table with no live claims hanging over it, and **(b)** install governance that looks — and is — investable: accountable single leadership, a real board, standard vesting, and a pre-committed path to a Delaware C-corp with a frozen cap table.

### 1.1 Why not simply "negotiate a new static split now"?

Because the evidence says the *process* is the product. Quick, negotiation-free splits — the team's original arrangement — are the documented failure mode: roughly a third of founding teams split equally, 73% split within a month of founding, and quick equal splitters raise at significantly lower valuations, with ~$450K NPV at stake for typical teams (Hellmann & Wasserman 2017, *Management Science*, N = 1,476 founders/511 ventures — correlational, selection-driven [A1]; Wasserman 2012 [A2]). Lab evidence sharpens the mechanism: the equal-split penalty operates through **sorting** — low contributors select into equal splits — and **delaying the split until contribution is observable mitigates it** (Kagan, Leider & Lovejoy 2020, *Management Science*, causal-lab [A6]). This team has already run the natural experiment: a year has passed and contribution is now observable. A contribution-measured settlement is precisely the "delayed, informed contracting" the causal evidence recommends — and a fresh static renegotiation would re-fight the same battle with no objective anchor, maximizing the perceived-injustice spirals that destroy teams (Breugst et al. 2015, 8-team qualitative [A9]).

One honest caveat up front, repeated in §11: **no peer-reviewed study validates any dynamic-equity framework end-to-end.** The design rests on a lattice: causal lab evidence for delayed/informed contracting [A6], large-N correlational evidence against unexamined equal splits [A1][A3], meta-analytic evidence on identifiability and free-riding [A12], justice research on legible unequal outcomes [A9][A10][A11], and practitioner convention for the specific machinery (Slicing Pie [S22]) — with that machinery deliberately bounded by its documented critiques [S23].

---

## 2. Design overview

| Element | Decision |
|---|---|
| Entity now | Keep the MA LLC through the formalization phase; fix Wage Act problem immediately |
| Entity later | Pre-committed merger-conversion into a Delaware C-corp at Crystallization (priced round ≥$1M, or vote, or 36 months) |
| Equity: 25% | Founder Reserve — 5% per founder, 16 quarterly tranches over 4 years, each gated by an objective activity test; missed = forfeited to the pool |
| Equity: 75% | Contribution Pool — CP = verified hours × published market rate for the role performed × 2 (non-cash); cash/property × 4; identical formula for founders, employees, advisor |
| Past year | Settled once through the same formula, with evidence-tier discounts (100% / 85% / 50%), ratified by supermajority + non-founder majority, granted now at low FMV |
| Inactive founders | Keep what the Ledger says they earned; forfeit unearned reserve tranches; no confiscation, no forced exit; optional fair-value buyout |
| Professor | Written advisor agreement supersedes the oral promise: fixed 0.5–1.0% grant, 24-month vesting + Ledger access at his *documented* market rate; conditioned on Yale COI clearance and IP provenance; no manager role |
| Governance | Manager-managed; 3-seat Board (≥1 non-founder), annual election by Units; single CEO appointed/removable by Board; 3-tier decision matrix; formula changes need 66⅔% + majority of non-founder Units |
| Disputes | Negotiation → mediation → AAA arbitration (Boston); deadlock → appraised fair-value buyout; explicitly no shotgun clause |
| Compliance | Wage Act remediation first; Rule 701 compensatory plan papering; IP present-assignments; 83(b) hygiene |

---

## 3. Governance: how the company is run

### 3.1 A single accountable CEO — not five equal partners

Evidence, in order of strength:
- Founder *replacement* causally improves startup performance in the strongest-identified study in this literature (Ewens & Marx 2018, *RFS*, instrumented via noncompete-law changes [A20]) — meaning governance must be able to change leadership; leadership entrenchment is the anti-pattern.
- Founder control levers correlate with materially lower value: each level of founder control (CEO seat + board control) is associated with 17.1–22.0% lower pre-money valuation (Wasserman 2017, *SMJ*, N = 6,130, correlational [A14]).
- Truly co-equal co-leadership underperforms moderate power differentiation (Krause, Priem & Love 2015, inverted-U in co-CEO power gap [A15]); flat startups commercialize worse even when they ideate better (Lee 2022 [A18]). Counterpoint presented honestly: an HBR study of 87 co-CEO firms found outperformance (9.5% vs 6.9% returns) under strict conditions — complementary roles, explicit decision rights [A16] — and the hierarchy meta-analysis finds the *average* hierarchy effect on team effectiveness is slightly negative, positive only when hierarchy is legitimate and stable (Greer et al. 2018, 54 studies/13,914 teams [A17]).
- VCs weight team above everything (important for 95%, the single most important factor for 47% — Gompers et al. 2020, N = 885 VCs [A19]); a five-headed leadership structure is a team red flag they price.

Synthesis: one CEO, chosen and removable by a board, with legitimacy derived from a process everyone signed — that is the configuration the evidence supports (differentiated but legitimate and non-entrenched). Shared technical leadership survives below the CEO as ordinary management structure.

### 3.2 The Board of Managers

Three seats, annually elected by Units, at least one seat always held by a non-founder; CEO appointed by and serving at the pleasure of the Board.

- **Three** because odd numbers avoid deadlock and pre-seed norms run 1–3 founder-controlled seats, expanding to 2:1 at seed and 2-2-1 at Series A [S26]; building the habit of a functioning board now is cheap and signals maturity.
- **Elected by Units** (one Unit, one vote) because the ch. 156C default — voting by unreturned capital contributions — would hand control to whoever happened to put in cash, which contradicts the contribution-based design; the operating agreement must expressly override it (M.G.L. c. 156C §§21, 24 [L1]).
- **Non-founder seat** because it hard-codes the promise that founders and employees are on identical terms, materially strengthens the procedural-fairness record that Massachusetts fiduciary law rewards (Wilkes burden-shifting: legitimate purpose, least-harmful alternative [L3]), and previews the independent-seat structure investors will install anyway [S26].
- **Removability** of managers by majority of Units, and of the CEO by the Board, keeps control migratable — the Ewens & Marx lesson [A20] — without giving any founder a veto.

### 3.3 The decision matrix

Three tiers (ordinary / significant / fundamental — full table in the operating agreement, Art. III). The distinctive choice: **changes to the equity formula itself require 66⅔% of Units AND a majority of Units held by non-founders.** Rationale: (a) the formula is the constitution of this company — the thing that makes unequal outcomes legible and therefore safe (unexplained dispersion is what damages interdependent teams — Shaw 2014 [A11]); (b) founders as a bloc could otherwise rewrite it in their favor, which is both the classic freeze-out fact pattern Massachusetts punishes (Donahue; Allison v. Eriksson [L2][L4]) and exactly what a diligence lawyer would flag; (c) it makes the "identical terms" requirement self-enforcing rather than aspirational.

### 3.4 Entering and leaving roles

Managers: stand for election at ≥1% of Units; leave by non-reelection, resignation, or removal by majority of Units. CEO: appointed/removed by Board majority. Ledger Committee (verification body, §4.5): three members elected annually, ≥1 non-founder, ≤1 Board member — deliberately separate from the Board so the people who ratify budgets do not also audit their own hours. No role is reserved for founders as such; founder status confers exactly two things in this design — the 5% earnable reserve and nothing else.

---

## 4. The Contribution Ledger: defining, measuring, and converting contribution

### 4.1 The formula (spreadsheet-computable)

For each person *i*, month *m*:

```
CP(i,m) = Σ_roles [ verified_hours(i, role, m) × RateCard(role, m) ] × 2.0
        + [ cash_contributed(i,m) + FMV_property(i,m) ] × 4.0
Share_of_pool(i) = ΣCP(i) / ΣCP(everyone)     — floating until Crystallization
Equity(i) = 75% × Share_of_pool(i) + vested_reserve(i)   [reserve: founders only, §5]
```

Constraints: ≤60 logged hours/person/week; entries filed within 60 days; hours paid in cash earn no CP (no double-dipping); the advisor's hours cap at Yale's one-day-per-week limit.

### 4.2 Why hours × market rate, not negotiated weights or subjective scoring

Alternatives considered and rejected:
- **Negotiated static split** (Demmler founders-pie factor weighting [S24]): subjective weights re-import the negotiation problem and cannot cover ten employees "on identical terms."
- **Milestone/deliverable pricing:** objective in principle but requires pricing every task ex ante — unworkable at 15 people, and creates gaming at the task-definition step.
- **Peer-rating systems:** well-studied in org behavior but subjective, cliquable, and litigation-fragile in a company already carrying fiduciary risk.

Hours × published market rate is the only base that is (a) observable and auditable, (b) role-sensitive (an hour of ML architecture ≠ an hour of QA — priced by the market, not by argument), and (c) identical in form for everyone — which is what the fixed requirements demand and what the pay-dispersion literature requires: dispersion tied to legible market inputs is the kind that does not corrode interdependent teams (Shaw 2014 [A11]; Colquitt et al. 2001 meta-analysis: procedural justice drives system-level trust [A10]).

### 4.3 The Rate Card

Published table, by role and seniority, sourced from named benchmarks (Carta/Pave/BLS Boston market data [S13][S14]), adopted annually by the Board, prospective-only changes. The rate attaches to the **work actually performed**, not the title — a founder doing junior work logs at the junior rate. Specialist rates above the engineering bands (relevant to the professor) require *documented external evidence* of that person's market rate — invoices or engagement letters to third parties — otherwise the published academic-consulting benchmark applies. This single rule is what turns "he expects a higher rate" from a favor into data (§7).

### 4.4 The multipliers (2× non-cash, 4× cash) — and their honest status

The multipliers implement risk compensation: unpaid work and out-of-pocket cash are investments at total-loss risk, not salary. The 2×/4× values come from Slicing Pie, the dominant practitioner framework (Moyer [S22]); they have **no peer-reviewed validation** — nothing in the literature pins down 2 vs 1.5 vs 3. What matters, per the justice literature, is that the parameters are uniform, published, and adopted before anyone knows whose ox is gored. We adopt the practitioner standard because a Schelling-point convention beats a bespoke number nobody can defend either. (Bounded: multipliers apply to accrual, not to voting; and the formula-change supermajority in §3.3 protects them from opportunistic revision.)

We also adopt the documented *critiques* of Slicing Pie as design constraints [S23]: it fits only the pre-salary phase (→ hard freeze at Crystallization, §9); it relies on self-reported hours (→ evidence-linked logging + audit committee, §4.5); it creates tax events if run inside a C-corp (→ run it in the LLC phase only, convert after freezing [L11–L14]); and investors will not fund a floating cap table (→ freeze *before* the round, present investors a finished table [S23][S2]).

### 4.5 Verification: the anti-free-riding machinery

Social loafing is real, large (g ≈ 0.44 across 78 studies), and disappears when individual output is identifiable and evaluable (Karau & Williams 1993 meta-analysis [A12]); free-riding pressure inside real founding teams grows with team size and is checked by peer monitoring (Backes-Gellner et al. 2015, N = 214 teams [A13]). Design translation:
- every logged hour links to an artifact (commit, PR, doc, ticket, meeting note);
- the full Ledger — hours, roles, rates, CP, evidence — is visible to all members (identifiability);
- a 3-person elected **Ledger Committee** (≥1 non-founder) audits entries with **no discretion to re-weight** — it verifies evidence, period (procedural justice with no room for favoritism [A10]);
- 30-day challenge window after monthly publication; appeals to arbitration;
- quarterly Board ratification is ministerial (process check only).

### 4.6 The retroactive year (one-time settlement)

Same formula, applied backward, with evidence-quality tiers replacing what verification would have caught in real time: contemporaneous records → 100% of computed CP; corroborated by ≥2 members in writing → 85%; uncorroborated self-report → 50%, capped at 20 hrs/week. The tiers are this design's own construction (no literature directly on point — flagged); their function is to make the settlement *strictly evidence-ranked* so that founders and employees genuinely face identical terms — engineers with commit histories will fare well, and a founder whose year is unevidenced will not outrank them by status. Settlement is audited by the first elected Ledger Committee, ratified by 66⅔% of Units + majority of non-founder Units, then closed forever (fraud excepted). Grants are made now, while FMV is defensibly low, with appraisal support and protective 83(b)s — because a retroactive grant of a *capital* interest for past services is ordinary income at FMV under §83 [L10], and the one moment this is cheap is now.

### 4.7 Ongoing operation and the instrument question

Monthly logging → publication → challenge → quarterly conversion of CP into Units. Tax wrapper per person (operating agreement §2.2A): **Member Units** (profits interests under Rev. Proc. 93-27 / 2001-43 — nontaxable at grant, no tax on vesting, protective 83(b)s anyway [L8][L9]) or **Ledger Rights** (409A-compliant phantom units settling in stock at conversion) for contributors who need to stay W-2 once payroll starts — necessary because an LLC member cannot be a W-2 employee (Rev. Rul. 69-184 [L11]), and Wage Act remediation (§10) requires real payroll for real employees. Economics identical either way; "identical terms" is preserved in substance; counsel picks the wrapper per person.

---

## 5. The Founder Reserve: 5% each, genuinely earned

Fixed requirement: capped at 5% per founder, use-it-or-lose-it. Implementation:
- 16 quarterly tranches (0.3125%) over 4 years — matching the near-universal 4-year norm (~92% of venture-backed companies put founders on vesting; where there's a cliff, ≥95% are 1 year — Carta [S6]; NVCA model documents embed the same [S7]).
- Each tranche additionally requires that quarter's **Activity Test**: ≥20 hrs/week of Ledger-verified contribution, or a Board-certified deliverable plan for lumpy work. This is the "earned, not guaranteed" requirement made mechanical — no discretionary judgment, no confrontation, no committee vote on a person.
- **Missed tranches are forfeited to the Contribution Pool** — to everyone pro rata, not to the other founders. This choice does double duty: it removes any incentive for founder-bloc gamesmanship against a struggling founder (they gain nothing individually), and it is the "least harmful alternative" posture that Massachusetts fiduciary review rewards (Wilkes [L3]).
- Year One credit: up to 4 tranches vest retroactively, but only for quarters where the founder actually passes the test on the evidence tiers of §4.6.
- Acceleration: double-trigger only (change of control + termination without cause); single-trigger acceleration is investor-hostile and NVCA-nonstandard [S7][S8].
- Expect a partial **re-vesting negotiation at Series A** regardless (investors typically don't want founders more than ~40% vested at the first priced round [S8]); the schedule above is designed to be credible enough to survive that negotiation with credit for time served.

**Evidence status, honestly:** vesting's support is theoretical (contingent contracts mitigate team-formation inefficiency — Hellmann & Thiele 2015 [A7]) plus lab (contingent equity + delay improves sorting — Kagan et al. [A6]) plus overwhelming adoption data [S6][S7]; there is **no causal field study of founder vesting on outcomes** [A22]. It is nonetheless the single most investor-legible feature in this design.

---

## 6. Inactive founders

Every dimension, decided:

1. **Economics — past:** they keep every Unit their verified contributions earned. Work performed is work owned; clawing back earned equity from a disfavored member is the Donahue/Pointer freeze-out fact pattern (utmost good faith and loyalty; termination and exclusion can themselves be freeze-outs [L2][L5]) and would hand them a litigation claim that would sit in every future data room. Confiscation is both illegal-ish and — more relevantly here — *unfundable*.
2. **Economics — future:** the Ledger simply stops accruing for people who stop working, and unearned reserve tranches lapse into the pool. Time, not confrontation, resolves the imbalance: an inactive founder's percentage shrinks monotonically as others' CP grows. This is the design's core answer to dead equity — prevented by dilution-through-contribution rather than cured by expropriation. (Dead equity is the #1 named cap-table red flag [S1][S2]; ~23% of startups lose a co-founder within 3 years [S3], so the mechanism will very likely be exercised.)
3. **Governance:** voting tracks Units, so influence fades proportionally; board eligibility requires ≥1% and election; committee seats require election. No special disenfranchisement — none needed.
4. **Status and information:** they remain members with full information rights. Stripping information rights from a member invites exactly the equitable remedies Allison v. Eriksson authorizes beyond appraisal [L4].
5. **Exit:** optional, mutual fair-value buyout (appraised, no minority discount, payable over time by note) — offered, never forced. [Open point: a company call right at fair value after N quarters of zero contribution is defensible but fiduciary-sensitive; flagged for counsel rather than assumed.]
6. **Unanimity at signing:** the settlement is structured so inactive founders rationally sign — they receive their earned history cleanly documented, keep upside via retained Units, avoid litigation, and their alternative (an oral equal-split claim against a company with treble-damage wage exposure) is worth little. Unanimous adoption moots most fiduciary attack vectors [L4]; if unanimity fails, counsel must advise on the majority-amendment path *before* proceeding — flagged as the single largest legal-risk decision in the project.

---

## 7. The professor

The promise was "a decent share," informal, with an expectation of a premium rate for part-time involvement. The market says: median advisor grants are 0.21% at pre-seed and only ~10% of pre-seed advisors get ≥1% (Carta H1 2024 [S16]); the FAST framework tops out at 1.0% for an "Expert" advisor at idea stage, vesting monthly over ~2 years [S15]; scientific-advisory-board norms for professors run 0.1–0.5%, with 0.25–1% for deeply engaged names (Atlas Venture / law-firm guides [S17]).

Design: **(a)** a fixed grant of **[0.5–1.0]%** — top-of-band, defensible as "decent" precisely because it is anchored to published grids rather than to feelings — vesting monthly over 24 months against a written advisor agreement; **(b)** open Ledger participation at his **documented** external consulting rate (the specialist-rate rule, §4.3), which honors "valued at a higher rate" the only way that survives the pay-dispersion evidence: as *explained*, verifiable market dispersion, applied through the identical formula [A11]; **(c)** hours capped at Yale's one-day-per-week external-activity limit; **(d)** all of it conditioned on Yale COI disclosure/clearance and IP provenance certification — Yale owns faculty inventions arising from Yale research and litigates the point (Yale Patent Policy; Fenn v. Yale [L16]); any Yale-derived IP must arrive via a Yale license, not as his personal contribution; **(e)** no manager title and no board seat — Yale restricts management roles in for-profits [L15], and MA Wage Act liability attaches personally to those "having the management" of the company [L6].

If he declines these terms, the company should conclude the promise was never performable and document the offer — a paper trail of a market-standard offer refused is diligence-safe; an unresolved oral promise is not (promissory-estoppel risk is real in MA given a year of reliance [L19] — hence the release-for-grant exchange in the operating agreement).

---

## 8. Governance of disagreements

Escalation ladder: principals (14 days) → mediation, Boston (30 days) → binding arbitration, single arbitrator, AAA, Boston — enforceable under the FAA and M.G.L. c. 251, valued for speed and confidentiality (reputational protection matters to a company that will be raising) [L20][S26]. Ledger disputes get the same ladder after the committee process, and the arbitrator applies the formula — no equitable re-slicing, or the objectivity promise unravels. Deadlock (board or fundamental vote, 60+ days, operations-threatening): appraised fair-value buyout process. **No shotgun clause**: shotguns systematically favor the wealthier party, signal founder-conflict risk to VCs, and in a Donahue jurisdiction an opportunistic shotgun against a cash-poor member is itself fiduciary-attackable [S25][L21]. Vesting + board mechanics + drag-along are the venture-standard substitutes [S25].

---

## 9. Entity, tax, and the investor path

**Now:** stay a Massachusetts LLC through formalization — it is already formed, tolerates a floating cap table (a C-corp running Slicing Pie generates taxable events on every shift [S23]), and supports profits interests (nontaxable at grant under Rev. Proc. 93-27/2001-43 [L8][L9]). Costs acknowledged: $500/yr MA fee, K-1 complexity, SE tax for members [L11].

**Then:** at Crystallization — the earliest of a ≥$1M priced round, a fundamental-vote decision, or 36 months — freeze the Ledger and convert to a **Delaware C-corporation**, because that is a hard gate, not a preference: VC funds' tax-exempt LPs can't hold pass-throughs (UBTI), SAFEs and preferred-stock mechanics assume corporate stock, ISOs require a corporation, QSBS applies only to C-corp stock, and YC's standard deal simply requires it [S18][S21]. Mechanics: ch. 156C has no clean outbound-conversion provision, so plan a **merger into a new Delaware corporation** (§§59–63), assets-over under Rev. Rul. 84-111, tax-free under §351 with the usual traps (§357(c), negative capital accounts) checked first [L12][L13]. Members pre-commit to the conversion via a cooperation covenant — a holdout veto over investor-required restructuring is itself a diligence flag, and Allison teaches that conversions executed *over* a dissenter invite equitable unwinding, so consent is banked now, not sought later [L4].

**QSBS timing (a genuine tension, decided):** conversion stock takes an FMV basis for the 10×-basis cap (arguing for converting *later*, after appreciation), but the holding clock — now tiered 50/75/100% at 3/4/5 years with a $15M cap and $75M asset ceiling under the 2025 OBBBA for post-July-4-2025 stock [S19][L14] — starts only at conversion (arguing for *earlier*). Decision: convert at the first priced round and no later than 36 months. Rationale: for a company whose stated objective is venture financing, the certainty of starting every holder's clock (founders' and future employees' alike) dominates speculative basis optimization, and the round itself forces the freeze anyway. Model both paths with the CPA at the time; flagged as a genuine judgment call.

**Securities:** paper the Ledger as a written compensatory plan → Rule 701 (available to non-reporting LLCs) / §4(a)(2); confirm the MA compensatory blue-sky exemption; never mix compensation grants with a cash raise (that goes 506(b) with Form D + MA notice) [L17][L18].

---

## 10. The Wage Act problem (gating item)

The single largest quantified legal risk found: ~10 workers unpaid for up to a year in Massachusetts means accruing claims carrying **strict-liability treble damages** (even good-faith late payment before suit — Reuter v. City of Methuen, 489 Mass. 465 (2022) [L6]), 3-year lookback, 12% interest, fees, and **personal liability** for the individuals managing the company [L6][L7]. Equity does not cure it: wage deferral by agreement is a void "special contract" (Stanton v. Lighthouse, D. Mass. [L7]); for-profit "volunteering" is not a thing; and the workers almost certainly fail the ABC contractor test (Prong B — they do the company's core work) [L7]. Every payday missed is a fresh violation.

Sequenced remediation (counsel-led, before or with signing): sort all ~15 people into bona fide members (genuine equity + governance participation — the member/employee line for token grants is fact-intensive and flagged), payroll employees (≥ $15/hr going forward), or paused; quantify accrued exposure; pair back-pay with individually negotiated releases (their enforceability for Wage Act claims is itself a counsel question); and only then execute the equity settlement. The design's phantom-unit option (§4.7) exists precisely so employees can hold full Ledger economics while staying lawful W-2 employees.

Why this leads the design rather than footnoting it: an unremediated Wage Act exposure is a contingent liability with treble multiplier and personal founder liability sitting in the middle of every future financing — the opposite of investor-attractive.

---

## 11. Where the evidence is thin, and where it disagrees

Presented per the task's standards:

1. **Equal splits: academia vs. YC.** Hellmann & Wasserman find quick equal splits associated with worse financing outcomes [A1]; Michael Seibel/YC advises splitting (near-)equally [S27]. The reconciliation — visible in both sources' fine print — is that the academic result is driven by *quick, negotiation-free* splits (selection), and YC pairs equality with vesting and deliberate discussion. This design is consistent with both: it replaces a stale handshake with a deliberate, information-rich allocation, and its outputs may well land near-equal for founders who contributed near-equally.
2. **Hierarchy.** The meta-analytic average effect of hierarchy on team effectiveness is slightly *negative* [A17]; the co-CEO and founder-control literatures cut the other way for leadership specifically [A14][A15]; HBR's co-CEO sample outperformed [A16]. Design response: differentiated-but-legitimate authority (elected board, removable CEO), which is the configuration all three literatures tolerate.
3. **Dynamic equity end-to-end: no peer-reviewed validation exists** [A8]. The framework here is practitioner machinery (Slicing Pie [S22]) bounded by its published critiques [S23] and by academic evidence on its load-bearing components (delay/information [A6], identifiability [A12], legible dispersion [A11], procedural justice [A10]). The 2×/4× multipliers and the 100/85/50 evidence tiers are convention and construction respectively — labeled as such, protected from abuse by supermajority entrenchment rather than by any claim of scientific precision.
4. **Founder vesting:** universal in practice [S6][S7], theoretically grounded [A7], causally unproven [A22].
5. **Retroactive renegotiation:** essentially no direct literature; nearest anchors are renegotiation-obstacle discussions [A1-WP] and the delay-improves-sorting lab result [A6]. The evidence-tier mechanism is our construction.
6. **Legal unknowns for counsel** (from the legal research, flagged not resolved): direct MA-LLC→DE-corp statutory conversion availability; enforceability of private Wage Act releases; the member-vs-employee line for token equity holders; Cook v. Patient EDU and Stanton citations to be confirmed; MA compensatory blue-sky exemption scope for profits interests; arbitrability of member fiduciary claims; any §469 passive-loss disclosures for inactive members.

---

## 12. Decision register (open points carried into the operating agreement)

| # | Decision | Recommendation | Where |
|---|---|---|---|
| 1 | Multipliers | Keep 2×/4× (practitioner standard) | OA §4.2 |
| 2 | Advisor fixed grant | 0.75% (midpoint; FAST-Expert-adjacent) | OA §6.2 |
| 3 | Corroborated-tier discount | 85% | OA §4.5 |
| 4 | Uncorroborated tier | 50%, 20 hr/wk cap | OA §4.5 |
| 5 | Activity test threshold | 20 hr/wk or certified deliverables | OA §5.2 |
| 6 | Board election method | Cumulative voting (protects employee bloc) | OA §3.2 |
| 7 | Reserve acceleration | Double-trigger, 100% of remaining | OA §5.5 |
| 8 | Crystallization outer bound | 36 months | OA §9.1 |
| 9 | Option pool at conversion | 12–15%, sized bottom-up from hiring plan [S9][S10] | OA §9.3 |
| 10 | Buyout call on long-inactive members | Do not adopt without counsel sign-off | OA §4.7/§6 |
| 11 | For-cause forfeiture reach | 12-month trailing CP, 50% default | OA §4.7 |
| 12 | Instrument per person (Units vs phantom) | Individual election with tax advice | OA §2.2A |
| 13 | Unanimity fallback | Do not proceed non-unanimously without written counsel risk opinion | OA signature block |

---

*Citation keys: [A#] = academic sources, [S#] = industry sources, [L#] = legal authorities — all resolved, annotated, and strength-rated in `plan-10-references.md`.*
