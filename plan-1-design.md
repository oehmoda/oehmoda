# Plan-1 Design — Governance & Equity Framework for a Five-Founder Massachusetts LLC

*Citations in brackets (e.g., [F1]) map to the annotated bibliography in `plan-1-references.md`, which carries the URL and an honest evidence-strength rating for each source. Where the evidence is thin or disputed, we say so in place.*

**Isolation attestation:** we did not read, check out, diff, or browse any other team's branch or files; we listed remote branch names once, solely to choose an unused plan number.

---

## 0. Reading map and design principles

The founders fixed four requirements: (1) five 5% use-it-or-lose-it set-asides; (2) everything else allocated by an objective contribution system on identical terms for founders and employees; (3) maximum investability; (4) business terms for a lawyer, not statutes. Within those, every design choice below follows five evidence-backed principles:

- **P1 — Process legitimacy beats any particular number.** Perceived justice of the split, not its equality, drives team spirals [F5]; un-negotiated splits are the ones people regret [F1][F4]. So the system is published, mechanical, peer-certified, and auditable.
- **P2 — Assume departures.** ~23% of co-founders are gone by year 3, ~40% by year 8 [C11]; ~50% of founder-CEOs are out of the seat by year 3 [F3][F4]. Everything is earned over time; nothing important requires renegotiating with someone on their way out.
- **P3 — Kill dead equity automatically.** Dead equity is a measured, growing diligence problem [C10] and a folkloric ≥10% red flag [C13]. Forfeitures happen by formula, into the pool that rewards the people still working.
- **P4 — Price the work, not the person or the title.** One rate schedule, applied to the work performed, satisfies "identical terms" while letting market rates carry legitimate differences (a famous ML professor's hour is worth more than a junior engineer's hour because the market says so, not because the rules do) [C1][D11].
- **P5 — Every mechanism must survive due diligence.** Dynamic equity freezes before any institutional money [C3][C4]; the cap table converts cleanly to a Delaware C-corp [B4][B5]; Massachusetts-law landmines (Wage Act, fiduciary duties, noncompete limits) are engineered around, not ignored [E8]–[E16].

---

## 1. URGENT preliminary: the Wage Act problem comes before the equity design

**Ten unpaid employees at a Massachusetts for-profit is an accruing legal emergency, and no equity plan can paper over it.**

- Massachusetts requires employees to be paid weekly/bi-weekly; violations carry **mandatory treble damages** plus attorney's fees, strict liability, no good-faith defense — and late back-pay does not cure exposure once wages were late (*Reuter v. City of Methuen*, 489 Mass. 465 (2022)) [E8][E9].
- Liability is **personal** to the founders who actually manage the company (*Segal v. Genitrix, LLC*, 478 Mass. 551 (2017) — itself an unpaid-startup-executive case) [E10].
- Consent does not help: salary-deferral and "we'll pay you when funded" agreements are **void** "special contracts" (*Stanton v. Lighthouse Financial*, D. Mass. 2009) [E11]. Equity promises do not extinguish wage obligations [E11][E14].
- There is no lawful volunteer status at a for-profit; the Massachusetts trainee exemption is effectively nonprofit-only; the minimum wage is $15.00/hr with its own treble-damages regime [E13]. Relabeling core-work contributors as "contractors" fails prong B of the § 148B ABC test [E12].
- The only recognized compliant paths [E14]: **(a)** pay at least minimum wage on a compliant schedule, or **(b)** make a worker a **bona fide member-partner** — real ownership, real governance rights, distribution risk, K-1 not W-2 — whose relationship is genuinely not employment.

**Design response (business terms; counsel must execute):**
1. Engage Massachusetts employment counsel **immediately** to quantify accrued exposure (~10 workers × hours × ≥$15 × 3, 3-year lookback [E8][E13]) and to structure releases/settlements. We flag, not resolve: whether Wage Act claims can be settled or released at all, and on what terms, is counsel's question.
2. At Formalization (§ 3), every active contributor — founder and employee alike — becomes a **Member** holding units, with governance rights described below. This serves requirement 2 (identical terms) *and* is the only structure under which continued unpaid work is even arguably lawful [E14]. Whether each individual's facts actually support member-partner (non-employee) status is a **counsel flag**, person by person.
3. Begin minimum-wage-compliant payroll (or compliant guaranteed payments to members) as soon as any funding permits; treat this as senior to all other uses of cash. Note the tax coupling: a person holding a profits interest cannot simultaneously be a W-2 employee of the LLC (Rev. Rul. 69-184 line) [A8] — so "member + guaranteed payment" is the LLC-phase pattern, and W-2 status returns after C-corp conversion [B4].

Everything below assumes this remediation is running in parallel.

---

## 2. Entity and tax strategy

**Now: remain a Massachusetts LLC, taxed as a partnership, and issue profits interests.** Profits interests are the only LLC equity instrument that is tax-free at grant (Rev. Proc. 93-27; unvested interests tested at grant under Rev. Proc. 2001-43) [A1][A2]:

- Every unit issued under this plan is a **profits interest** with a **distribution threshold ("hurdle") equal to company FMV at its grant date**, so it has zero liquidation value at grant [A5][A6]. The company maintains a defensible valuation record for each grant tranche (the LLC analog of 409A discipline) [A7].
- Every recipient files a **protective 83(b) election within 30 days** of each grant, even though Rev. Proc. 2001-43 makes it technically unnecessary — it costs nothing and insures against safe-harbor failure [A9]. The 2-year-disposition and treat-as-partner-from-grant conditions are respected [A1][A2]; retroactive-period services can support grants under the broad "for the benefit of" reading of *ES NPA Holding* (T.C. Memo. 2023-55) [A3].
- Consequence, disclosed to every grantee in writing: **you become a K-1 partner; W-2 status, withholding, and some employee benefits end; you owe SE tax and quarterly estimates** [A4][A8]. For the ~10 employees this burden is real; it is also exactly congruent with the Wage Act remediation (§ 1), which needs them to be bona fide members anyway. (Phantom units/UARs would keep W-2 status [A7] but would defeat both the Wage Act structure and the "identical terms" requirement, so we reject them — counsel may revisit per person.)
- Securities compliance: grants ride **Rule 701** (available to LLCs; 12-month cap = greatest of $1M / 15% of assets / 15% of the class; enhanced disclosure above $10M) [A10][E17] plus the Massachusetts compensatory-plan exemption, 950 CMR 14.402(B)(13) [E18]. Any cash raise uses Reg D 506(b) + Form D notice to MA within 15 days / $300 fee [E18].

**At the first qualified financing: convert to a Delaware C-corporation.** This is pre-authorized in the operating agreement (§ 8, reserved matters) so no holdout can block it — the single highest-leverage investability feature we can give the company:

- VC funds avoid pass-throughs (UBTI for tax-exempt LPs, ECI for foreign LPs, K-1 sprawl); the YC SAFE is drafted only for Delaware C-corps; >90% of Carta companies are corporations and ~88% of those are Delaware [B4][B5].
- QSBS is C-corp-only and, for stock issued after July 4, 2025, materially better: **$15M (or 10× basis) per-issuer cap, $75M gross-asset ceiling, 50/75/100% exclusion at 3/4/5 years** [B1]. The QSBS clock starts **at conversion**, and §1202(i) sets basis at conversion-date FMV (pre-conversion appreciation is excluded from the exclusion but enlarges the 10× cap) [B2] — so we convert at the *first* qualified financing rather than "someday," and the operating agreement also lets the Board convert earlier by supermajority if a raise is imminent (converting 30–60+ days before the round, per practitioner consensus [B6]; mechanics: DGCL § 265 statutory conversion + MA filings, ≈$220 DE fee, ~$3k–$7k legal, 30–60 days [B3]).
- On conversion each member's units (set-aside, contribution, advisor) exchange for common stock pro rata to frozen percentages (§ 4.6), unvested tranches carry into reverse-vesting restricted stock on the same schedule [F11], and the Future Pool becomes the option pool.

**Trade-off disclosed:** staying an LLC until the raise costs QSBS-clock time [B6][B2]; converting now costs the pass-through of early losses and forces 409A-style option mechanics prematurely, and the dynamic contribution system (§ 4) is materially cleaner in an LLC than a corporation (continuous re-slicing of a C-corp cap table creates taxable-event risk) [C3]. Because the contribution system must run for at least the retroactive true-up and some forward period, the LLC-now / C-corp-at-financing sequence dominates. If a term sheet appears tomorrow, freeze immediately and convert — the design tolerates that.

---

## 3. The capital structure at Formalization

"Formalization" = the date the amended and restated operating agreement is signed. All percentages are of **pre-financing fully diluted units**; the unit ledger is maintained in cap-table software from day one (spreadsheet cap tables are a diligence credibility problem [C3]).

| Block | Size | Instrument | Governed by |
|---|---|---|---|
| Founder Reserved Pool | **25.0%** (5 × 5.0%) | Profits-interest units, earned quarterly | § 5 |
| Contribution Pool | **62.0%** | Profits-interest units via points formula | § 4 |
| Advisor Grant (Professor) | **1.0%** | Profits-interest units, 24-mo vesting | § 7 |
| Future Pool (new hires & advisors) | **12.0%** | Unissued; Board-controlled | § 6 |

Rationale for the sizes: the 25% is fixed by the founders. 12% matches the measured median seed option pool (12.5% on Carta; seed companies fund at 12–13%) [D5] — an investor-legible number. 1% for the professor is the top of the marquee-advisor band (§ 7). The remainder, 62%, goes to the contribution system — deliberately enormous relative to the ~5% that market-median grants to ten early hires would consume [D1], because in this company employees compete for the same pool as founders and the pool must be able to reward an employee who out-contributes a founder (a fact pattern the founders say has already happened). For calibration: median founding-team ownership is 56.2% post-seed [C12]; here the five founders' *maximum* (25% set-asides + their contribution shares) lands in the same region only if they actually do the work — which is the point.

---

## 4. The Contribution Pool: the identical-terms engine

This is a Slicing-Pie-derived system [C1] with four modifications for enforceability and investability: fixed rate schedule (no per-person negotiation), category guardrails, quarterly certification, and a hard freeze. **No peer-reviewed empirical validation of dynamic equity exists** [C4]; what is peer-reviewed is that static handshake splits correlate with worse outcomes [F1] and that contingent, contribution-sensitive contracting is theoretically the right instrument under skill uncertainty [F7]. We adopt the mechanics and cabin the risk with the Freeze Event.

### 4.1 The formula (spreadsheet-computable)

For each person *p* and calendar quarter *q*:

```
Points(p,q) = Σ over work categories c [ Hours(p,c,q) × Rate(c) × 2 ]
            + CashContributed(p,q) × 4
            + UnreimbursedExpenses(p,q) × 4
            + ApprovedNonCashProperty(p,q) × 2
```

- **×2 / ×4 are the Slicing Pie risk multipliers** for non-cash and cash at-risk contributions [C1]; the general sweat-equity literature uses 1.5×–3× for labor, so 2× is the defensible midpoint [C8]. Only *at-risk* (unpaid/unreimbursed) contributions earn points; any hour or dollar actually paid for earns none [C1]. If the company later pays partial wages, the paid fraction of each hour is excluded: at-risk hour-fraction = max(0, 1 − actual pay rate ÷ Rate(c)).
- **Hours(p,c,q)**: logged per § 4.4, categorized by the work performed, not the person's title.
- **Rate(c)**: the Rate Schedule hourly value of category-*c* work = benchmark annual market salary ÷ 2,000 [C1].
- Points are denominated in dollars ("slice-dollars") but are not debt, wages, or a claim to cash — they are the allocation key for the pool (Wage Act caution: nothing in the plan may promise wages; counsel to review all language [E11]).

**A person's share of the Contribution Pool at any date = their cumulative Points ÷ all cumulative Points, × 62%.** Until the Freeze Event, percentages float exactly as in Slicing Pie [C1].

### 4.2 The Rate Schedule (Exhibit B of the operating agreement)

One schedule for everyone — founder, employee, or advisor. Rates are set from public market-compensation benchmarks for Greater Boston (Carta compensation data and Pave market data are the named benchmark sources [D6][D7]), adopted at Formalization and re-benchmarked each January by the Contribution Committee (§ 4.5) with Board approval; changes apply prospectively only.

Illustrative opening schedule (final numbers to be pulled from the named benchmarks at signing — bracketed for counsel/committee):

| Category of work | Benchmark role | Annual benchmark | Rate/hr (÷2,000) | Slice rate (×2) |
|---|---|---|---|---|
| Software engineering — junior (L1–L2) | SWE I–II, Boston | [$120,000] | $60 | $120 |
| Software engineering — senior (L3–L4) | Senior SWE, Boston | [$180,000] | $90 | $180 |
| Software engineering — staff+ (L5+) | Staff/Principal SWE | [$220,000] | $110 | $220 |
| Engineering management | EM (5–15 reports) | [$210,000] | $105 | $210 |
| Product / technical vision & strategy | Head of Product / CTO-strategy | [$200,000] | $100 | $200 |
| Business planning, fundraising, sales, ops | Head of BizOps / VP-level | [$190,000] | $95 | $190 |
| Specialist ML consulting (external-expert tier) | Senior ML consultant day-rate | [$500/hr equiv.] | $250 | $500 |

Notes on the contested choices, stated honestly:

- **Coding vs. management vs. vision.** All three are priced at market salary for the role *doing that work* — vision/strategy work is a well-paid category (~Head-of-Product/CTO rates), not a super-category. This deliberately implements Slicing Pie's zero-idea-premium doctrine [C1] and *rejects* both Demmler's idea-weight-7/10 [C5] and the observed 10–15 pp idea premium in Wasserman's data [C15]. Reason: the founders' requirement is an "objective" system; an idea premium is exactly the unmeasurable, self-servingly inflatable input that torpedoes perceived justice [F5]. The idea already gets paid through the 5% set-asides, which only founders have.
- **Leveling.** Each person's level per category is proposed by the CEO, reviewed by the Contribution Committee, and set by the Board annually; a person can hold different levels in different categories (a staff-level coder may be junior-level at management). Disputes go down the § 9 ladder.
- **The specialist tier** exists so the professor's hours are priced at his market ($2,500–$5,000/day ≈ $312–$625/hr is the documented professor-advisor norm [D11]) under the same rules as everyone. Any member may qualify for it for specific work if the Committee finds an arm's-length market for that person's services at that rate (evidence: actual paid consulting engagements).

### 4.3 Category guardrails (anti-gaming)

The known failure mode of hour-priced systems is unfalsifiable "strategy" hours [C3]. Guardrails, all mechanical:

1. **Strategy/vision cap:** ≤15% of a person's logged hours per quarter may be in the vision/strategy category, unless tied to a Board-pre-approved deliverable (a written spec, a fundraising process, a filed patent application).
2. **Management floor:** management hours require named reports or named coordination deliverables in the log.
3. **Evidence norm:** engineering hours should reconcile loosely with repository activity; all categories admit calendars, documents, and shipped artifacts as evidence. Logs are evidence-backed claims, not honor-system diaries.
4. **Late-log forfeit:** hours not logged within 60 days of quarter-end are forfeited (prevents retroactive log-stuffing; the one-time § 4.7 retroactive process is the sole exception).
5. **Cash cap:** cash contributions above $[25,000]/person/quarter require Board pre-approval to earn the 4× multiplier (prevents wealth from buying the pool; investors price money at 1× in real rounds — the 4× is for genuine early risk capital [C1], not a side-door financing).

### 4.4 Ongoing tracking and certification cycle

- **Weekly:** hours logged in the tracking system (any auditable tool; entries carry category, description, evidence link).
- **Monthly:** each person certifies their own log; the CEO (or, for the CEO's log, the Independent Manager) countersigns.
- **Quarterly:** the Contribution Committee publishes to all members a statement per person: hours by category, points, cumulative points, resulting pool share. Members have 30 days to object (→ § 9 ladder; unobjected statements become final). Transparency is the point: perceived justice tracks visible process [F5].
- **Quarterly issuance:** finalized points convert into Contribution Units (profits interests, hurdle = current FMV [A5]) so that the unit ledger always reflects the current split. Each issuance batch carries its own protective 83(b) round [A9].

### 4.5 The Contribution Committee

Three members: the Independent Manager (chair) and two members elected annually by unit vote, at most one of whom may be a founder. It administers logs, publishes statements, proposes rate re-benchmarks, and rules first-instance on categorization disputes. It cannot change the formula, multipliers, or anyone's past points — those are reserved matters (§ 8).

### 4.6 The Freeze Event

The pool stops floating at the **earliest** of:
1. a qualified financing (≥ $[1,000,000] in one transaction or series),
2. C-corp conversion (§ 2),
3. 36 months after Formalization, or
4. Board supermajority (4 of 5) plus 66⅔% of units electing to freeze.

At freeze: percentages fix at cumulative-points shares; unallocated pool units (if any points-capacity is unused) roll into the Future Pool; all *future* compensation moves to conventional fixed grants from the Future Pool on standard 4-year/1-year-cliff schedules [F10][F11]. This is precisely the "write the freeze into the operating agreement in advance" discipline that both Slicing Pie's author and its critics agree on [C1][C3][C4].

### 4.7 The retroactive year (one-time true-up)

The past unpaid year is scored with the **same formula** — no special founder treatment (requirement 2):

1. Each person files a **Retroactive Contribution Statement** within 45 days of Formalization: quarter-by-quarter hours by category, cash, expenses, with evidence (git history, PR reviews, release tags, calendars, documents, invoices, bank records). Sworn accuracy; knowing inflation is a Cause event (§ 5.4).
2. Statements are published to all members; each statement needs counter-certification by two other members who worked closely with the person; 30-day objection window.
3. The Contribution Committee (bootstrapped for this purpose: the Independent Manager plus two members elected before statements are filed) resolves objections; unresolved objections go to § 9 final-offer arbitration (each side submits a number; the arbitrator picks one [G16]).
4. Retroactive points then enter everyone's cumulative totals; the same 2×/4× multipliers apply (uniform — we considered a higher "earliest risk" multiplier and rejected it as an unfalsifiable knob; 2× already prices the risk [C1][C8]).
5. Memorialization only, no renegotiation: the informal agreement the founders already made ("reserved allocation + contribution-based remainder") is treated as the pre-existing deal being *documented*, per the process-legitimacy evidence [F1][F5]. **Counsel flags:** tax character of units issued for past services (compensation-at-FMV risk for anything that is not a clean profits interest [C8][A3]); Wage Act interaction for the ten employees (§ 1) — the retroactive scoring must not be drafted as "payment for past labor."

### 4.8 Worked example (illustrative numbers)

Year-1 reconstruction for four people (quarterly detail collapsed; rates from § 4.2):

| Person | Work | Hours | Slice rate | Cash | Points |
|---|---|---|---|---|---|
| Founder A | senior SWE 1,800h + strategy 200h (capped OK) | 2,000 | $180 / $200 | $10,000 ×4 | 1,800×180 + 200×200 + 40,000 = **$404,000** |
| Founder B | staff SWE 900h + EM 900h | 1,800 | $220 / $210 | — | 198,000 + 189,000 = **$387,000** |
| Founder C (drifting) | senior SWE 300h | 300 | $180 | — | **$54,000** |
| Employee E1 | senior SWE 1,900h | 1,900 | $180 | — | **$342,000** |

E1 (an employee) out-points Founder C by 6.3× — the system does what the founders asked: employees and founders on identical terms, and the inactive founder's contribution share reflects reality without anyone having to fight about it. If total Year-1 points across all 15 people were $2.6M, Founder A's share of the pool is 404,000/2,600,000 × 62% ≈ **9.6%**, E1's ≈ 8.2%, Founder C's ≈ 1.3% — before anyone's 5% set-aside earnings (§ 5).

---

## 5. The five 5% set-asides: earn-out mechanics

The set-asides are the founders' "premium for having founded" — bounded at 5% each by their own fixed requirement, and earned, never guaranteed.

### 5.1 Schedule

Each founder's 5.0% divides into **16 equal quarterly tranches of 0.3125%**, over 4 years measured from the company's founding date (not Formalization) — the standard 4-year founder horizon [F10][F11], with the elapsed first year handled retroactively (§ 5.3). There is no cliff: the first year already served functions as the cliff period, mirroring the customary practice of backdating vesting commencement for demonstrable pre-formalization work [C9].

### 5.2 Earning conditions (use-it-or-lose-it)

A founder **earns a tranche** for quarter *q* if and only if both:

1. **Active Service:** ≥ **250 qualified contribution hours** logged and certified for *q* under § 4.4 (≈ half-time; the threshold is deliberately objective and shared with the § 6.2 inactivity definition), and
2. **Performance:** the Board (founder recused) determines the founder met at least "meets expectations" on the majority of their pre-agreed quarterly objectives (§ 6.1). If the Board sets no objectives for a founder in time, condition 2 is deemed met — the burden of goal-setting is on the Board, not the founder.

A tranche not earned is **permanently forfeited into the Contribution Pool** — no make-up, no carry-forward. Forfeiture into the pool (rather than into a dead reserve) means inactive-founder equity automatically becomes active-contributor equity, the anti-dead-equity design the diligence literature demands [C10][C13].

### 5.3 The retroactive four quarters

Year-1 tranches are earned by the same test applied to the § 4.7 retroactive statements — Active Service is testable from the evidence; the performance condition is deemed met for the retroactive period (no objectives existed). In the § 4.8 illustration, Founders A and B earn all four tranches (1.25% each), Founder C earns at most one (the quarter with ≥250 hours, if any), and roughly 3.75%+ of Founder C's set-aside has already rolled into the pool that pays the people who did the work.

### 5.4 Departure and leaver terms (uniform for everyone, per Donahue equal treatment [E4])

| Event | Set-aside tranches | Contribution/advisor units |
|---|---|---|
| **Good leaver** (death, disability, termination without Cause, resignation for Good Reason) | future tranches lapse to pool; earned tranches retained | retained in full (Slicing Pie good-leaver rule [C2]) |
| **Bad leaver** (termination for Cause; resignation without Good Reason before Freeze+12 months) | future tranches lapse; earned tranches: company repurchase option at the **lower** of FMV and $[nominal] | non-cash-derived units: company repurchase option at $[nominal]; cash-derived units: repurchase at 1× cash contributed (multiplier stripped) [C2][C14] |

"Cause" and "Good Reason" get tight definitions in the operating agreement (Cause includes fraud, conviction, material uncured breach, knowing log inflation; Good Reason includes material role/economics reduction without consent). Repurchase mechanics must be uniform and exercised uniformly — selective repurchase from insiders is a Donahue equal-opportunity violation [E4]. **Counsel flags:** enforceability of nominal-price repurchase against the Donahue/utmost-good-faith backdrop [E4][E6]; interaction with the non-waivable § 36 resignation right (we regulate the economics of exit, which the statute permits, not the right to exit [E2]); *Miele* confirms forfeiture-for-breach-of-nonsolicit conditions live outside the noncompete act [E16].

### 5.5 Financing interactions

Unearned tranches simply continue on schedule through a financing; the operating agreement pre-authorizes the Board to accept investor-standard re-vesting or double-trigger acceleration terms at a qualified financing without member renegotiation [F11]. We do not grant single-trigger acceleration (investor-disfavored [F11]).

---

## 6. Founder roles, performance, and inactive founders

### 6.1 Roles and measurement

- Every founder who wants Active status holds a **role charter** (title, scope, reports, deliverables) approved by the Board annually. Titles follow function, and the "founder" honorific carries no governance rights by itself — board seats and offices follow election and appointment (§ 8), not history. (This is what lets the company truthfully tell investors there are no legacy-title landmines.)
- **Quarterly objectives** (OKR-style) are set per founder-officer by the CEO and Board; the CEO's own objectives are set by the non-CEO managers. The annual cycle includes a Blumberg-style CEO review: self-assessment + 360 from team and Board + objective scoring, with quarterly check-ins [G13]. These reviews drive § 5.2's performance condition and officer continuation — not equity beyond the tranche test (equity flows through the formula; reviews gate the set-asides only, keeping the "objective system" promise).

### 6.2 Inactive founders (the current live problem)

**Definition (mechanical):** a founder is **Inactive** after two consecutive quarters below 250 qualified hours (same threshold as § 5.2), and returns to Active after one quarter at or above it (prospectively only — missed tranches stay forfeited).

Consequences, all automatic:

| Dimension | Treatment |
|---|---|
| Set-aside | tranches stop accruing (already § 5.2); forfeited tranches feed the pool |
| Contribution share | keeps every point earned; earns ~nothing new (the formula does this by itself) |
| Officer roles | Board may remove from any office; given *Pointer v. Castellani*, removal must be documented with a legitimate business purpose and consideration of less-harmful alternatives — the objective hour/performance record **is** that documentation [E5] |
| Board seat | none by right; an Inactive founder may stand for election like anyone, but the member-elected seats are annual (§ 8), so an inactive founder's seat naturally comes up for a vote within a year |
| Voting | earned/issued units keep full votes — we do not strip vested economic rights (dead-vote stripping invites a Donahue-line challenge and destroys the credibility of "earned means owned" [E4][E6]) |
| Information | observer rights at Board meetings continue while a ≥[2]% holder [G14] |
| Covenants | NDA, IP assignment, and 12-month nonsolicit survive; **no noncompete** (mostly unenforceable here and unnecessary — see § 10 flags [E15][E16]) |

An Inactive founder who never returns simply converges to: earned set-aside tranches + earned points, both frozen — which after a mostly-inactive Year 1 is a low-single-digit percentage. That is the honest answer to "what does a founder who stopped working deserve": what they earned, computed by the same ledger as everyone else, with no negotiation and no lawsuit. Expected dead weight stays far under the ~10% diligence red line [C13].

### 6.3 Expulsion

Because c. 156C has **no statutory expulsion** [E2], the operating agreement creates one: a member may be expelled (units treated per the § 5.4 bad-leaver column) only for Cause, by Board determination **plus** 66⅔% of units excluding the affected member. Expulsion is deliberately hard — the system is built so that inactivity self-resolves economically without expulsion, which is the fiduciary-safe path in Massachusetts [E4][E5][E6].

---

## 7. The professor

**The promise:** an informal "decent share," with an expectation of "a higher rate than others," part-time. **The constraint set:** requirement 2 (identical terms in the contribution system), Yale's one-day-in-seven consulting cap [D14], Yale's ownership of inventions within his research scope [D15], COI disclosure/approval obligations [D13], and market norms that top out around 1% for marquee advisors (FAST Expert tier at startup stage: 0.80% [D8]; measured medians are far lower — 0.21% pre-seed, 0.12% seed [D9]; ~1% reserved for "highly desired candidates with strong track records" [D10]; professor-SAB norm 0.1–0.3% + day rates, more for stars [D11]).

**The package:**

1. **Advisor Grant: 1.0%** in profits-interest units, vesting monthly over 24 months, no cliff, single-trigger acceleration on change of control (the advisor-market norm, unlike employee grants [D9]) — conditioned on a signed advisor agreement with the IP/COI terms below and ≥[8] hours/month average engagement. 1.0% honors "a decent share" at the very top of the defensible market band, and materially above measured medians — a generous, citable answer the company can show investors without embarrassment [D8][D9][D10][D11].
2. **Higher rate, identical rules:** for hours beyond the advisor baseline he may earn Contribution Points like everyone else, priced at the **specialist ML consulting tier** of the Rate Schedule ($[500]/hr slice rate), which is simply his documented market rate [D11]. His seniority is expressed through the market price of his time — not through special mechanics. If he asks for a superior *class* of terms, the honest answer is that requirement 2 forbids it, and this package pays him more per hour than anyone in the company anyway.
3. **Advisor agreement terms** (Cooley-pattern for university-affiliated advisors [D18]):
   - IP assignment **narrowly scoped** to work performed for the company, outside Yale duties and without Yale resources; anything within his Yale research scope is Yale's and reaches the company only by a Yale license [D15][D18].
   - Publication: company pre-review limited to [30] days for confidential-information excision, patent-delay extension ≤[90] days (≤180 total), never a veto [D21].
   - COI: written confirmation that he has made Yale's required disclosures and obtained any needed approvals (Provost approval is required for board seats, especially where his IP is involved — so **no board seat** for the professor) [D13]; total commitment sized inside the one-day-in-seven cap [D14].
   - **No Yale students** work for the company absent written, university-cleared agreements (Northwestern-style student-agreement discipline as best practice) [D17].
   - No noncompete (unenforceable/toxic here); NDA + nonsolicit only [E15][E16].
4. **What we do not do:** no "advisory board seat with voting rights," no revenue share, no uncapped promise. The informal "decent share" conversation is memorialized and superseded in the signed agreement (integration clause) — open-ended oral promises to well-known people are diligence poison.

---

## 8. Governance: board, officers, voting, reserved matters

### 8.1 Structure

**Manager-managed LLC** (management vests in a Board of Managers; members qua members do not manage) [E2] — the corporate-style structure investors can read, and the one that cleanly maps onto the post-conversion board.

**Board of Managers: 5 seats.**
- **Seat 1: the CEO**, ex officio.
- **Seats 2–4: member-elected managers**, elected annually by plurality of all voting units (founders and employees vote the same units the same way — there are no founder-class seats).
- **Seat 5: Independent Manager** — an outside person with no units before appointment, nominated by the Board and confirmed by majority of units; compensated from the Future Pool at the market rate for independents (~0.78% at seed / 0.53% at Series A on Carta [G12]); chairs the Contribution Committee and casts tie-breaking votes.

Rationale: the market norm is a 3-seat seed board and a 5-seat 2–2–1 at Series A [G12]; a 5-founder company cannot seat all founders (five founder-directors is outside all observed norms [G12][G13]), and seats tied to election rather than founder status is what makes the inactive-founder problem self-resolving (§ 6.2). Founders not on the Board hold observer rights (attend + information, no vote) while ≥[2]% holders, keeping information symmetric at zero control cost [G14]. Retaining founder control of the board is itself associated with 17–22% lower valuations per control level [F2] — the independent seat and annual elections are the counter-signal. At a financing, the Board is pre-authorized to renegotiate to the NVCA-standard structure (e.g., 2 common / 2 investor / 1 independent) [G11].

### 8.2 Officers and the CEO decision

**One CEO.** The peer-reviewed co-CEO evidence says shared command is the configuration that fails (performance rises with the power gap between co-leaders) [G3]; the pro-co-CEO HBR data is survivor-biased and its own success factors concede the point [G4]. With five equal-ish founders the temptation is a committee; the evidence-backed rule is Eisenhardt's **consensus with qualification**: the executive team seeks consensus, and when consensus fails the CEO decides with input [G5] — while avoiding dominant-CEO autocracy, which underperforms in turbulent environments [G7]. Concretely:

- **Selection:** the Board elects the CEO by majority (candidate recused). For the first selection, any founder may stand; the Board interviews all candidates against a written role spec and votes. (No rotation, no co-CEOs, no "CEO in name only" — titles must match decision rights [G3][G5].)
- **Accountability:** annual structured review (self-assessment + 360 + objectives, § 6.1) [G13]; the CEO manages board relationships bilaterally as the venture-CEO literature advises [G2].
- **Removal:** majority of the four non-CEO managers, at any time, with or without cause (succession is a base-rate event — ~50% by year 3 — and pre-agreed removal machinery beats a mid-crisis improvisation [F3][F4]). Removal from CEO is not expulsion as a member and does not touch earned equity (§ 5.4 governs only actual departures).
- Other officers (CTO, VP Eng, etc.) are appointed and removed by the Board on CEO recommendation.

### 8.3 Voting and classes

One class of voting units; **one unit, one vote**, whether held by founder, employee, or advisor (identical terms, requirement 2). Unissued points don't vote; issued units do. [Counsel flag: whether the advisor grant should be non-voting for securities/COI cleanliness — we default to voting for uniformity, but flag Yale COI optics [D13].]

### 8.4 Reserved matters

Requiring **Board majority + 66⅔% of voting units**: amending the operating agreement; issuing units outside the § 3 pools; admitting members outside the plan; sale/merger/dissolution; debt > $[100,000]; related-party transactions > $[25,000]; changing the Rate Schedule *retroactively* or changing multipliers/formula at all; expulsion (§ 6.3); electing to freeze early (§ 4.6.4).

Requiring **Board supermajority (4/5) only**: annual Rate Schedule re-benchmark (prospective); budget; opening the Future Pool beyond [3]%/year.

**Pre-authorized (no further consent):** C-corp conversion and associated filings at a qualified financing, with every member obligated to execute conversion documents (drag-along-style covenant) — the NVCA-legible feature that removes the classic LLC-holdout risk at term-sheet time [G11][B4].

This list deliberately mirrors NVCA protective-provision vocabulary so future investors see familiar machinery [G11].

---

## 9. Dispute and deadlock resolution

Layered ladder (ABA deadlock-mechanism canon [G15]), cheapest first:

1. **Operational disagreements:** consensus with qualification — CEO decides after hearing the team [G5].
2. **Board ties:** the Independent Manager's casting vote [G15].
3. **Quantifiable disputes** (points, categorization, rates, leveling, valuation, buyback price): Contribution Committee first instance → **final-offer ("baseball") arbitration** — each side submits one number, a single arbitrator with industry expertise must pick one, loser pays. FOA's moderation incentive is theoretically strong and drives high pre-hearing settlement in practice, though empirical convergence findings are mixed [G16]. FOA is ideal here precisely because these disputes are numeric.
4. **Member-level deadlock on reserved matters** persisting 60 days: mandatory mediation (JAMS/AAA, 30 days) → binding arbitration [G15].
5. **Irreconcilable member deadlock** (arbitration cannot resolve a governance impasse): a deadlock **put/call** — the Board may cause the company to buy out the dissenting minority at FMV set by § 9.3-style appraisal-FOA. **No shotgun/Russian-roulette clause**: shotguns are fair only between symmetrically informed, symmetrically *funded* parties, and lab evidence shows the cash-poor side gets exploited [G10] — these founders are unpaid; a shotgun would hand the wealthiest founder a weapon.
6. Everything above exists to keep everyone out of § 44 judicial dissolution ("not reasonably practicable"), the value-destroying end state [E3][G15].

Fiduciary backdrop: Massachusetts imposes Donahue-line "utmost good faith and loyalty" among close-LLC members and it cannot simply be waived [E1][E4][E6][E7]. The agreement therefore **specifically** authorizes defined self-interested acts (serving on the Contribution Committee while holding units; voting one's units on reserved matters; outside activities that are not company-opportunity usurpation) rather than attempting a Delaware-style blanket elimination that Massachusetts probably doesn't allow [E1][E7].

---

## 10. Consolidated counsel flags (we decide business terms; these are the legal risks we are handing over, not resolving)

1. **Wage Act remediation** (§ 1): quantify exposure; person-by-person analysis of member-partner status for the ten employees; whether/how accrued claims can be settled or released; guaranteed-payment design; the § 4 plan's language must never promise wages [E8]–[E14].
2. **Partner/W-2 dual status**: mechanics of moving grantees off W-2; benefits transition; whether any employee should get phantom units instead (with the requirement-2 tension noted) [A4][A8].
3. **83(b)/valuation**: protective elections for every tranche; defensible FMV/hurdle support at each quarterly issuance; tax character of the one-time retroactive issuance [A5][A9][C8].
4. **Securities**: Rule 701 plan documentation and caps; 950 CMR 14.402(B)(13) fit for member-partners who are arguably not "employees/consultants"; Form D discipline for any cash [A10][E17][E18].
5. **Fiduciary-duty drafting**: specificity of duty-restriction clauses (blanket elimination unavailable in MA); Donahue-safe uniform repurchase mechanics; expulsion and freeze-out exposure (*Pointer*, *Allison*) [E1][E4]–[E7].
6. **§ 36 resignation interaction**: confirm the leaver-economics survive the non-waivable 6-month-notice resignation right [E2].
7. **Restrictive covenants**: nonsolicit/NDA/forfeiture architecture per *Miele*; no noncompetes for non-exempt (unpaid) workers; whether member-noncompetes in the operating agreement fall under the sale-of-business exclusion (unsettled — we did not rely on it) [E15][E16].
8. **Professor**: advisor agreement vs. Yale policy rider; verify his COI disclosure/approvals actually exist; Yale license needed for any of his in-scope IP; publication clause; no students without cleared agreements [D13]–[D18][D21].
9. **Conversion**: DGCL § 265 conversion vs. merger method; QSBS timing/basis at conversion; profits-interest → stock exchange mechanics; EIN/contract continuity [B2][B3].
10. **Newest authorities**: confirm reporter cites (e.g., *Miele*, 2025) and the post-OBBBA QSBS parameters before relying on them [E16][B1].

---

## 11. Why this design wins on the founders' own criteria

- **Requirement 1** — the set-asides are real but earned: quarterly tranches, objective hour + performance gates, automatic forfeiture into the pool. A fully active founder gets the full 5%; the already-inactive ones have already returned most of theirs to the people doing the work — with no confrontation, because the ledger does it.
- **Requirement 2** — one formula, one rate schedule, one certification process, one dispute ladder for founders and employees alike; the worked example (§ 4.8) shows an employee out-earning a founder 6:1, which is the requirement operating as intended.
- **Requirement 3** — profits interests with clean 83(b)s now; a pre-authorized Delaware flip with drag-along at the first real round; a frozen, software-maintained cap table; a 12% pool at the measured market median; no dead-equity overhang; NVCA-shaped reserved matters; an independent tie-breaker; no shotgun timebombs; and the Wage Act problem being remediated instead of discovered in diligence.
- **Requirement 4** — every mechanism above is a business term with bracketed parameters; `plan-1-operating-agreement.md` hands counsel the article-by-article skeleton.
