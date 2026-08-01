# Plan 5 — Governance & Equity Framework: Full Design and Rationale

**Prepared by plan5 for the five founders of [Company], a Massachusetts LLC (~1 year old, 5 founders, ~10 employees, all unpaid).**

Companion documents: `plan-5-one-pager.md` (summary), `plan-5-operating-agreement.md`
(article-by-article business-terms draft), `plan-5-references.md` (annotated bibliography
with evidence-strength ratings). Citations below use [R-n] keys resolved in the
references file; every source URL there was verified live this session (see the
verification-method note at the top of that file).

---

## 1. What we were asked to do, and the one thing we must say first

We were asked to design governance and equity within four fixed requirements: (1) each
founder's reserved allocation capped at 5%, earn-only; (2) all remaining equity through an
objective contribution-based system on identical terms for founders and employees;
(3) maximum attractiveness to future investors; (4) business terms for counsel, not
statutory drafting.

**Before any of that: the company's ~10 unpaid employees are a live legal emergency, not a
design parameter.** Under U.S. Department of Labor policy, private for-profit companies
cannot lawfully use volunteers at all [R-40], equity cannot substitute for minimum wage
[R-41], and the Massachusetts Wage Act awards **mandatory treble damages plus attorney's
fees** for unpaid wages [R-36], with **personal civil and criminal liability** for the
individuals who manage the LLC (*Cook v. Patient Edu, LLC*, 465 Mass. 548 (2013)) [R-38],
and no cure by paying late (*Reuter v. City of Methuen*, 489 Mass. 465 (2022)) [R-37].
Relabeling the ten as contractors fails prong B of the Massachusetts ABC test
(c. 149 § 148B) because they do the company's core work [R-42]. At $15/hour Massachusetts
minimum wage [R-41], ten people × a year of work implies a floor exposure in the high six
figures *before* trebling — borne personally by whichever founders run the company. Every
equity mechanism below is designed so it can also *mitigate* this (by making contributors
genuine members, see §9.1), but only employment counsel can defuse it. **Nothing else in
this document matters as much.**

---

## 2. Diagnosis: what kind of problem this company actually has

Five facts drive the design:

1. **The founders already tried the default and it failed.** They began as equal partners;
   contributions then diverged; some founders went inactive while some employees
   out-contributed founders. This is the textbook trajectory: 73% of founding teams split
   equity within a month of founding, mostly with no adjustment mechanism [R-3], about
   one-third to one-quarter of teams split equally [R-1][R-8], and equal splits agreed
   quickly are associated with lower first-round valuations [R-1]. More than 23% of
   cofounders are gone by year three [R-8]. This team is living the base rates.

2. **Nothing is written down.** The informal reserved-allocation agreement and the
   professor's "decent share" are oral promises layered over a default statutory LLC.
   Perceived justice of the split — not its arithmetic — is what sends founding teams into
   positive or negative interaction spirals [R-4], and unexplained reward inequality
   measurably destroys effort (output −0.24 to −0.45 SD in the best field experiment),
   while inequality with *observable* justification does not [R-14]. A transparent,
   evidence-based settlement process is therefore not bureaucracy; it is the intervention.

3. **The team is engineers whose work spans code, management, and vision.** Any
   contribution metric that scores "vision" subjectively will be gamed or fought over;
   any metric that counts only commits will be Goodharted. The design prices the *role*
   (at benchmarked market rates) rather than judging the brilliance (§5.3).

4. **Investors will judge the cap table.** Venture infrastructure presumes a Delaware
   C-corporation (NVCA model documents [R-27]; ~88% of C-corp startups on Carta are
   Delaware [R-26]; VC funds avoid LLC pass-throughs because of their tax-exempt LPs'
   UBTI [R-25]). Departed founders holding large stakes are a named deal-killer
   (a departed cofounder at 25–40% kills deals; investors expect ex-advisor stakes of
   0.1–1% [R-33]), and investors "are very likely" to require founder vesting, wanting
   founders no more than ~40% vested at Series A [R-32].

5. **The fixed requirements already choose a side in a real academic dispute.** Y
   Combinator's advice is the opposite of contribution-metering: split near-equally
   because "99% of the work is left to be done" [R-24]. The founders' requirement 2
   forecloses that path — but we flag honestly (§10) that the pro-metering evidence is
   correlational and the strongest practitioner voice in startups disagrees with metering
   as a philosophy. Our design threads this: a *dynamic* system for the messy bootstrap
   phase, converting deliberately to the conventional fixed-cap-table-plus-vesting stack
   that YC-style companies use, at the first financing (§5.4, §8).

---

## 3. Design overview

```
                       ┌──────────────────────────────────────────┐
                       │  100% of pre-financing equity            │
                       ├──────────────────────────┬───────────────┤
                       │  Contribution Pool ≥75%  │ RFA ≤25%      │
                       │  (identical terms:       │ (5%/founder,  │
                       │  founders, employees,    │  earn-only,   │
                       │  professor)              │  1/36·month)  │
                       └──────────────────────────┴───────────────┘
  Measurement:  Slices = hours × benchmarked role rate × 2  (cash × 4)
  Issuance:     Contribution Units quarterly, 1 Unit per Slice; % = your Units / all Units
  Retroactive:  Year-1 reconstructed once, evidence-weighted, same formula
  Governance:   3-manager elected board → accountable CEO → domain leads
                ("consult, then decide"; no vetoes; supermajorities for big moves)
  Exit ramp:    Freeze Event (financing / conversion / 36 months) → fixed cap table,
                Delaware C-corp, standard option pool + vesting
```

---

## 4. Governance: what the evidence supports

### 4.1 The question we were told to investigate honestly

Should a 15-person startup have a single leader, shared leadership, rotating leadership,
or consensus? We looked for evidence on each. Summary of what exists:

| Option | Best evidence | What it says | Strength |
|---|---|---|---|
| Shared leadership | 3 meta-analyses [R-15][R-16][R-17] | Positive team-level effects (ρ ≈ .18–.35), strongest for complex, interdependent work; adds variance **over and above** vertical leadership | Peer-reviewed meta-analytic, but samples are teams *inside* organizations, not whole companies |
| Fully flat / self-managing | Lee & Edmondson review [R-18]; Zappos record [R-20] | Empirical base "limited — only a few empirical studies"; flagship whole-company experiment lost 14–18% of staff to buyouts and was rolled back | Review + case; thin |
| Consensus / equal power | Deadlock literature [R-23]; co-CEO study [R-22] | 50/50 power without tiebreakers is a documented catastrophic failure mode; even among co-CEOs, a clear power *gap* improves performance (inverted-U) | Peer-reviewed (law & econ theory + experiment; archival) |
| Co-CEOs | HBR 2022 analysis [R-21] | 87 public firms, co-CEO tenures returned 9.5% vs 6.9% — but tiny, selection-biased, practitioner-grade | Weak-moderate |
| Rotating CEO | — | **No empirical literature found.** (The Huawei anecdote circulates uncited; we do not rely on it.) | None |
| Single accountable leader + heavy input | Eisenhardt [R-19]; Aghion-Tirole [R-24b]; psychological safety [R-19b] | Fast, high-performing deciders in high-velocity markets use *more* real-time information and *more* alternatives, then resolve via **"consensus with qualification"**: everyone gets voice; if consensus doesn't come quickly, the responsible executive decides | Peer-reviewed (8-firm inductive; formal theory; field study) |

### 4.2 The design that follows

**A single accountable CEO, appointed and removable by an elected three-person board, with
formally delegated domain leads and a mandatory consult-then-decide protocol.** This is
not the conventional answer adopted by reflex; it is the configuration at the
intersection of the evidence:

- *Why one accountable executive:* the deadlock and co-leadership literature penalizes
  equal power at the top [R-22][R-23]; Eisenhardt's fast-decider pattern requires a
  decision-maker of last resort [R-19]. With five founders of diverging commitment, any
  power-sharing scheme among "the founders" as a class would hand influence to inactive
  people — exactly what requirement 1 and 2 are trying to end.
- *Why the CEO is hired help, not a throne:* founder control (board control and/or the CEO
  seat) is associated with 17–22% lower pre-money valuations per control dimension
  retained [R-13]; half of founders are no longer CEO by year three, usually after
  success, not failure [R-2][R-12]; and causal evidence (IV design) shows founder
  *replacement* improves startup performance [R-7]. So: annual board appointment, removal
  at will, no founder birthright. This is also the strongest investor signal available —
  a team that has pre-built professional governance.
- *Why real domain leads (this is where the shared-leadership evidence lands):* the
  meta-analytic benefit of shared leadership is real but is a **complement to vertical
  leadership, in interdependent work** [R-16]. We implement it as formally delegated,
  published decision authority per domain (Aghion-Tirole's real-authority delegation
  [R-24b]) rather than as diffuse collective decision-making.
- *Why consult-then-decide is mandatory, not cultural:* Eisenhardt's "consensus with
  qualification" [R-19] plus psychological-safety evidence that voice drives learning
  [R-19b]. The operating agreement makes consultation a *duty* whose breach is reviewable,
  while making clear that consensus failure never blocks a decision.
- *Why a 3-person elected board:* practitioner convergence for seed-stage boards is three
  members, odd-numbered to avoid deadlock [R-30]; venture-board scholarship is young but
  confirms boards are the apex venue for the decisions that matter [R-28][R-29]. Annual
  election by all unit-holders (with cumulative voting bracketed to protect minorities)
  replaces founder entitlement with accountability, and gives the ~10 employees — who now
  hold real equity — a genuine franchise.
- *Decision stack:* operational → CEO (after consultation); significant/reserved → Board
  majority; fundamental → 66⅔% of units; the equity engine itself → 75% (entrenched).
  No individual has a veto anywhere. Disputes escalate CEO → mediation → binding
  arbitration, with the buy-sell machinery deliberately absent because a many-holder unit
  structure cannot produce a 50/50 deadlock [R-23].

**Evidence honesty:** the strongest claims here rest on correlational or small-sample
work. Eisenhardt is 8 firms; Wasserman's control discount is association, not causation
(control-hungry founders differ systematically); the shared-leadership meta-analyses
aren't about whole companies. What we can say: *no configuration has better evidence than
"one accountable, removable executive + institutionalized voice + real delegation," and
the alternatives' failure modes (deadlock, Zappos-style exodus, inactive-founder veto) are
better documented than their successes.*

---

## 5. The contribution engine

### 5.1 Requirements the engine must satisfy

From requirement 2 plus the situation: (a) objective enough that a spreadsheet computes
every share; (b) identical treatment of founders and employees; (c) handles one
retroactive unpaid year; (d) handles ongoing unpaid work; (e) prices code, management, and
vision without a judging panel; (f) doesn't poison the future cap table.

### 5.2 The base: a modified Slicing Pie

The only developed practitioner framework for exactly this situation — bootstrapped,
unpaid, uneven-commitment teams — is Moyer's Slicing Pie: **a contribution's "slices" =
its fair market value × a risk multiplier (2× for time/non-cash, 4× for cash)**, and a
person's equity = their slices ÷ all slices [R-45]. A UK advisory that runs it reports
investors accept it *pre-*round but priced rounds require crystallization [R-48]; a US
law firm that implements it reports it has "virtually eliminated equity disputes" in
their client base while warning that US legal/tax infrastructure is "not geared toward"
it [R-46]. **There is no peer-reviewed evaluation of Slicing Pie or any dynamic split —
this is a practitioner framework, full stop** [R-1..R-6 find nothing]. Its academic
support is indirect: theory showing contingent founder contracts and vesting mitigate
team-formation inefficiencies [R-6]; evidence that heterogeneous contributions *should*
produce heterogeneous shares [R-1][R-5]; and the fairness literature's finding that
inequality with observable justification does not damage effort while opaque inequality
does [R-14][R-4] — a transparent ledger is precisely the "observable justification"
machine.

We adopt the 2×/4× multipliers as-published rather than inventing our own: they are the
established Schelling point, their rationale (risk premium on unpaid work and at-risk
cash) is coherent, and no data exists to tune them better. Deviating would spend
negotiating capital on an unfalsifiable parameter.

### 5.3 The modifications (each fixes a documented failure mode)

| Documented failure mode | Source | Our fix |
|---|---|---|
| "Fair market value" of a person's time is contestable | [R-47] | Rates are **role-based from a named published benchmark** (Schedule B: 50th-percentile Boston cash comp per role/level, e.g., levels.fyi US SWE median ≈$192.5K, senior ≈$312K total comp [R-49]), refreshed annually, methodology changes need 75% |
| Time inflation — unfocused hours out-earn shipped work | [R-47] | Hours creditable only on **Board-approved quarterly workstreams**; lead attestation; 250 h/month cap; 10% random audit; falsification = cause + 2× forfeiture |
| "Vision"/management either over- or under-valued | (design issue) | Vision, management, and business planning are credited **as hours in the appropriate benchmarked role** (engineering-manager, product/business-lead, executive rates). The role commands a market premium; the ideas themselves earn nothing extra — consistent with Spolsky ("ideas earn nothing") [R-51] and with pricing observability [R-14] |
| Commit-counting gets Goodharted | (design issue) | Git history is **evidence, not metric** — used to corroborate logged hours, never to compute slices |
| No cliff → two-week contributors keep slices | [R-47] | Minimum engagement threshold for new participants **[bracketed]**, plus for-cause forfeiture; main protection is that slices only accrue for approved work actually attested |
| Moving split = ownership anxiety, cap-table churn, tax events | [R-46][R-50] | **Units are issued once per quarter and never re-priced or clawed back**; the split moves only because the denominator grows. LLC profits-interest mechanics (Rev. Proc. 93-27/2001-43 [R-56]) make quarterly issuance non-taxable if papered correctly; protective 83(b)s within 30 days [R-58] |
| Investors won't price a moving pie | [R-48][R-32] | Hard **Freeze Event** (§8): the pie bakes into a fixed cap table at the earlier of a priced round, conversion, or 36 months — exactly Moyer's own bake trigger (breakeven/Series A) [R-45] |
| Purely mechanical systems miss outcome quality | (design issue) | Optional, bounded **outcome-bonus pool** (≤10% of a quarter's slices, unanimous board, written public reasons) — bracketed because it reintroduces subjectivity; the founders should decide with eyes open |

### 5.4 Why transparency is load-bearing

The ledger, every participant's slices, and running percentages are visible to all
participants by default. This is not a nicety: the single best causal result in the
adjacent literature is that pay inequality suppresses output and attendance **only when
coworker productivity is unobservable** [R-14]; dispersion that is explained and
performance-based is neutral-to-positive [R-14b]; and perceived-justice spirals in
founding teams run on whether the split's rationale is legible [R-4]. A secret ledger
would recreate the exact pathology this design exists to cure.

### 5.5 Handling the retroactive year

One-time reconstruction (Art. VII): everyone submits monthly hours per workstream with
evidence; contemporaneous artifacts (git, PRs, calendars, docs) credit at 100%,
recollection-only at 50% [bracketed]; 60 h/week cap; same rates and multipliers as
go-forward. An initial Ledger Committee including one outside independent scores it,
publishes drafts, takes objections, and individual disputes go to fast-track arbitration
without blocking everyone else. Precedent for retroactive credit: Cooley GO explicitly
blesses "retroactive credit reflecting their respective periods of work before
incorporation" when imposing vesting late [R-32].

### 5.6 Worked example (illustrative numbers — the spreadsheet is the spec)

Schedule B (illustrative; from published benchmarks [R-49], ÷2,080 h):
SWE-L3 $67/h · SWE-L4 $82/h · SWE-L5 $106/h · EngMgr $115/h · Product/Biz lead $96/h ·
ML research consultant (documented external rate [R-52]): $400/h.

Year-1 reconstruction (hours are post-evidence-weighting; ×2 non-cash multiplier; cash ×4):

| Person | Basis | Slices | % of slices |
|---|---|---:|---:|
| F1 (biz lead 60% / L5 40%, 2,300 h; +$20k expenses) | 2,300×$100×2 + 20,000×4 | 540,000 | 14.05% |
| F2 (L5, 2,200 h) | 2,200×$106×2 | 466,400 | 12.14% |
| F3 (EngMgr/L5 blend $110, 1,800 h) | 1,800×$110×2 | 396,000 | 10.30% |
| F4 (L5, 700 h — semi-active) | 700×$106×2 | 148,400 | 3.86% |
| F5 (L5, 350 h then inactive; +$5k cash) | 350×$106×2 + 5,000×4 | 94,200 | 2.45% |
| E1 (L5, 2,000 h) | 2,000×$106×2 | 424,000 | 11.03% |
| E2 (L4, 1,900 h) | 1,900×$82×2 | 311,600 | 8.11% |
| E3 (L4, 1,700 h) | | 278,800 | 7.25% |
| E4 (L3, 1,500 h) | | 201,000 | 5.23% |
| E5 (L4, 1,400 h) | | 229,600 | 5.97% |
| E6 (L3, 1,200 h) | | 160,800 | 4.18% |
| E7 (L4, 1,000 h) | | 164,000 | 4.27% |
| E8 (L3, 900 h) | | 120,600 | 3.14% |
| E9 (L3, 800 h) | | 107,200 | 2.79% |
| E10 (L3, 600 h) | | 80,400 | 2.09% |
| Professor (150 h × $400) | 150×$400×2 | 120,000 | 3.12% |
| **Total** | | **3,843,000** | 100% |

If (purely for illustration) a Freeze happened at month 12: founders F1–F3 have 12/36
RFA months each (1.667% each), F4 has 6 (0.833%), F5 has 3 (0.417%) → RFA issued 6.25%,
Contribution Pool 93.75%. Resulting fully-diluted:

| | Pool share | +RFA | **Total** |
|---|---:|---:|---:|
| F1 | 13.17% | 1.67% | **14.84%** |
| F2 | 11.38% | 1.67% | **13.05%** |
| F3 | 9.66% | 1.67% | **11.33%** |
| F4 | 3.62% | 0.83% | **4.45%** |
| F5 | 2.30% | 0.42% | **2.72%** |
| E1 | 10.34% | — | **10.34%** |
| E2–E10 | 38.34% | — | **38.34%** |
| Professor | 2.93% | — | **2.93%** |

Note what the system does without anyone having to fight about it: the top employee
out-owns two founders (identical terms, requirement 2); the inactive founder holds 2.7%,
not the ~20% a static equal split would have fossilized — small enough that investors'
dead-equity tolerance (~≤2% for departed contributors; 25–40% is a deal-killer [R-33])
is nearly met even in the worst case; and the professor's "decent share" priced itself
at ~2.9% via his own market rate and actual hours (§7).

---

## 6. Founders: reserved allocations, inactivity, departures

### 6.1 The 5% reserved allocations (requirement 1)

Each founder's 5% accrues **1/36 per month of Active Service (≥120 h/month)** over 36
months, with retroactive credit for active Year-1 months, hard stop at month 36, no
make-ups. Design logic:

- *Why time-based accrual rather than milestones:* milestone vesting invites definitional
  litigation; service-based vesting is the industry's convergent solution (92% of
  venture-backed companies; 4-year/1-cliff standard [R-31]). Our 36 months + 12 months'
  retroactive credit ≈ the standard 4-year total, matching Cooley's back-vesting pattern
  [R-32].
- *Why an activity threshold instead of mere employment:* "use it or lose it" is the
  founders' own requirement; 120 h/month (~0.75 FTE) is the bracketed default defining
  genuinely active.
- *Why unearned RFA dissolves into the pool pro rata (not to other founders):* keeps the
  founder class from having any collective interest in a colleague's failure, and
  automatically rewards everyone actually working.

### 6.2 Inactive founders — every dimension

| Dimension | Treatment | Rationale |
|---|---|---|
| Past work | Paid in full through the retroactive ledger, same rate as anyone | Perceived-justice evidence [R-4]; removes the legitimate kernel of their claim |
| Reserved 5% | Only months actually served accrue; window closes at month 36 | Requirement 1; dead-equity discipline [R-33][R-34] |
| Future equity | Identical ledger access if they return to approved work | Identical-terms requirement; no punishment, no privilege |
| Governance | No founder-qua-founder rights anywhere; board seats are elected annually | Founder-control valuation discount [R-13]; inactive vetoes are the failure mode |
| Title | "Founder" is historical fact, not a legal status | — |
| Buyout | None forced; earned units are theirs. For-cause misconduct → repurchase option at lower of ledger value/FMV | §6.4 |

The result in numbers (worked example): a founder inactive since month 3 ends with ~2.7%
— visible, defensible, and roughly at the edge of investor dead-equity tolerance [R-33],
versus 20% under the original handshake.

### 6.3 Why not claw back or strip votes

We considered mandatory buybacks of earned units and vote-stripping for non-service
members, and rejected both: earned-equity confiscation invites exactly the fiduciary/
freeze-out litigation Massachusetts is famous for (close-corporation "utmost good faith
and loyalty" duties extend to LLCs: *Donahue*, *Allison v. Eriksson* [R-43]), and it
poisons the perceived-justice channel that keeps the eleven active people motivated
[R-4]. Retention pressure comes from the RFA, refresh grants at conversion, and
investor re-vesting — the standard stack [R-31][R-32].

### 6.4 Departures

Encoded in Art. X: no-fault leavers keep earned units and accrued RFA fraction (dead
equity stays structurally small because nothing unearned exists to keep); for-cause
leavers face repurchase of everything at the lower of ledger value or FMV; fraud forfeits
2× falsified slices. This is deliberately softer than Slicing Pie's own recovery
framework (which strips all non-cash slices from anyone resigning "without good reason"
[R-45b]) — that regime is an enforceability and morale risk we flag rather than adopt
**[bracketed for the founders: adopting full Slicing Pie recovery is defensible if
counsel blesses it]**.

---

## 7. The professor

**Promise:** "a decent share," informally, expecting a higher rate than others.
**Constraint:** requirement 2 says all non-RFA equity flows through one identical-terms
system.

**Resolution: his higher rate is real and objective — it is his market consulting rate.**
PhD-level ML consulting bills $250–500/h (up to $1,000) [R-52] versus ~$67–115/h
engineering rates; the identical *rules* price his hours at 3–5× everyone else's. In the
worked example, 150 part-time hours already yield ~2.9% — more than 10× the median
pre-seed advisor grant (0.21–0.275%, Carta, 20k+ advisors [R-53]) and above the FAST
ceiling (1% for expert-level engagement at the earliest stage [R-54]). "Decent," by any
market benchmark, and every basis point of it earned and auditable.

Why not a special class or a fixed floor: (a) it breaks requirement 2 and re-opens every
other side-deal; (b) market norms say special professor stakes are the canonical cap-table
regret — advisor medians are ~0.05–0.28% by stage and falling [R-53], SAB norms for
eminent scientists are 0.1–0.3% plus day-rate cash [R-55]; (c) the evidence that star
names help is real but conditional — prominent affiliates accelerate IPOs and raise
proceeds *when quality is opaque* (a Nobel affiliate was worth >$30M in early-biotech
IPOs), and the signal decays as markets mature [R-60][R-61]; the benefits come from
*engaged* stars doing real work with the team, not from names on decks [R-59]. Our
system pays exactly for engagement, which is exactly what the evidence values.

If he demands a guarantee anyway, the bracketed fallback (Art. XI.3) is a market-norm
advisor option grant at the Freeze Event — 0.10–0.50%, 2-year monthly vesting, the Carta/
FAST band [R-53][R-54] — approved by 66⅔% because it steps outside the system. Our
recommendation: offer ledger participation + SAB-chair title; if he walks over a
guarantee, the data say the company loses less than it thinks.

**Counsel must clear (Art. XI.4):** Yale's one-day-per-seven-day-week consulting limit
and restrictions on management roles [R-62]; Yale COI disclosure and management plans,
including any involvement of his students [R-63]; Yale's patent policy asserting
ownership of inventions made with significant university resources, with consulting
inventions reportable to Yale Ventures (Yale's standard startup license itself takes
3–5% of founder shares — a reason to keep the IP boundary bright) [R-64]; NIH/PHS rules
making *any* equity in a private company a disclosable significant financial interest if
he is on PHS-funded research [R-65]; and supersession of the informal promise (with
promissory-estoppel exposure assessed).

---

## 8. Entity, tax, and the investor path

**Recommendation: run the ledger inside the existing Massachusetts LLC for a bounded
period, then convert to a Delaware C-corporation — deliberately early (target within
6–12 months, at latest 24), not "when a term sheet forces it."**

Why the LLC phase at all: the dynamic ledger is only tax-feasible in a partnership —
quarterly issuances can be profits interests with no tax at grant (Rev. Proc. 93-27 /
2001-43 [R-56]), whereas a corporation issuing stock quarterly against a moving ledger
would create repeated taxable comp events [R-50]. The company is already an MA LLC and
already needs a retroactive settlement computed *before* any conversion fixes percentages.

Why convert early and definitively:

1. **Investability.** VC funds structurally avoid LLCs (tax-exempt-LP UBTI [R-25]); the
   NVCA document stack assumes a Delaware corporation [R-27]; ~88% of Carta C-corps are
   Delaware [R-26]; standard SAFEs presume a corporation, and LLC-adapted SAFEs are
   friction investors reject [R-35].
2. **QSBS.** LLC interests can never be QSBS; the §1202 clock starts only at conversion.
   Post-OBBBA (stock issued after July 4, 2025): 50%/75%/100% exclusion at 3/4/5 years,
   $15M per-issuer cap (or 10× basis), $75M gross-asset ceiling [R-57]. Every month of
   delay is a month of forfeited holding period for 15+ people. (The known counter-
   argument — converting *later* at higher FMV enlarges the 10×-basis cap [R-57b] — is
   real but second-order for a pre-revenue company against the certainty of starting the
   clock; we flag it for counsel rather than resolve it.)
3. **The partner-tax problem gets worse every quarter.** Anyone holding a profits
   interest is a partner, not an employee — K-1s, self-employment tax, no W-2 (Rev. Rul.
   69-184 [R-56b]). Running ~16 partners is manageable briefly and miserable at scale;
   phantom-unit alternatives keep people W-2 but sacrifice capital-gains treatment
   [R-56c]. Conversion dissolves the whole problem into ordinary equity comp under a
   Rule 701 plan [R-44].
4. **Mechanics (counsel):** Massachusetts provides no outbound statutory conversion of an
   LLC into a (Delaware) corporation — c. 156C § 69 runs inbound-only — so the route is a
   merger into a new DE corp (c. 156C §§ 59–63; >50% of unreturned contributions to
   approve) or an interests-over §351 exchange per Rev. Rul. 84-111 [R-39][R-57c].
   Counsel picks the method; the operating agreement pre-wires member consent (Art. XII)
   so no one can hold up the financing.

At conversion (a Freeze Event): the Art. VI.5 arithmetic fixes the cap table; a standard
equity incentive plan is adopted (~15% initial pool; seed norms 10–15%, Carta median
employee pool 12.1%, Index recommends 12.5–15% [R-31b][R-34b]); go-forward work is paid
in salary + refresh grants, not ledger slices; and members have pre-committed to accept
up to bounded investor re-vesting (investors typically want founders ≤~40% vested at
Series A [R-32]). Double-trigger acceleration norms apply [R-31c].

---

## 9. Legal risk register (for counsel; ranked)

1. **Wage Act / FLSA — severe, immediate** (§1 above; [R-36][R-37][R-38][R-40][R-41]).
   Design assist: admitting all contributors as members with governance and information
   rights strengthens (does not guarantee) a bona-fide-partner characterization — the
   only FLSA carve-out found is the 20%+ owner-manager exemption [R-41b], which cannot
   cover ten rank-and-file people. Counsel must drive: raise-and-pay plan, characterization
   analysis, settlement/release strategy (Wage Act rights are not waivable "by special
   contract" [R-36]), and whether "past services" recitals in grant paperwork create
   admissions (no authority found either way — flagged, not resolved).
2. **Securities compliance** for ~16 grantees: Rule 701 written-plan discipline and its
   $10M/12-month disclosure trigger; Massachusetts blue-sky exemption to be confirmed
   [R-44].
3. **Tax mechanics:** profits-interest thresholds, protective 83(b)s (30-day,
   non-extendable; IRS Form 15620 e-filing now available [R-58]), K-1 logistics,
   §351/84-111 conversion, QSBS qualification at conversion [R-56][R-57].
4. **IP chain of title:** confirmatory PIIAs back to inception from every contributor —
   the most common early-stage diligence failure [R-66]; open-source audit; the
   Yale/professor boundary (§7).
5. **Massachusetts fiduciary overlay:** close-corporation duties extend to LLCs
   (*Donahue* → *Allison*) [R-43]; MA does not clearly permit Delaware-style duty
   elimination (c. 156C § 63 "expand or restrict" vs. 6 Del. C. § 18-1101(c)
   "eliminate") [R-43b] — draft the settlement and any repurchases with minority-fairness
   process; this is also a quiet extra argument for the Delaware conversion.
6. **Restrictive covenants:** Massachusetts noncompetes require garden leave (≥50% of
   highest base over prior 2 years) or other agreed consideration, cap at 12 months, and
   fail entirely against people terminated without cause — rely on NDAs + nonsolicits
   instead [R-67].
7. **Housekeeping once payroll starts:** workers' comp, withholding, D&O/EPLI.

---

## 10. Where the evidence is thin, and where it disagrees (stated plainly)

1. **No peer-reviewed test of dynamic equity exists.** Slicing Pie's support is
   practitioner experience plus indirect theory [R-6][R-46]. We adopted it because the
   founders' requirement 2 demands a contribution-metering system and it is the most
   battle-tested one; not because science validates it.
2. **The strongest practitioner voice disagrees with metering altogether.** YC's Seibel:
   split near-equally, "99% of the work is left to be done" [R-24]. The Hellmann &
   Wasserman result cuts the other way but is explicitly correlational — weak teams sort
   into quick equal splits; nobody has shown re-splitting causes better outcomes [R-1].
   Our freeze-and-convert ramp is the synthesis: metering for the unequal-commitment
   bootstrap phase, the YC-style standard stack afterward.
3. **Governance evidence is level-of-analysis-limited** (§4.2 close): team-level
   meta-analyses, 8-firm case studies, and archival correlations. Rotating leadership has
   no evidence base at all. We report the envelope honestly and chose the configuration
   whose *failure modes* are best documented as avoidable.
4. **Fairness evidence is from wages, not equity.** The Breza RCT and dispersion
   literature [R-14][R-14b] concern pay; extrapolation to equity is plausible, untested.
5. **The professor's signaling value is context-dependent.** Star-affiliation effects are
   strongest exactly where this company sits (young, hard-to-evaluate deep tech) and
   decay with market maturity [R-60][R-61]; evidence for *passive* name-advisors is
   essentially nil (§7).
6. **Numbers we could not verify** are bracketed in the operating agreement rather than
   asserted (e.g., the 50% evidence discount, the 120 h/month threshold, the 10% audit
   rate — these are design choices, not findings).
7. **Verification limits:** all web sources were verified via live search-retrieved page
   content because this environment's egress policy blocks direct page fetches; two
   GitHub-hosted sources were fetched directly. Details per-source in
   `plan-5-references.md`. We saw no other team's branch or content at any point.

---

## 11. Implementation sequence (90 days)

| When | What |
|---|---|
| Week 0 | Engage MA employment counsel (Wage Act) + startup corporate counsel. Freeze all new oral promises. |
| Weeks 1–2 | Founders resolve the [bracketed] decision points; adopt the Amended & Restated Operating Agreement; sign supersession acknowledgments; confirmatory PIIAs from everyone. |
| Weeks 2–6 | Year-One reconstruction (Art. VII): submissions, committee scoring, objection window. Stand up the ledger tooling (a spreadsheet suffices; Pie Slicer-class software optional [R-45c]). |
| Weeks 6–8 | Retroactive settlement units issued (profits interests + 83(b)s); board elected; CEO appointed; Schedule B rate table published; quarterly workstreams approved. |
| Weeks 8–12 | Professor: Yale disclosures initiated, consulting agreement + ledger enrollment signed (or the bracketed advisor-grant fallback negotiated). Wage-mitigation plan (financing to fund minimum payroll) in motion. |
| Months 6–12 | Delaware conversion executed per counsel (Art. XII); QSBS clock starts; Rule 701 plan + ~15% pool adopted. |

*— plan5*
