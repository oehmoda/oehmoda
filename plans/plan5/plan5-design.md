# plan5 — Governance & Equity Design for a Five-Founder Massachusetts LLC

**Prepared by team plan5 · 2026-08-01**

This document states the complete recommended framework and the evidence behind each
choice. Citations like **[A1]**, **[B2]**, **[C3]** point to the annotated
bibliography in `plan5-references.md`, which carries full URLs and per-source
evidence-strength ratings. The article-by-article encoding for counsel is
`plan5-operating-agreement.md` ("OA"). A summary is in `plan5-one-pager.md`.

**Two honesty notes up front.**
(1) *Verification:* our research environment blocked all direct page fetches; every
source was corroborated through live web-search results showing matching page
content, and none is cited from memory — but none could be fetch-verified either.
Details in the references file's disclosure section.
(2) *Isolation:* we did not read, check out, or browse any other team's branch or
files at any point; our branch began as an empty tree.

---

## 0. The design in one paragraph

Stay an LLC just long enough to run a one-time retroactive true-up and a dynamic
contribution ledger tax-efficiently, then convert to a Delaware C-corp at the first
real financing, when the cap table freezes. Equity comes from exactly two channels:
a 25% founder reserve earned in quarterly use-it-or-lose-it tranches against an
objective activity test, and a 75% contribution pool in which founders, employees,
and the professor accrue points under one public formula — hours × published
market rate × 2 for unpaid work, cash × 4 — with the professor's "higher rate"
honored only as his *documented* consulting market rate, capped at 2% total.
Governance is a three-seat elected board, a single accountable CEO on a renewable
12-month term, and DRI-owned day-to-day decisions sorted by Amazon's
one-way/two-way-door test; disputes ride a mediation→arbitration ladder that keeps
the company out of court. Inactive founders keep exactly what they earned, stop
accruing, and can be bought out at appraised fair value before a round. The single
most urgent action item is not equity at all: ten unpaid employees at a for-profit
Massachusetts company is an accruing wage-law violation with mandatory treble
damages and personal founder liability, and it must be fixed before any of this
matters.

---

## 1. Entity and tax path: LLC now, Delaware C-corp at the freeze

**Recommendation.** Remain a Massachusetts LLC while the dynamic split runs; convert
by statutory conversion into a Delaware C-corporation at the Freeze Event (first
qualified financing, breakeven, or sale — OA 1.4, 3.3), with every member's
pre-consent locked in now.

**Why not convert immediately?** Because the equity system the founders mandated —
a continuously recomputed, contribution-based split — is *far* cheaper to run in an
LLC. Partnerships can shift relative ownership percentages without the taxable
compensation events a corporation triggers on every re-grant [C1-criticisms:
Equity Matrix], and LLC profits interests can deliver equity to workers with no tax
at grant and no 409A appraisal [B10, B12]. Running quarterly reallocations in a
C-corp would generate either repeated taxable stock grants or an option-repricing
treadmill.

**Why convert at all — and why Delaware?** Institutional VCs structurally avoid
pass-through entities: tax-exempt LPs face UBTI, and K-1s are unmanageable across a
portfolio [B13-AngelList]; the standard early-stage instruments (YC SAFEs) are
drafted for Delaware corporations only [B13-YC/Cooley]; and Delaware is the default
domicile investors underwrite [B13-Cooley]. Converting also opens §1202 QSBS
treatment for everyone's post-conversion holding period: for stock issued after
July 4, 2025, the OBBBA regime gives a 50/75/100% exclusion at 3/4/5-year holds,
with a $15M per-issuer cap and a $75M gross-asset ceiling [B9]. Two timing forces
cut against each other: converting **earlier** starts everyone's QSBS clock sooner
and preserves gross-asset headroom, while converting **later** raises the 10×-basis
alternative cap because basis is set at FMV of assets at conversion (§1202(i))
[B9-FoxSwibel/HansonBridgett]. For a company whose exit ambitions exceed ~$15M per
holder, the modeling matters; we bracket it for tax counsel (OA 3.3) rather than
pretend one answer dominates.

**The instrument trap we designed around.** Profits interests convert into C-corp
stock only to the extent of value *above their hurdle*; interests granted shortly
before conversion can convert into approximately nothing [B10-BakerTax]. Since our
ledger issues equity continuously right up to the freeze, a naive
profits-interest-only implementation would systematically cheat late contributors —
mostly employees. OA 3.6 therefore forces counsel to choose per tranche among
(a) profits interests, (b) low-value capital interests with 83(b) elections
(30-day hard deadline; IRS Form 15620, e-filable since July 2025 [B11]), or (c) a
single catch-up issuance at the freeze immediately before conversion. This is the
kind of trap that makes us confident the "stay-LLC-briefly" path needs a tax lawyer
in the loop from day one — but it is a solvable implementation detail, not a reason
to abandon the design.

**Massachusetts specifics for counsel** (flagged, not resolved): the exact MA-side
filing route for an outbound conversion is genuinely unclear in secondary sources
(156C merger vs. surrender filings — [B7]); after conversion the Delaware entity
must register as a foreign corporation in MA within 10 days of commencing business
and remains subject to MA corporate excise [B16].

---

## 2. The equity system

### 2.1 Why a formula-driven dynamic split (and the strongest argument against it)

The founders' requirement #2 mandates a contribution-based system on identical
terms. The evidence says the *way* to do that is a self-executing formula, not
periodic renegotiation:

- Founder teams that split quickly and equally — 73% of teams split within a month
  of founding [A3]; 42% settle in a day or less [A1] — obtain lower first-round
  valuations and raise outside money less often, with roughly 10% of equity
  (~$450K NPV for a typical startup) at stake [A1]. The authors read this as
  *selection* (teams that dodge the hard conversation), not causation — which is
  exactly the point: a written, contribution-based system is the credible signal
  that this team did the hard conversation.
- Renegotiation does not happen voluntarily. Longitudinal registry data shows
  equal-splitting teams exhibit "dynamic fairness preference" — they almost never
  adjust relative stakes even as contributions diverge; stakes move mainly when
  outside financings force it [A9-2019]. This team's own history (an informal
  reallocation agreement that was never executed while contributions diverged) is a
  textbook instance. A system that requires a future vote to rebalance will not
  rebalance. The formula must be self-executing.
- Contract theory supports contingency: static upfront splits lock in ineffective
  founders, pure delay invites idea appropriation, and contingent contracts with
  vesting mitigate both — most valuable precisely when founder-skill uncertainty is
  high [A9-2015]. Unconditional equal shares in a 15-person team also sit squarely
  in Holmström's 1/N free-rider result: each member bears full effort cost for
  1/15th of the marginal payoff [A6].

**The counterargument, stated fairly.** Y Combinator advises the opposite: split
equally or near-equally, because "all the work is ahead of you" over a 7–10-year
horizon and "more equity equals more motivation" [C4]; and Carta data shows the
market has *moved toward* equal splits among two-founder teams (45.9% in 2024, up
from 31.5% in 2015) [C3]. We take this seriously and answer it three ways. First,
the YC fact pattern — a two-person team at day zero with no contribution history —
is not this company: five founders, a year of sharply divergent contribution, and
ten employees who out-contributed some founders. Equal-split logic degrades with
team size even in Carta's own data (only 16.7% of four-founder teams split
equally) [C3]. Second, YC's motivational argument is about *prospective* incentive,
which our design preserves: every active founder can still earn their full 5%
reserve plus an uncapped share of the 75% pool going forward. Third, the founders'
requirement #2 forecloses relitigating this — our job was to check whether the
evidence made the requirement unwise, and it does not: the strongest empirical
result in the area [A1] cuts *against* the quick equal split for teams whose
contributions have already diverged.

**What the fairness literature adds.** Perceived *justice* of the split, not its
equality, is what drives positive vs. negative team spirals [A2]; procedural
justice has effects on commitment independent of outcomes [A10]. Design
consequences: rules published before outcomes; one public rate table; no negotiated
side deals; a ledger any member can audit; appeal rights to a neutral (OA 4.2, 7.4,
12.2). We also deliberately chose **earned-is-kept** for departures (see §2.5).

### 2.2 The two channels

**Founder Reserve — 25%, earned quarterly, never granted** (OA Art. V). Each
founder's 5% divides into 16 tranches of 0.3125% across the 16 quarters after
formation. A tranche is earned only if the founder met an *objective* Active
Service test that quarter — ≥240 accepted hours, or points ≥50% of the median
full-time participant, whichever is lower (OA 1.4). Missed tranches recycle
irrevocably into the contribution pool. This implements requirement #1 literally
("use it or lose it") and matches the market's near-universal 4-year earning
horizon for founder equity: 4-year/1-year-cliff is the standard, and where grants
have cliffs, ≥95% sit at one year [C3-vesting]; YC calls founder vesting the one
thing you don't innovate on [C4]; investors will demand it anyway [C5-Feld,
B14-Cooley]. We use quarterly earn-in rather than a single cliff because the cliff
year has already passed and the problem here is *ongoing* divergence, not early
flight.

**Contribution Pool — 75% plus recycled reserve** (OA Art. IV). A points ledger on
Slicing Pie arithmetic [C1]: percentage = your points ÷ all points × pool size.
Points accrue as:

| Contribution | Formula | Basis |
|---|---|---|
| Unpaid time | hours × Rate(level) × **2.0** | Slicing Pie non-cash multiplier [C1] |
| Cash invested | dollars × **4.0** | Slicing Pie cash multiplier [C1] |
| Unreimbursed approved expenses | dollars × **4.0** | cash-equivalent [C1] |
| Contributed property/IP (appraised) | FMV × **2.0** | non-cash [C1] |
| Underpaid time once salaries start | (market − cash paid) × **2.0** | at-risk gap only [C1] |

Nothing else earns points: no idea royalties, no title premiums, no tenure credit
(§2.5 explains the deviations). Hours count only when logged within 14 days, tied
to a deliverable in a DRI's area, and accepted — acceptance being a good-faith
existence check, not a performance grade, with written-reason rejection and appeal
(OA 4.5). The multipliers are risk compensation for unpaid/at-risk contributions —
the standard dynamic-equity convention [C1] — and sit behind a supermajority
amendment lock so they cannot be quietly retuned by whoever holds a majority
(OA 6.5).

### 2.3 The Rate Table: how "contribution" becomes dollars before it becomes points

All five founders are engineers whose work spans coding, management, and vision, so
the pricing question is the whole game. Our answer: **role-leveled market rates,
published in advance, identical for everyone at the same level** (OA 4.3).

- Rates = median US **startup** cash compensation per level (Carta startup payroll
  data as primary — new-hire startup engineers average ≈ $189K salary
  [C10-Carta]) ÷ 2,080 hours. We deliberately do *not* use big-tech total-comp
  medians (US senior SWE ≈ $312K [C10-levels.fyi]) as the base: the equity being
  earned *is* the risk premium — pricing hours at a number that already includes
  equity would double-count. The 2× multiplier then compensates the unpaid-cash
  risk on top of the startup-cash base.
- Management hours are priced at a management-level rate only for hours actually
  spent managing; vision/business-planning hours are priced at the contributor's
  own engineering-level rate. **There is no idea premium.** Slicing Pie itself
  prices only "the" founding idea, via revenue royalties [C1-FMV]; we drop even
  that, because in a five-engineer team a royalty on the shared founding idea is
  an unadministrable conflict generator, and the empirical founder literature
  associates idea-premium claims with the *antecedents* of unequal splits, not
  with any measured performance payoff [A1].
- Level assignments come from a published rubric, applied by the Allocation
  Committee, appealable like any ledger decision (OA 4.3, 12.2).

This is the mechanism that satisfies "identical terms" while still letting a
world-class specialist earn faster — the *rate*, not the *rules*, carries the
difference (§6).

### 2.4 Instrument and securities mechanics

Grants issue as LLC Incentive Units — default profits interests under the Rev.
Proc. 93-27/2001-43 safe harbors with liquidation-value hurdles, protective 83(b)s
within 30 days, and no 409A appraisal needed [B10, B11, B12-Notice2005-1] — subject
to the conversion-trap decision bracketed in OA 3.6 (§1 above). Every issuance
needs a securities exemption; Rule 701's compensatory exemption (12-month cap =
greatest of $1M / 15% of assets / 15% of the class) is the model, with counsel to
confirm its LLC application and whether quarterly reallocation is a "continuous
offering" problem [B12] (OA 11.5).

### 2.5 Where we deviate from Slicing Pie, and why

We adopt Slicing Pie's arithmetic (FMV × multiplier, all-slices denominator,
freeze at breakeven-or-financing) [C1] but deviate on four points, each for a
reason we can defend:

1. **Separation.** Slicing Pie strips a resigning-without-good-reason participant
   of all non-cash slices [C1-recovery]. We chose **earned-is-kept**: delivered
   value stays owned, accrual stops, and the company holds an appraised-FMV call
   after four fully-inactive quarters (OA 9.1–9.3). Three grounds: (a) perceived
   injustice — retroactively zeroing a colleague's delivered year — is precisely
   the trigger for the negative team spirals in [A2]; (b) a forfeiture that large
   invites exactly the litigation the dispute ladder is built to avoid, and
   Massachusetts courts' hostility to wage forfeitures [B2] makes aggressive
   clawbacks a bad bet for counsel to defend `[⚖ flagged in OA 9.4]`; (c) the
   investor problem Slicing Pie's rule solves — dead weight on the cap table — is
   solved less combustibly by the FMV call plus natural dilution. We keep true
   forfeiture only for Cause, narrowly defined (OA 9.4).
2. **No idea royalties, no relationship commissions** [C1-FMV] — dropped per §2.3;
   fundraising execution is creditable as hours (level B), not as a finder's fee,
   which for unregistered persons is also a securities-law tripwire `[⚖]`.
3. **A founder reserve exists at all.** Pure Slicing Pie has no reserved
   allocations; requirement #1 mandates one. At 25% max it is small enough to
   leave the pool dominant, and its use-it-or-lose-it earn-in makes it
   incentive-compatible rather than an entitlement.
4. **A hard freeze with pre-consents.** Slicing Pie freezes informally at
   breakeven/Series A [C1]; we hard-wire the trigger, the conversion, the option
   pool, and investor-standard reverse vesting into pre-agreed obligations
   (OA 3.3–3.5, 10.2), because the known investor objection to dynamic equity is
   not the concept but the residual uncertainty at diligence time
   [C1-criticisms: EquityMatrix; C5].

Honest caveat: **no peer-reviewed outcome study of Slicing Pie or any dynamic-split
framework exists** (we looked — references Part C, "could not support" item 5).
Its support is indirect: the renegotiation-failure evidence [A9], the
contingent-contracting theory [A9-2015], the fairness-process literature [A2, A10],
and practitioner reports that dynamically-split companies have raised through
multiple rounds [C1-Fairsquare]. We adopt its arithmetic because it is the only
published, administrable convention for pricing at-risk contributions — while
hard-wiring the freeze so the unconventional machinery is gone before investors
arrive.

### 2.6 Worked example (the spreadsheet test)

Illustrative Year-1 true-up, plausible for this team (16 people; rates E3 $72/h,
E4 $94/h, E5 $115/h from a $150K/$195K/$240K table pending signing-date
benchmarks; multipliers ×2 time, ×4 cash). Full-time = 45 h/wk credited per
OA 4.8 defaults.

| Person | Year-1 pattern | Points | Pool share (of 77.81%*) | Reserve earned | **Total today** |
|---|---|---:|---:|---:|---:|
| F1 | E5, FT all 4 quarters + $20K cash | 576,800 | 15.64% | 1.250% | **16.89%** |
| F2 | E4, FT all 4 quarters | 406,080 | 11.01% | 1.250% | **12.26%** |
| F3 | E4, FT 2 quarters, then 15 h/wk | 270,720 | 7.34% | 0.625% | **7.96%** |
| F4 | E3, FT Q1 only, then dormant | 77,760 | 2.11% | 0.3125% | **2.42%** |
| F5 | E4, ~10 h/wk in Q1 only | 22,560 | 0.61% | 0% | **0.61%** |
| E1 | E4, FT from Q2 | 304,560 | 8.26% | — | **8.26%** |
| E2 | E3, FT from Q2 | 233,280 | 6.32% | — | **6.32%** |
| E3–E6 (each) | E3, FT from Q3 | 155,520 | 4.22% | — | **4.22%** |
| E7–E10 (each) | E3, 20 h/wk from Q3 | 69,120 | 1.87% | — | **1.87%** |
| Professor | ~100 h @ documented $400/h | 80,000 | 2.17% → **capped 2.00%** | — | **2.00%** |

\* Pool = 75% + 2.8125% recycled from the 9 founder-reserve tranches already
forfeited by F3/F4/F5. Total allocated to date: 81.25%; the remaining 18.75% is
future reserve tranches that will be earned or recycled over quarters 5–16.
Every number above is reproducible from the OA Article IV formulas — that is the
"spreadsheet could compute it" requirement, satisfied.

Sanity checks against market: senior employees E1–E2 land at 6–8% — well above the
post-A market range for salaried hires (#1 hire: 2–3% [C6-Holloway]) — correct,
because they worked a year *unsalaried*, which Holloway explicitly says warrants
more [C6]. The two dormant founders hold 0.6–2.4% instead of a reserved 5% each —
below the >5%-inactive-holder threshold one fund publishes as a dead-equity red
flag [C5-ISA]. The professor's cap binds at 2.0% — 2.5× the FAST expert-tier
ceiling for a startup-stage company (0.80%) and 8× Carta's pre-seed advisor median
(0.25%) [C2, C3-advisor], defensible as generous but bounded.

---

## 3. Governance

### 3.1 What the leadership evidence actually supports

We investigated the open question honestly — single leader, co-leaders, rotation,
consensus — and the evidence lands on a **hybrid**: genuinely distributed
decision-making below the top, one accountable executive at the top, both under an
elected board.

- Three meta-analyses agree shared leadership has a *positive* average association
  with team performance (ρ ≈ .15–.35 depending on measurement) [A4], and the one
  most relevant finding for structure is that shared leadership adds variance
  *over and above* vertical leadership — complement, not substitute
  [A4-Nicolaides]. They *disagree* about the task-complexity moderator (Wang:
  stronger under complexity; D'Innocenzo: weaker) [A4] — so we do not rest any
  design weight on complexity claims. All inputs are correlational, mostly
  non-founder teams; this evidence justifies distributing real authority, not
  abolishing the vertical role.
- On multi-CEO tops: the peer-reviewed result is that co-CEO pairs perform better
  the *larger* the power gap between them — i.e., co-leadership works when it
  approximates single leadership [A5-Krause]. The pro-co-CEO HBR piece (9.5% vs
  6.9% shareholder returns, n=87) is non-peer-reviewed and selection-biased
  [A5-Feigen]. Rotation among five founders multiplies the known costs (handoffs,
  ambiguous accountability) with no literature support we could find.
- The board is not optional decoration: venture boards are small,
  milestone-focused monitors whose structure investors will impose anyway
  [A8]; and an outside residual claimant is Holmström's own cure for team moral
  hazard [A6].

### 3.2 A single CEO — held on a 12-month renewable term, decoupled from equity

The base rate is that founder-CEOs get replaced: half are out of the seat by year
3, under 25% lead their IPO, and 4 of 5 departures are forced [A3]; the
*triggers* are success events — shipping product, raising money [A7]. Startups
usually absorb this as a traumatic investor-forced rupture. We build it into the
constitution instead: the board appoints the CEO for a renewable 12-month term,
from any member or outside, and non-renewal has **zero equity consequence**
(OA 6.3). Because pay-for-work runs entirely through the ledger and office
confers no points (OA 6.7), losing the title costs nothing but the title — which
is what makes a five-founder team able to choose its best available CEO rather
than its most entitled one. This is the rich-vs-king tradeoff [A3] resolved, in
advance, on the "rich" side for everyone.

### 3.3 The board

Three managers, all elected annually by all members, any active member eligible
(OA 6.2). No founder-reserved seats: requirement #2's identical-terms principle
extended to power, and dead-equity logic extended to board chairs. Sized to graft
cleanly onto a standard post-financing venture board [A8]. Removal by 60% vote
keeps managers accountable between elections.

### 3.4 Decision rights below the board

DRIs — one named owner per area, Apple-style [C7-Lashinsky] — hold day-to-day
authority, sorted by Amazon's test: reversible two-way-door decisions are made
fast at DRI level; consequential one-way-door decisions escalate [C7-Bezos2015]
(OA 6.4–6.5). One escalation per decision, then disagree-and-commit
[C7-Bezos2016] (OA 6.6). The reserved-matters list (sale, dissolution, formula
amendments, non-standard investor terms) requires 66⅔% of members plus the board
(OA 6.5). Rationale from the conflict literature: task conflict is not harmful —
especially in top teams and for decision quality — but relationship and process
conflict reliably are [A11]; the structure's job is to give task disagreement a
fast, impersonal channel (written proposals, named deciders, one appeal) so it
never curdles into the process-conflict pattern this team has already tasted.
These provenance sources are practitioner mechanisms, not outcome studies, and we
label them as such [C7].

---

## 4. The retroactive year

The unpaid Year 1 is handled by the same formula, seeded once (OA 4.8): each
person reconstructs hours from artifacts (commits, PRs, docs, calendars);
defaults of 45 h/wk (documented full-time months) / 15 h/wk (part-time) fill
evidence gaps; two-peer attestation plus committee acceptance; disputes go
straight to fast-track arbitration; the true-up closes in 120 days, hard.
Design intent: **retroactive fairness with a statute of limitations** — the
justice literature says the process being visibly fair matters as much as the
numbers [A2, A10], and the renegotiation literature says an open-ended true-up
would never close [A9-2019]. Founders and employees run through identical
machinery, which is what converts the informal "employees count too" promise into
something an employee could actually enforce.

## 5. Inactive founders

Every dimension, explicitly:

- **Equity:** keep what the ledger and reserve say they earned (F4: ~2.4%, F5:
  ~0.6% in the worked example) — nothing more. Unearned reserve is already gone
  (OA 5.4). No negotiation occurs because nothing is left to negotiate.
- **Future accrual:** zero unless they return to work; the system is indifferent
  to the label "founder" (OA 5.6).
- **Cap-table hygiene:** after four fully-inactive quarters the company can buy
  them out at appraised FMV on a 36-month schedule (OA 9.2), and is directed to
  exercise before a priced round (OA 9.6) — because an uninvolved >5% holder is a
  published diligence red flag and a departed co-founder with a large stake can
  kill a financing [C5-ISA]; the replacement-cost logic of founder vesting
  [C5-Wilson] is the same logic here.
- **Governance:** no reserved seats to lose; voting power floats down with their
  percentage automatically (OA 2.4).
- **Dignity:** earned-is-kept (§2.5) means the buyout is a valuation conversation,
  not an accusation — deliberately, per [A2].

## 6. The professor

The informal promise ("a decent share," "valued at a higher rate") is the design's
most dangerous liability if left informal, and its cleanest demonstration case if
formalized:

- **Share:** he accrues through the same ledger as everyone (requirement #2 —
  identical terms), and *only* through it. The written advisor agreement
  supersedes the oral promise, with a release `[⚖ OA 8.1]`.
- **Higher rate, objectively:** his Rate-Table rate is his *documented* external
  consulting FMV — invoices from arm's-length clients — capped at $450/h
  (OA 8.2). A genuine market premium flows through; an asserted one does not.
  This honors the promise's substance without granting a special deal.
- **Cap:** 2.0% at freeze (OA 8.3) — deliberately above the entire advisor-market
  range (FAST expert/startup tier: 0.80% [C2]; Carta pre-seed median: 0.25%
  [C3-advisor]) so "decent share" is defensibly true, and bounded so part-time
  involvement cannot compound into a dead-equity problem at diligence [C5].
- **Yale, before anything else** (OA 8.4): his outside work is limited to ~one day
  per seven-day week on average under Yale's external-activities policy; equity
  and startup roles trigger COI review; Yale's patent policy claims inventions
  made within employment scope or with more-than-minimal university resources;
  and if he holds federal grants, the equity arrangement is disclosable
  current-and-pending support [B17]. An IP-tainted ML model is a
  diligence-killer, so points accrue only after his COI confirmation and an IP
  boundary covenant are signed. If Yale's review forces a smaller role, the
  ledger simply prices the smaller role — the system degrades gracefully.

## 7. Disputes

The ladder (OA Art. XII): negotiation (10 days) → mediation (30 days) → binding
expedited arbitration in Boston; ledger appeals get a documents-only fast track;
valuation fights use final-offer ("baseball") arbitration — **our design choice
from general commercial ADR practice; we found no source pairing it with LLC
deadlock specifically, and flag it as such** [C8-honesty note]; last-resort
member deadlock uses a sealed-bid buyout auction with a fairness backstop
bracketed for counsel, since shotgun mechanisms demonstrably favor the
deeper-pocketed party [C8]. All of it exists because the failure base rates say
governance kills startups at rates rivaling product: 65% of high-potential
startup failures trace to people problems in the largest founder dataset [C9-
Wasserman]; 23%/13% of post-mortems cite team/disharmony in the (weaker,
self-reported) CB Insights sample [C9]. Med-then-arb tiers are the standard
contractual alternative to judicial dissolution [C8-ABA].

## 8. Legal risk register for counsel (flag, not resolve)

| # | Issue | Sources | Urgency |
|---|---|---|---|
| 1 | **Ten unpaid employees**: M.G.L. c.149 §148 violation accruing now; treble damages are mandatory and strict-liability (*Reuter*); founders personally liable as managers (*Cook*); equity cannot substitute for wages (29 C.F.R. §531.27; DOL); no volunteer or contractor escape (FLSA; §148B ABC test) | B1–B5 | **Immediate — before any equity work** |
| 2 | Retroactive-equity instrument choice (profits vs. capital interests vs. freeze catch-up); 83(b) discipline | B10, B11 | High |
| 3 | Securities exemptions for ledger issuances; quarterly reallocation as continuous offering? | B12 | High |
| 4 | Conversion mechanics: DE §265 route, MA-side filings (conflicting sources), §351/Rev. Rul. 84-111 method, QSBS timing model | B7–B9 | Before financing |
| 5 | Yale COI/patent-policy clearance and federal-grant disclosures before the advisor agreement | B17 | Before advisor signs |
| 6 | Enforceability of Cause forfeitures; 156C fiduciary-duty tailoring limits; implied covenant non-waivable | B2, B6 | Drafting |
| 7 | Noncompete policy under the 2018 MA Act (garden leave economics); NDAs/non-solicits outside the Act | B15 | Drafting |
| 8 | Oral-promise exposure to the professor; releases and integration clause | B17, OA 14.9 | With #5 |

## 9. Investor-readiness checklist (requirement #3, operationalized)

1. No dead equity: reserve recycling + FMV call + pre-round cleanup directive
   (OA 5.4, 9.2, 9.6) keeps uninvolved holders under red-flag thresholds [C5].
2. Founder ownership lands in market range: active founders in the worked example
   hold ~37% combined after one year, consistent with Carta's median founding-team
   ownership of 56.2% post-seed → 36.1% at Series A [C3] given this team's unusual
   width (5 founders, 10 employees).
3. Everything unconventional sunsets at the money: dynamic ledger, elected-board
   quirks, and LLC status all end at the Freeze Event; financing docs are NVCA
   forms; pre-consents (conversion, pool, reverse vesting, 1× non-participating
   preference) mean no member can hold up the round (OA 3.3–3.5, 10.2, XIII) [B14].
4. Diligence-ready from day one: data room, IP assignments from every past
   contributor as a condition of allocation, 83(b) receipts, board minutes
   (OA 11.2, 11.4).
5. QSBS positioned under the post-OBBBA regime for all post-conversion holders [B9].
6. The wage-law remediation (§8 #1) is itself an investor item: accrued Wage Act
   liability is a diligence discovery that kills or reprices rounds — fixing it is
   cap-table hygiene as much as compliance.

## 10. Evidence-strength summary — what we know vs. what we chose

- **Strong (statute/case/regulator):** the wage-law emergency; conversion and QSBS
  mechanics; profits-interest safe harbors; Yale's policies as written [Part B].
- **Strong-correlational (peer-reviewed, large-N):** quick-equal splits associate
  with worse financing outcomes (selection, per the authors) [A1]; voluntary
  renegotiation doesn't happen [A9-2019]; founder-CEO replacement base rates [A3,
  A7]; shared leadership complements vertical leadership [A4].
- **Mechanism-only (theory or small-N):** free-riding [A6]; contingent contracting
  [A9-2015]; justice spirals [A2, N=8]; venture-board propositions [A8].
- **Practitioner convention, no outcome data:** Slicing Pie arithmetic and
  multipliers [C1]; FAST advisor tiers [C2]; DRI/door-type/disagree-and-commit
  [C7]; deadlock mechanics [C8]; the >5% dead-equity threshold [C5].
- **Chosen by us where evidence ran out** (and labeled as such in place): the 2×/4×
  multiplier values (convention, not measurement); the 240-hour/50%-of-median
  Active Service thresholds; the 2.0% advisor cap; quarterly rather than monthly
  recomputation; baseball arbitration for valuations; earned-is-kept over Slicing
  Pie forfeiture. Each is a defensible point in a reasonable range, and each is a
  single parameter a future board can retune by the amendment rules without
  touching the architecture.

The literature disagrees in three places that matter here — task-complexity
moderation of shared leadership [A4], co-CEO performance [A5], and task-conflict
effects [A11 vs. its predecessor] — and in each case we designed so that either
side of the disagreement leaves the structure sound.
