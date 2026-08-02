# plan-7 — Full Governance & Equity Framework
### For a 1-year-old Massachusetts LLC: 5 founders, ~10 employees, all unpaid; one part-time academic advisor promised "a decent share"

**Team:** plan7 · **Date:** 2026-08-02
**Companion documents:** `plan-7-one-pager.md` (summary), `plan-7-operating-agreement.md` (article-by-article business-terms draft), `plan-7-references.md` (annotated bibliography with per-source evidence ratings and URL-verification status).

**Isolation note:** This work was produced on an orphan branch created from an empty tree. No other team's branch, file, or content was read at any point.

**Evidence-verification caveat (applies to every citation herein):** the research environment's egress proxy blocked direct fetches to all non-GitHub hosts, so all URLs except one were verified through the live search index (URL + matching content excerpt) rather than fetched byte-for-byte. Per-source verification status is recorded in `plan-7-references.md`. Figures that reached us only through secondary summaries are marked ⚠ in that file.

---

## Part 0 — How to read this document

The founders fixed four requirements: (1) a 5%-per-founder reserved allocation that must be **earned**; (2) all remaining equity through an **objective contribution system with founders and employees on identical terms**; (3) **maximum attractiveness to future investors**; (4) a **business-terms design for counsel**, not statutory drafting. Everything else was open. Part 1 states what the research actually found, including where it disagrees with itself. Parts 2–9 are the design, each choice tied back to Part 1. Part 10 is an honest statement of the limits of the evidence.

---

## Part 1 — What the research found

### 1.1 Founder equity splits: the academic record

- About **one-third of founding teams split equity exactly equally** (32% in Hellmann & Wasserman's 511-venture CompStudy sample, *Management Science* 2017), and **73% of teams settle their split within the first month** of founding, before uncertainty about commitment is resolved (Wasserman, *The Founder's Dilemmas*, 2012).
- Teams that split equally **and** negotiated for a day or less ("quick handshake") show a significant penalty at first financing — lower probability of raising and lower pre-money valuation, with the value at stake around **10% of firm equity (~$450K NPV, ~25% of an average founder stake)** (Hellmann & Wasserman 2017). The authors are explicit that this is **selection, not proven causation**: conflict-avoidant teams both split quickly and fundraise worse.
- In 24,194 German startups, unequal-split teams grew ~**1.3 percentage points faster over 3 years**, but **survival rates were the same** as equal splitters (Hennicke & Mueller, *European Management Journal* 2024). Equal splits correlate with slower growth and worse first-round terms — not with death.
- Lab evidence (Kagan, Leider & Lovejoy, *Management Science* 2020, randomized): equal-split contracts attract and shelter free-riding types; the authors recommend **delaying final contracting until teammates' types are revealed** — which is precisely the position this company is in after one revealing year.
- Process matters as much as numbers: in the only dedicated process study (Breugst, Patzelt & Rathgeber, *JBV* 2015, 8 teams over 6 months), **perceived justice of the split — not the split itself — drives positive or negative team spirals**; Wasserman's data adds that teams that split "by default" without real negotiation were **~3x more likely to be unhappy** with the split later.
- Theory: a 5-way budget-balanced sharing rule is exactly the structure Holmström's "Moral Hazard in Teams" (1982) proves under-provides effort; Kandel & Lazear (1992) show peer pressure counteracts free-riding best in **small, mutually-monitoring groups**; a 214-team empirical test finds founder effort follows an **inverted U in team size** — five founders sits where free-riding pressure is material (Backes-Gellner et al., *J. Business Economics* 2015).
- **The practitioner world disagrees with itself.** Y Combinator (Michael Seibel) argues for equal or near-equal splits because value comes from the *next* 7–10 years, not the first months. Frank Demmler ("splitting equally is a recipe for failure") and Mike Moyer (Slicing Pie) argue for contribution-weighted splits. Carta's data shows equal splits *rising* (45.9% of two-founder teams in 2024 vs 31.5% in 2015). We present this conflict rather than hide it — and note that the founders here have already chosen the contribution-weighted side by fixed requirement (2), and their situation (diverged contributions, unpaid year, employees out-contributing founders) is squarely the fact pattern the equal-split camp's advice assumes away.

**Bottom line used in the design:** a renegotiated, contribution-based, dynamic split with strong procedural fairness is the best-supported answer *for this fact pattern* — supported by the delay-contracting experiment, the quick-handshake penalty, the unhappiness data, and incentive theory — while acknowledging that no rigorous study yet evaluates dynamic-split mechanisms' outcomes directly (a real evidence gap, stated plainly).

### 1.2 Contribution-measurement systems: the practitioner record

- **Slicing Pie (Moyer)** is the only widely used fully specified dynamic model: *slices = fair market value of the contribution × a risk multiplier* — canonically **2x for non-cash (time, IP, equipment) and 4x for cash**; time is valued at fair-market salary ÷ 2,000 hours; only at-risk (unpaid) value earns slices; the pie **freezes at breakeven or a priced round**, when the company can pay market compensation and nothing further is at risk.
- **Critiques from startup lawyers** (Sentient Law; Lloyd & Mousilli; Equity Matrix): the fairness logic is not disputed; what is disputed is (a) enforceability if the ledger isn't kept, (b) tax mechanics in corporations (continuous share adjustment can create taxable events — *works cleanly only in LLCs*), and (c) investor acceptance — **VCs require a fixed cap table, so the pie must freeze before a round**. All three critiques are absorbed into this design (LLC now, disciplined ledger, hard freeze at conversion).
- **Static alternatives** (Demmler's Founders' Pie Calculator; foundrs.com; Gust) are one-time weighted-scoring negotiations — useful cross-checks, but they cannot satisfy requirement (2)'s "ongoing objective system."
- **Market benchmarks for scale-checking outputs:** Carta (8,000+ first-10 grants, 2023–24): median first hire ~**1.49%**, hire #5 ~**0.33%**; Polovets' 2014 AngelList data for *low/no-salary* early hires: **0.5–3%** — the better analog for this company's unpaid employees. Median seed option pool **12.1–12.5%** (Carta); Index Ventures recommends ~12% at Series A. Founder vesting is near-universal: **~92% of venture-backed companies** impose it; standard is **4 years, 1-year cliff, monthly thereafter** (Carta).
- **Retroactive sweat valuation:** consensus base = fair-market salary rate × hours (BLS OEWS May 2024: software developers median **$133,080/yr ≈ $66.50/hr**; 10th pct $79,850 ≈ $40/hr; 90th pct $211,450 ≈ $105/hr). No consensus multiplier exists; **2x is the most-cited figure** (Slicing Pie non-cash; "Convertible Sweat"), with guides ranging 1.5x–3x.

### 1.3 Governance and leadership: the evidence, honestly stated

- **Shared-leadership meta-analyses are real and positive** (Wang et al. 2014, 42 samples, ρ ≈ .34; D'Innocenzo et al. 2016, 3,198 teams) — but they measure shared leadership *behaviors*, not the absence of a formal leader. The startup-specific study (Ensley, Hmieleski & Pearce 2006; 66 Inc. 500 firms + 154 random startups) finds vertical (CEO) leadership and shared leadership **both** predict performance — they are complements, not substitutes.
- **Co-CEO evidence cuts both ways:** an HBR/consultant study of 87 public co-CEO firms found **9.5% vs 6.9%** annual shareholder returns vs index (small N, heavy selection); but the strongest strategy-journal study (Krause, Priem & Love, *SMJ* 2015, 71 co-CEO pairs) finds performance *rises with the power gap between co-CEOs* — i.e., even within shared structures, **unity of command wins**; and Korean panel data (Yoo & Lee 2021) shows co-CEO adoption is often a symptom of trouble, not a cause of success.
- **Decision speed:** Eisenhardt (*AMJ* 1989) — fast, high-performing teams in high-velocity markets used **"consensus with qualification"**: seek consensus quickly; if it doesn't emerge, **the CEO decides after consulting the relevant experts**. Pure autocracy breeds politics and underperformance (Eisenhardt & Bourgeois 1988); pure consensus is the maximally conservative architecture that systematically rejects good projects (Sah & Stiglitz 1986); decision speed predicts subsequent growth and profitability in 318-CEO longitudinal data (Baum & Wally 2003). Single-leader risk is also real: overconfident CEOs destroy value in acquisitions (Malmendier & Tate 2005/2008) — the check is a real board, not a committee of five.
- **Founder control is priced:** each additional level of founder control retained (CEO seat and/or board control) is associated with **17–22% lower pre-money valuation** (Wasserman, *SMJ* 2017); by year 3, half of founders are no longer CEO (Wasserman 2008). Founder *replacement*, instrumented causally, **improves** startup performance (Ewens & Marx, *RFS* 2018) — the mechanism must make leadership replaceable.
- **What investors will impose anyway:** seed boards of 3 (2 founders : 1 investor), Series A boards of 5 (2-2-1 with an independent tie-breaker); NVCA model documents implement board composition via a voting agreement plus protective provisions; the independent director typically joins after the second financing and holds the swing vote (Ewens & Malenko, *J. Finance* 2025).
- **Deadlock:** the ABA-endorsed ladder is negotiation → mediation → arbitration/tie-breaker → buy-sell → dissolution. Shotgun (Texas buy-sell) clauses are theoretically fair but **empirically rarely triggered** and favor the better-financed party (Brooks, Landeo & Spier, *RAND* 2010) — a deterrent of last resort, not a routine tool.
- **Team size warning:** no credible source endorses 5 co-equal founders as optimal; practitioner consensus centers on 2–3, and solo-vs-team evidence is genuinely mixed (Greenberg & Mollick 2018 vs. First Round/Startup Genome ⚠). The design therefore does not try to preserve five co-equal principals; it lets contribution and election sort standing.

**Bottom line used in the design:** one accountable CEO operating "consensus with qualification," under a small elected board that can remove them, with shared-leadership *behaviors* institutionalized (role charters, open information), and an automatic sunset into the NVCA-standard structure at financing.

### 1.4 The professor: advisor-market and Yale-specific findings

- Benchmarks: FAST agreement expert tier at pre-seed = **1.0%** (2-year vest); **Carta medians are far lower — 0.21% pre-seed, 0.12% seed**, with only ~10% of pre-seed advisors at ≥1%; Holloway: most common **0.25–0.5%**, 2-year monthly vest, 3-month cliff. The **part-time academic co-founder** norm (stays in academia, ~1 day/week) is **~5%**, with guidance that academic cofounders should stay ≤10% unless hands-on (Osage University Partners; YC spinout guidance). Biotech SAB analog: **0.1–0.3% + $2.5–5K/day cash** (Bruce Booth).
- Rates: elite ML consulting is commonly quoted at **$300–600/hr** (vendor surveys, weak quality); the survey-grade anchor is SEAK's expert-witness study: **median $450–500/hr**. A premium *rate* for a star contributor is exactly what a fair-market-value system produces natively — no special class needed.
- **Yale constraints:** external activities capped at ~**one day per seven per week**; faculty typically may not manage outside entities day-to-day; annual COI disclosure required; **Yale's patent policy claims inventions made under university auspices**, and a consulting invention can be assigned to the company **only if** Yale Ventures deems it unrelated to the professor's Yale research and made without Yale resources — a very hard test for an ML professor advising an ML startup in his own field. Yale enforces this against star faculty (*Fenn v. Yale*, D. Conn. 2003 — Nobel laureate; reassignment plus ~$1M).
- **The informal promise is a live liability:** oral equity promises are litigated under promissory estoppel, quantum meruit, and implied contract; full performance can defeat statute-of-frauds defenses (*Zakk v. Diesel*, Cal. App. 2019). Best practice: supersede the oral promise with a signed agreement containing an integration clause.

### 1.5 Legal/tax structuring: what is settled and what is dangerous

- **Settled norms (execute, don't debate):** institutional VCs require a **Delaware C-corp** (UBTI/blocker logic for tax-exempt LPs; ISOs exist only for corporate stock; Chancery predictability). Convert **before the priced round at low valuation**: §351 makes it generally tax-free; the **QSBS (§1202) clock starts at conversion with basis = FMV at conversion**, so only post-conversion appreciation is excludable — another reason to convert early. Post-OBBBA (stock issued after July 4, 2025): per-issuer cap **$15M** (or 10x basis), tiered exclusion **50%/75%/100% at >3/4/5 years**, gross-asset ceiling **$75M**. 83(b) elections have a hard **30-day** deadline; options require a **409A** valuation.
- **LLC advantages worth keeping until conversion:** profits interests (Rev. Proc. 93-27 / 2001-43) are **tax-free at grant** and ideal for the go-forward contribution engine; dynamic percentage adjustment among members is clean in an LLC and messy in a corporation — the lawyers' own critique of Slicing Pie says it "works cleanly in LLCs."
- **The Massachusetts Wage Act is the single most urgent finding of this entire research effort.** M.G.L. c.149 §148 + §150: earned wages due within 6 days of period end; **mandatory treble damages**, attorneys' fees, 3-year lookback; **strict liability** even for good-faith lateness (*Reuter v. Methuen*, SJC 2022); **personal liability for LLC managers** who direct policy (*Cook v. Patient Edu*, SJC 2013); **deferral agreements are void** as "special contracts," and a startup co-founder's deferred salary was held to be "wages" (*Stanton v. Lighthouse*, D. Mass.); minimum wage **$15.00/hr** (c.151); the §148B **ABC test** (presumption of employment; prong B nearly impossible for core-work startup staff) blocks the "call them contractors" escape. Ten unpaid employees = a treble-damage claim accruing daily, personally against the managing founders. This design cannot fix that; Part 9 sequences the remediation counsel must lead.
- **Squeezing out inactive founders is legally fraught in Massachusetts.** Close-corporation owners owe each other "**utmost good faith and loyalty**" (*Donahue v. Rodd*, SJC 1975); adverse action against a minority owner requires a **legitimate business purpose** with no less-harmful alternative (*Wilkes v. Springside*, SJC 1976); and in LLC freeze-out mergers minority members get equitable remedies beyond the statutory exit (*Allison v. Eriksson*, SJC 2018) — which directly reaches a Delaware conversion used to strip an inactive founder. Consequence for design: **take only unearned equity, never earned equity; get unanimous written consent to the new agreement; paper the legitimate business purpose.**

---

## Part 2 — Entity and tax path

**Decision 2.1 — Remain a Massachusetts LLC now; commit contractually to convert to a Delaware C-corporation at the Freeze Event (defined in 3.6).**
Rationale: the contribution engine requires continuous re-percentaging, which is tax-clean only in an LLC (§1.5); profits interests give employees tax-free-at-grant equity now; conversion before the first priced round at low valuation is the settled investor-readiness norm and starts the QSBS clock on favorable terms. The operating agreement pre-wires the conversion (obligation, mechanics, vote threshold) so no member can hold it hostage later — with the *Allison* fiduciary caveat flagged for counsel (Part 10 and OA Art. XIII).

**Decision 2.2 — Unit structure while an LLC:**
- **Class A Units ("Earned Units")** — full economic + voting units held as earned under Parts 3–4. Issued as **capital interests** for the retroactive Year-1 allocation (taxable at grant; do it now while FMV is low, with a supporting valuation — counsel/tax item), and as **profits interests** (Rev. Proc. 93-27/2001-43, hurdle = current FMV, protective 83(b) within 30 days) for go-forward accrual.
- **No separate "founder class."** The founder reserve is a *quantity* of future Class A Units per founder, not a superior class — one class of economic rights keeps the cap table investor-clean.
- Employees receiving units become members receiving K-1s (they lose W-2 status — a real administrative cost, disclosed to them in writing; the phantom-unit alternative is bracketed in OA Art. IV for counsel).

**Decision 2.3 — Conversion mechanics (for counsel):** Delaware-side conversion under DGCL §265 or a c.156C §§59–63 merger into a new DE corp (member approval default: >50% of unreturned contributions); §351 non-recognition check including §357(c) liabilities-over-basis; Rev. Rul. 84-111 form choice; profits interests exchanged for common stock preserving vesting; 409A-consistent valuation at conversion; QSBS documentation from day one.

---

## Part 3 — The equity engine (spreadsheet-computable)

### 3.1 Overview

Total equity = **25% Founder Reserve** (5% per founder, earned; Part 3.5) + **75% Contribution Pool** (Part 3.2–3.4). Until the Freeze Event both are tracked in a **Contribution Ledger**; ownership percentages at any date are computed from the ledger. At the Freeze Event percentages crystallize into the fixed cap table (3.6).

### 3.2 Contribution Units — the formula

For each person *i* and month *m*:

```
ContributionUnits(i,m) =
    Hours(i,m,activity) × Rate(activity, band) × M_noncash        [time]
  + CashOut(i,m) × M_cash                                         [cash spent / unreimbursed expenses]
  + FMV(other accepted contribution) × M_noncash                  [equipment, pre-existing IP — Board-accepted FMV]
```

- **M_noncash = 2.0; M_cash = 4.0** (Slicing Pie canonical multipliers — the single most-cited practitioner standard; the honest caveat that no peer-reviewed validation of these exact numbers exists is recorded in Part 10).
- Any cash compensation actually paid for the period reduces the at-risk time value dollar-for-dollar before multiplication (only at-risk value earns units).
- Cash *committed but unspent* earns nothing until spent (Slicing Pie "Well" rule).
- A person's **Pool share** at any time = their cumulative ContributionUnits ÷ all ContributionUnits, × 75%.

### 3.3 The Rate Table (identical for founders and employees — fixed requirement 2)

Rates are **role-of-the-work** rates, not role-of-the-person rates: one person logging both coding and management logs each activity at that activity's band. Anchors: BLS OEWS May 2024, software developers (SOC 15-1252): 10th pct $79,850; median $133,080; 90th pct $211,450; ÷ 2,000 hours.

| Band | Covers | Annual FMV anchor | Hourly rate |
|---|---|---|---|
| E1 | Junior engineering work | $80,000 | **$40/hr** |
| E2 | Core engineering work (default) | $133,000 | **$66.50/hr** |
| E3 | Staff-level engineering / engineering management | $211,000 | **$105/hr** |
| B1 | Business planning, ops, admin | $133,000 | **$66.50/hr** |
| X1 | Recognized outside-expert advisory (see Part 6) | $400/hr × hours | **$400/hr** [$300–$500 bracket] |

- Band assignment per person per activity is set annually by the Board against the published anchors, appealable to the arbiter (Part 8). Nobody sets their own band.
- **Deliberate design choice:** "vision"/CEO-type work is priced at E3, not at a premium CEO band. The literature gives no defensible market rate for founder "vision," and premium self-priced bands are exactly the procedural-injustice trigger Breugst et al. warn about. Leadership is rewarded through the reserve, election to responsibility, and the larger pie — not a private rate.
- Rate table re-anchors annually to the then-current BLS OEWS release (mechanical update, no vote needed).

### 3.4 Logging, acceptance, transparency

- Hours logged weekly in a shared system; entries older than 30 days are inadmissible (prevents retro-padding).
- The CEO (or a Board-designated administrator) accepts or challenges entries monthly; challenges go to the Board, then the arbiter. Silence for 60 days = accepted.
- **The full ledger and everyone's running percentage are visible to all members monthly.** This is the procedural-justice mechanism the evidence says matters most (Breugst et al. 2015; Wasserman's "unhappiness" data): fairness must be *seen* continuously, not discovered at a crisis.

### 3.5 The Founder Reserve — 5% each, earned monthly, use-it-or-lose-it

- Each founder's 5% reserve vests **1/48th per month over 48 months** from the Effective Date, **but only in months where the founder meets the Active Founder Standard: ≥80 accepted contribution-hours in that month** (≈ half-time). A missed month's tranche is **permanently forfeited to the Contribution Pool** — not paused, not recoverable. That is "use it or lose it" made literal, and forfeitures flow to the people doing the work, not to the other founders' reserves.
- **Retroactive credit:** for each Year-1 month in which a founder's evidence-based activity (Part 4 banding) was ≥ half-time, one tranche vests at signing. A founder fully active for the whole first year therefore starts ~25% vested — matching the investor-standard "retroactive vesting credit for time served" norm (§1.5) — while a founder inactive since month 4 starts with ~3–4 tranches and forfeits the rest month-by-month unless they return to the standard.
- The reserve is the *only* founder-specific economic right in the company. Everything else — pool units, board eligibility, officer roles, voting — is identical for founders and employees.
- On any founder's death or disability, unvested reserve tranches terminate without fault-based forfeiture of earned units [bracketed compassion carve-out: up to 6 months' tranches vest — OA Art. V].

### 3.6 The Freeze Event and after

- **Freeze Event** = the earliest of: (a) closing of a priced equity financing ≥ $[1,000,000]; (b) the Delaware conversion; (c) three consecutive months of cash-flow breakeven with all staff paid ≥ fair-market cash compensation; (d) a member-approved sale. Rationale: the pie exists to price *at-risk* contribution; when people are paid market rates, nothing further is at risk (Slicing Pie freeze logic; VC fixed-cap-table requirement).
- At the Freeze: ledger closes; percentages crystallize; on conversion each member receives common stock pro rata (vesting carries over); a new **option pool of [12.5]%** (Carta median seed pool 12.1–12.5%) is created for post-freeze hires and refreshes; all post-freeze compensation moves to salary + standard grants.
- **Worked example** (illustrative numbers a spreadsheet reproduces; full-time = 2,000 hrs/yr at E2 unless noted):

| Person | Year 1 (banded) | Year 2 (logged) | Cash spent | Units (Y1+Y2+cash) |
|---|---|---|---|---|
| Founder A (active, E3 mgmt half her time) | 2,000h → 343,000* | 2,000h → 343,000* | $20,000 → 80,000 | 766,000 |
| Founder B (active, E2) | 2,000h → 266,000 | 2,000h → 266,000 | — | 532,000 |
| Founder C (went inactive month 6, E2) | 900h → 119,700 | 0 | — | 119,700 |
| Founder D (quarter-time, E2) | 500h → 66,500 | 500h → 66,500 | — | 133,000 |
| Founder E (inactive since month 3, E2) | 400h → 53,200 | 0 | — | 53,200 |
| Employee 1 (full-time, E2) | 1,500h → 199,500 | 2,000h → 266,000 | — | 465,500 |
| … employees 2–10 similarly … | | | | |
| Professor (X1, 100h/yr) | 100h → 80,000 | 100h → 80,000 | — | 160,000 |

*A: (1,000h × $105 + 1,000h × $66.50) × 2 = 343,000. Each person's share of the 75% pool = own units ÷ total units. Note the system's automatic verdicts: Employee 1 out-owns three of five founders from the pool — exactly what fixed requirement (2) demands; Founder E ends with pool units ≈ 0.3–0.5% of the company plus only the reserve tranches earned before going inactive.

### 3.7 Departures and recovery (pre-freeze)

- **Any departure:** earned Class A Units (vested reserve + accrued pool units) are **kept**. This deliberately rejects Slicing Pie's harsher rule stripping a bad leaver's non-cash slices: under *Donahue/Wilkes*, confiscating earned equity from a minority member is a freeze-out claim waiting to happen (§1.5). Unvested reserve and future accrual stop — that is loss enough, and it is legally defensible because it takes only the *unearned*.
- **Termination for Cause** (narrowly defined: fraud, conviction, material IP breach, willful and continued failure after written notice + cure period): company gains a **buyback option** on the departed member's units at independently appraised fair value [bracketed: minus a [20]% illiquidity discount — counsel must test against *Wilkes*]. For-cause determinations require a Board vote **plus** the arbiter's confirmation if contested.
- Company right of first refusal on all transfers; no transfers except to estates/trusts without Board consent; drag-along at the Fundamental-Decision threshold; tag-along for all members (OA Art. X).

---

## Part 4 — Pricing the unpaid Year 1 (retroactive, without time records)

Nobody logged hours in Year 1, so the design refuses false precision and uses **coarse banding + artifact corroboration + blind peer rating**:

1. **Claim.** Each person (founders, employees, professor) files a Year-1 Contribution Claim: months involved, an involvement band per month, activity mix, cash outlays, and pointers to evidence (git/PR history, design docs, calendar records, shipped work, receipts).
2. **Bands** (annualized): Full-time = 2,000h · ¾ = 1,500h · ½ = 1,000h · ¼ = 500h · Minimal = 100h · None = 0. Banding is robust where hour-recall is not: outcomes turn on differences everyone can verify (full-time vs. checked-out), not on ±200 hours. Bands feed the 3.2 formula exactly like logged hours.
3. **Blind peer rating.** Every member independently bands every other member (self excluded) before seeing others' claims. The panel median is the presumptive band.
4. **Reconciliation.** Claim vs. peer-median vs. artifacts: agreement within one band → settled at the *lower* of claim and peer median [bracketed: at the peer median]. Larger gaps go to the **Neutral Arbiter** (Part 8) whose banding decision is final. Undocumented, unratified claims earn nothing.
5. **Cash** outlays require receipts; they convert at 4x regardless of band.
6. Output: each person's Year-1 ContributionUnits, entered as opening ledger balances, published to all members, and — critically — **released**: signing the operating agreement ratifies the Year-1 allocation and (subject to counsel's advice on what is releasable, esp. Wage Act claims, which likely are **not** privately releasable — Part 9) waives further claims to pre-signing equity, superseding every informal promise, including the professor's.

**Legal flag:** retroactive units are compensation for past services — a taxable grant of capital interests. Doing this at today's (low) FMV with a supporting valuation minimizes the tax; counsel + CPA must paper it (grant-date valuation, K-1 treatment, possible phantom-unit fallback for employees who can't absorb K-1 status).

---

## Part 5 — Inactive founders

The framework's answer, assembled from Parts 3–4 (each element is arithmetic, not accusation):

1. **Year 1:** they receive exactly their banded, evidenced contribution — typically small, never zero if they genuinely worked early months.
2. **Reserve:** unvested tranches forfeit monthly while below the Active Founder Standard; a founder inactive since month 3 retains ~3 tranches (~0.3%) and, absent a return, forfeits the remaining ~4.7% to the pool over time.
3. **Power:** no automatic board seat; unit-weighted voting makes their say proportional to earned stake; the Fundamental-Decision threshold (66⅔%) is set so no individual small holder is a blocking party.
4. **What is never taken:** earned units. *Donahue/Wilkes/Allison* make clawing back earned equity from minority members the highest-risk move available; this design never needs it.
5. **Clean-up actions now:** each inactive founder signs the new OA (ratifying their number), a PIIA/IP assignment, and is offered — not forced — a buyback of earned units at appraised fair value if they prefer cash-out. An ambiguous 20% oral claim is a fundraising killer; a signed, quantified ~0.5–1% stake is a rounding error investors accept.
6. **If any founder refuses to sign:** escalation per Part 8; counsel evaluates the merger/amendment routes (c.156C §60's >50%-of-contributions default) — but with *Allison* front of mind: unanimous consent is the safe harbor, and the negotiation should price that.

---

## Part 6 — The professor

**Design: run him through the identical engine at an evidence-anchored expert rate, cap the outcome, and paper everything.**

1. **No special class, no negotiated lump of equity.** Fixed requirement (2) says identical terms; the engine already values scarce skills higher via fair-market *rates*. His "higher rate than others" expectation is satisfied *objectively*: band X1 at **$400/hr** [$300–$500 bracket], anchored to SEAK's expert-fee survey (median ~$450–500/hr) and ML-consulting ranges ($300–600/hr) — roughly 6x the core engineering rate. His equity is then hours × $400 × 2, like everyone else's formula.
2. **Scale check against benchmarks:** at ~100 documented hours/year he accrues equity that lands, on realistic total-unit denominators, in the **0.5–1.5%** neighborhood by the freeze — squarely between Carta's advisor medians (0.21% pre-seed) and the FAST expert tier (1%), and far below the ~5% part-time academic *co-founder* norm, which supposes ongoing 1-day/week commitment he does not have. If the founders intend him as a true scientific co-founder at ~1 day/week, the same engine prices that too (≈400 hrs/yr → materially more) — the design does not need a different mechanism, only his actual hours.
3. **Advisor Agreement (signed, with integration clause) superseding the oral "decent share" promise** — the research is unambiguous that unwritten promises are enforceable enough to be dangerous (promissory estoppel; quantum meruit; *Zakk v. Diesel* on full performance defeating the statute of frauds). The agreement states: participation in the engine at band X1; 2-year expectation horizon consistent with advisor-market vesting norms; termination provisions; confidentiality; **IP assignment with a Yale carve-out drafted by counsel**.
4. **Yale compliance is his obligation and our diligence item:** stay within Yale's ~1-day/7 external-activity cap; no day-to-day management role (Yale policy discourages it — so he must not be an officer or manager); annual COI disclosure on his side; and — the sharp edge — **IP**: Yale claims inventions made under university auspices, and the consulting carve-out requires Yale Ventures to find the invention unrelated to his Yale research — nearly impossible for ML work in his own field. *Fenn v. Yale* shows Yale litigates this against stars and wins. Counsel must structure his contributions to be advisory (direction, review, introductions) rather than inventive, or negotiate directly with Yale Ventures; any core algorithmic IP he authors is a company-threatening title defect otherwise.
5. **Total-advisor cap:** all advisory (non-employee) allocations combined capped at **[2]%** absent a Fundamental Decision — keeping the cap table within the 2–4%-to-all-advisors-by-Series-A market band (Carta).
6. **Wage/classification flag:** he must be a bona fide independent consultant; the §148B ABC test is a Massachusetts trap even here — counsel item.

**What we do not recommend:** honoring "a decent share" as a negotiated 3–5% grant. Every benchmark says part-time advisory work at this stage is worth well under 2%; over-granting a famous name is a known anti-pattern the market has repriced (Carta advisor medians have *fallen* every year since 2021). His fame is worth a premium *rate*; it is not worth exempting him from the only principle holding this cap table together. If his cooperation genuinely depends on more, the honest instrument is a milestone-based top-up grant (e.g., +0.5% on a named technical milestone he demonstrably drives), bracketed in OA Art. VII for the founders to decide — visibly earned, therefore defensible to every employee out-earning him in the engine.

---

## Part 7 — Governance

### 7.1 Structure (pre-freeze)

- **Members** (all Class A holders — founders and employees identically) elect a **Board of Managers of 3** annually, unit-weighted, [bracketed: cumulative voting to give any ~25% minority bloc a seat]. Any member is eligible; seats are earned by election, not by founder status. [Bracketed alternative: third seat reserved for an outside independent when a qualified candidate exists.]
- The **Board appoints, reviews, and removes the CEO** (removal by 2-of-3 at any time), sets officer role charters, approves budgets, bands, and the annual rate-table re-anchor, and administers the contribution engine's challenge process.
- The **CEO** runs day-to-day operations on Eisenhardt's "consensus with qualification": consult the people closest to the problem, seek quick consensus, and decide when consensus doesn't come. The CEO is a single accountable leader — the configuration the strongest startup-specific evidence supports (§1.3) — made safe by being removable in one board meeting.

### 7.2 Decision taxonomy

| Tier | Examples | Who decides |
|---|---|---|
| Operational | hiring within budget, product, spend within plan | CEO |
| Significant | annual budget, bands/rates, off-plan spend > $[25]K, litigation, for-cause findings, admitting members | Board majority |
| Fundamental | sale/merger/dissolution; amending the equity engine or this taxonomy; new unit classes; issuances outside the engine; debt > $[100]K; the Delaware conversion (pre-authorized in Art. XIII); removing the engine's transparency rules | Members ≥ **66⅔%** of units, **plus** (for amendments reducing any member's earned units) the affected member's consent |

Rationale: no five-way unanimity anywhere (Sah & Stiglitz's conservative-architecture failure; De Dreu & Weingart's conflict costs on complex decisions); no autocracy anywhere (Eisenhardt & Bourgeois; Malmendier & Tate); every level of concentrated power is checked by a faster-moving level above it.

### 7.3 Sunset at financing

At the Freeze Event the elected-board mechanism terminates automatically and the company adopts the investor-standard structure (voting agreement; expected 5-seat 2-2-1 at Series A with an independent tie-breaker — Ewens & Malenko). Founders should internalize now: retaining excess control is *priced against them* (−17–22% per control level, Wasserman 2017), and the design deliberately builds no entrenched control to unwind — itself an investor-attractiveness feature.

---

## Part 8 — Disagreements and deadlock

Escalation ladder (ABA-standard, each rung time-boxed):

1. **Principals meeting** within 10 days of a written dispute notice.
2. **Board resolution** (for member-level disputes not in the Fundamental tier).
3. **Mediation** — half-day minimum with a neutral mediator, within 30 days.
4. **Binding arbitration** (single arbitrator, AAA/JAMS commercial rules, seat: Boston; the same standing **Neutral Arbiter** engagement covers contribution-ledger and banding appeals, so equity disputes get a fast specialized track).
5. **Buy-sell (shotgun) as last resort only**, triggerable only after steps 1–4 fail on a Fundamental-tier deadlock persisting 90+ days: offeror names one price; offeree elects buy or sell at it. Included as a deterrent with eyes open — the evidence says it is rarely triggered and favors the better-financed party (Brooks, Landeo & Spier 2010) — because the alternative backstop, judicial dissolution, is worse.

Anti-deadlock by construction: odd board (3), no unanimity requirements anywhere, supermajority only at the Fundamental tier, and the engine itself de-politicizes the most combustible topic (who deserves what) into ledger arithmetic with an appeal path.

---

## Part 9 — Investor-readiness and the remediation sequence (with counsel)

**Do immediately (order matters):**
1. **Wage Act remediation** — counsel-led, before anything else is signed: begin at least minimum-wage-compliant cash pay (or counsel-validated bona fide member/partner restructuring — whether member status takes workers outside "employee" is a fact-specific call we do **not** make here); quantify the 1-year exposure (10 employees × ≥$15/hr × hours, trebled, personal to managing founders); note deferral agreements are void and private releases of Wage Act claims are likely ineffective. **This liability predates and survives every other choice in this document.**
2. Unanimous signing of the new Operating Agreement + Year-1 ratification + PIIAs/IP assignments from all 15+ people + professor's Advisor Agreement.
3. Retroactive capital-interest grants at supported low FMV; protective 83(b)s within 30 days; profits-interest paperwork for go-forward accrual; securities-law exemption check for issuing to ~16 people (federal + MA blue sky — counsel).
4. Ledger live; first monthly transparency report.

**At financing:** Freeze → Delaware conversion (§351, valuation, QSBS file) → NVCA-standard docs → [12.5]% pool → 409A → standard 4-year/1-cliff grants thereafter.

**Why this package is attractive to investors (the design's answer to fixed requirement 3):** no dead equity (use-it-or-lose-it reserve + activity gates); no oral promises outstanding; every percentage traceable to a ledger a diligence associate can audit; vesting universal (the 92% norm, pre-installed rather than retrofitted at the term sheet); IP assignments complete including the academic-affiliation cleanup; single accountable CEO; no entrenched governance to negotiate away; QSBS preserved for them and the founders; and the one thing VCs require of dynamic-equity companies — a hard freeze into a fixed cap table before their money arrives — is contractual.

---

## Part 10 — Honest limits of the evidence and open risks

1. **No causal evidence** that equal splits harm outcomes or that contribution-based splits improve them; the headline valuation findings are correlational and partly selection (Hellmann & Wasserman say so themselves). The design's reliance is on converging *directional* evidence + incentive theory + this company's specific facts.
2. **Dynamic-equity mechanisms have never been rigorously outcome-evaluated.** Slicing Pie's 2x/4x multipliers are practitioner convention, not measured quantities. We adopt them for legitimacy and simplicity, and bracket them in the OA.
3. **The governance recommendation extrapolates.** Evidence supports a single accountable leader with consultative process and a real board; it does not specifically validate *annually elected* startup boards — that element is our reasoned response to this company's entrenchment problem, stated as such, and it sunsets at financing.
4. **Year-1 banding is a reconstruction**, deliberately coarse; its legitimacy rests on process (blind peer rating, arbiter, ratification), not on measurement precision.
5. **URL verification was constrained** (egress proxy); all-but-one citations are search-index-verified, not fetched; ⚠-marked figures in the references arrived via secondary sources.
6. **Legal risks expressly left to counsel:** Wage Act exposure and remediation strategy; whether founders themselves are Wage Act "employees"; §148B classification of everyone including the professor; *Donahue/Wilkes/Allison* exposure of every step that disadvantages an inactive founder (unanimous consent is the safe harbor); conversion mechanism and §357(c); taxable-grant mechanics of retroactive units; 409A/83(b) execution; securities exemptions; Yale IP negotiation; enforceability of the arbitration and buy-sell provisions under Massachusetts law.
