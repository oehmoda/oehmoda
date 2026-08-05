# Founder Ownership and Seed-Round Readiness

**Memo to:** The Founding Team
**From:** Firas
**Re:** Sequencing our seed-round readiness, and fixing the one cap-table variable our plan leaves uncontrolled
**Date:** August 2026 · **v2** — revised after an independent investor-perspective review; this version corrects the dilution model, adds CEO-level numbers, and ranks the ownership question inside the full readiness list.

---

## Summary

Our equity plan is strong where most startups are weak: everything vests, inactive people stop earning automatically, and every share traces to documented work. But we are not seed-ready, and the ownership question this memo raises is **fourth** on the list, not first. Items one through three are legal exposures that could kill a round outright; item four — the subject of this memo — is that the founders' combined ownership at the freeze is an *output of a ledger nobody has computed*, with realistic outcomes landing well below what funded companies look like. The fix proposed here is a **floor-and-collar**: the founder class lands between 50% and 65%, trued up through a neutral reserve, with contribution mechanics preserved inside every layer. It binds founders in both directions, costs nothing if our projections come out fine, and is nearly impossible to add after signatures.

## The seed-readiness list, in the order investors will read it

1. **Employment and wage compliance, per jurisdiction — before any signatures.** Fifteen people have worked unpaid time for a Massachusetts LLC over the company's life — nine current, six departed — spread across **Massachusetts, Texas, the UK, and India**. Each person's *local* law governs: the MA Wage Act (mandatory treble damages, *personal* liability for managing founders) for MA-based workers; federal FLSA for Texas; UK national-minimum-wage rules; Indian employment law. Equity cannot legally substitute for wages in any of these. The sharpest exposure is the **departed** workers — current teammates rarely sue; removed ones do — and wage claims generally cannot be waived by a simple release. Counsel must structure the lookback and the settlement payments together, jurisdiction by jurisdiction. Workstream #1.
2. **Settle the six departures in writing.** Two departed members contributed real work: compute their share with the **same backfill formula as everyone else** — nobody negotiates, the ledger decides — then prefer a **cash buyout at today's independently supported (near-nominal) valuation** over leaving them on the cap table; settling now is when fair is also affordable. If equity must remain: funded from the reserve, combined single digits, votes proxied, drag-along bound. Two contributed minimally — the formula will price that honestly (likely a token amount; pay it, it is cheap insurance). Two never started and receive nothing. **All six sign separation agreements with releases and IP-assignment confirmations** — six undocumented departures is six open claims.
3. **Paper the two oral promises.** A professor was promised "a decent share" (with university IP and conflict-of-interest exposure attached), and a fifth person was promised "equal partnership." Undocumented equity promises are the classic eight-figure diligence killer (Snap paid Reggie Brown $157.5M). Both need written agreements — the professor's conditioned on Yale COI/IP clearance — before we ratify anything.
4. **Fix the freeze trigger.** The ledger freezes at a "priced round" — but seed money now usually arrives via SAFEs, which the trigger ignores. Extend it: cumulative financing threshold, change of control, or a date-certain backstop.
5. **Control the founder-ownership outcome.** The rest of this memo.

## Why the founder number is uncontrolled today

Current team: **four cofounders and five employees.** (Older plan documents model five founders and fifteen people; every document should be reconciled to the restructured team before ratification.)

- Each cofounder's 5% reserve (**20% combined**) is a ceiling, not a grant — earned monthly while active; unearned portions flow into the shared pool.
- The remaining **80%** is earned by cofounders and employees under identical rules. With five employees against four cofounders and a deliberately compressed rate table (max 1.5×), hours decide the split.

Projected cofounder class at the freeze (pre-round), with sensitivity on relative hours:

| Scenario | Equal hours | Founders log 1.25× | Founders log 1.5× |
|---|---|---|---|
| All four cofounders active | ~56% | ~60% | ~64% |
| One cofounder inactive | ~48% | ~52% | ~55% |
| Two cofounders inactive | ~38% | ~42% | ~45% |

Now translate honestly to **post-round** — because the current plan has no reserve, a seed round costs ~20% *plus* a 10–15% option pool investors require us to create before their money ([standard mechanics](https://carta.com/learn/startups/equity-management/option-pool/); seed dilution data: [Carta](https://carta.com/data/state-of-private-markets-q1-2025/)):

- **Best case** (all active, equal hours): 56% at freeze → **~39–41% post-seed**, versus the funded-company median of **56.2%** ([Carta, 45,000+ startups](https://carta.com/data/founder-ownership-2026/)).
- Even the most founder-favorable sensitivity (1.5× hours) lands ~45% post-seed — still ~11 points under the median.
- **The CEO's line — the first number investors actually read:** at equal hours the CEO holds ~14% at freeze → **~10% post-seed → ~6–7% by Series A**. For a four-founder company, low-teens post-seed is defensible; single digits invites the motivation question in every partner meeting.

To be precise about what this is: none of these outcomes *forecloses* fundraising — corrected round-over-round math (see below) keeps even weak cases above the hard floors. The problem is that we would **enter every round below the median with no cushion, by accident rather than by decision** — and that nobody, today, can tell the team which row of this table we are living in.

The plan does contain a patch — a leadership floor (CEO + top two at ~30% at freeze, topped up from the new option pool). It is insufficient for this problem: it triggers only at the round, from a pool investors control, with tax friction, in exactly the negotiation we should not be having then.

## The evidence, corrected

**1. The dilution ladder.** Dilution is multiplicative, not additive. From Carta's medians: seed→A retains ×0.64, A→B retains ×0.64 ([Carta](https://carta.com/data/founder-ownership-2026/)):

| Post-seed position | Post-Series A | Post-Series B |
|---|---|---|
| 39% (our best case, current plan) | ~25% | ~16% |
| 48% (proposed structure) | ~31% | ~20% |
| 56% (median company) | 36% | 23% |

Every path clears the catastrophic floors — but the current plan's *best* case reaches Series B where the median company sits two full rounds earlier. "No cushion" is the accurate description.

**2. Split structure affects what investors pay.** The largest study of founder splits ([Hellmann & Wasserman, *Management Science* 2016](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=1805427); 3,700+ founders) finds that splits set without deliberate negotiation are associated with a valuation penalty around **10% of firm equity value** at first financing. Read carefully, it cuts both ways: it argues for deciding *deliberately and now* — and it warns against fixing shares *detached from contribution*, which is why the proposal below keeps contribution mechanics inside every layer and routes forfeitures to a neutral reserve rather than to anyone's windfall.

**3. The mechanism investors act on.** Operators with large personal stakes perform better — agency theory ([Jensen & Meckling 1976](https://www.sciencedirect.com/science/article/pii/0304405X7690026X)) and founder-CEO performance evidence ([Fahlenbrach 2009](https://ideas.repec.org/a/eee/empfin/v16y2009i1p136-150.html); public-firm scope, honestly noted). This is why seed investors screen the CEO's line first.

**4. Market practice.** Carta's platform data (the strongest source available): median founding team 56.2% post-seed, 36.1% post-A; median employee pool at seed **12.1%** ([report](https://carta.com/data/founder-ownership-2026/)). Practitioner commentary consistently treats founders below investors combined, and large inactive stakes, as diligence flags ([SaaStr on departed founders](https://www.saastr.com/how-vcs-think-about-departed-co-founder-equity-stakes/); [Equity Matrix](https://equitymatrix.io/blog/what-investors-look-for-in-cap-tables) — practitioner sources, weighted accordingly).

## Proposed structure: floor-and-collar with a neutral reserve

| Layer | Size | Who | Mechanics |
|---|---|---|---|
| Founder base | 20% | 4 cofounders, 5% each | Earned monthly while active |
| Cofounder contribution pool | 40% | Cofounders only | Same slice formula, competed among cofounders |
| Employee contribution pool | 25% | Current employees | Same slice formula; a ceiling — unearned portions roll to the reserve |
| Neutral reserve | 15% | Company | Future hires; converts into the option pool at the round; balancing layer for the floor-and-collar |

**The rules that make it defensible:**

1. **All forfeitures — founder and employee alike — route to the neutral reserve.** Nobody's inactivity enriches a teammate. This preserves the current plan's single best diligence story ("dead equity is structurally zero") and removes the conflict of interest in inactivity rulings (certified by the Independent Manager).
2. **Floor and collar at the freeze:** if the active founder class would hold under **50%**, it is trued up from the reserve; anything above **65%** flows back to the reserve. The band binds founders in *both* directions — this is a stabilizer, not a founder giveaway.
3. **Everything still has to be earned.** No layer is a grant; the formula, logging, and vesting mechanics are unchanged inside each class.
4. **The arithmetic closes in every case.** If the fifth partner takes a 5% base, the cofounder pool drops to 35% (class ceiling unchanged at 60%). The professor's advisor grant (~1%, conditional on Yale clearance) and the Independent Manager's ~0.5% come from the reserve. Total is 100% under all outcomes.
5. **A pro-forma freeze cap table is published every quarter.** The "nobody can compute it" problem disappears at zero political cost — everyone, employee or founder, watches the same projection move.
6. **Distributed-team mechanics (MA / TX / UK / India).** Two decisions the rate table and unit classes must answer at ratification: **(a)** whether Rate-Card benchmarks are geo-adjusted or a single global rate — this materially moves accrual for non-US teammates and is a fairness call to make openly, once; **(b)** non-US residents should hold **phantom units tracking the ledger** rather than direct LLC interests until the Delaware conversion — direct holdings make them US K-1 taxpayers and trigger home-country rules (India FEMA/RBI, UK HMRC). IP assignments must be executed in local-law-valid form for each jurisdiction, or they do not actually protect us.

Post-round outcome at a standard ~20% seed with the reserve absorbing the pool requirement: founder class ~48%, employees ~20%, new investors ~20%, pool ~12% — unusual but explainable in one sentence: *the team worked unpaid for a year and earned it under audited rules.*

## What investors will see at the round

If we adopt this structure and clear the readiness list, the pro-forma at a standard ~20% seed round reads:

| Holder | Post-seed |
|---|---|
| Cofounders (4, active, fully vested schedules) | ~48% |
| — of which the CEO individually | ~13–16% |
| Employees (5, earned under audited rules) | ~20% |
| Unallocated option pool (from our reserve) | ~12% |
| Seed investors | ~20% |

And the diligence packet behind it: an audited contribution ledger where every percent traces to logged work or bank records; 100% of equity on vesting schedules; **zero dead equity by construction**; signed, locally-valid IP assignments from every past and present contributor in every jurisdiction; all six departures settled with releases; no outstanding oral promises (professor and fifth partner papered); employment compliance remediated with counsel across MA, TX, UK, and India; one designated CEO with a meaningful personal stake. Most seed-stage companies can show two or three of these. A company that can show all of them has turned its cap table from a diligence risk into a closing argument.

## Both tails are company risks

The goal is the company's best odds, which means avoiding two failure modes: **founders too thin** (below ~50% pre-round → every raise needs us to be the exception, and the CEO's line invites the motivation question) and **employees too thin** (for a nine-person company running on unpaid work, losing two engineers over equity resentment is as lethal as a failed round). The floor-and-collar addresses both symmetrically: employees keep a pool ~2× the market norm with identical earning rules, founders accept a hard cap, and the reserve — not any person — absorbs every adjustment. The floor's cost is bounded and visible; the downside it prevents is not.

## Anticipated objections

**"This is self-serving — you're proposing it before the backfill, exactly what the plan's veil-of-ignorance rule prohibits."**
Deciding class sizes *before* anyone sees their individual number **is** the veil of ignorance. Every cofounder faces the same uncertainty inside the cofounder pool; the collar caps our upside as firmly as the floor protects our downside; and forfeitures now flow to a neutral reserve instead of to remaining founders. I am proposing a rule I cannot tune to my own benefit — that is the definition of the veil, not a violation of it.

**"The employees were promised the same terms as founders."**
Within their pool, terms are identical: same formula, same rates, same evidence standards. Nothing is signed yet — this is the designed moment for setting parameters — and the offer remains roughly double the market-norm pool with upside no salaried startup matches. What changes is bounded class sizes, which is also what makes their equity *fundable* — and their equity is worth nothing if the company can't raise.

**"You might land fine anyway — why change?"**
Maybe we do. Then the floor never triggers, the collar never triggers, and the only thing we bought is a quarterly projection everyone can see. The cost of the mechanism in the good scenarios is zero; the cost of its absence in the bad ones is the round.

**"We can fix a thin founder position at the round with top-up grants."**
Top-ups come from the investors' pool, need their consent, carry tax friction, and happen in the exact negotiation where we have the least leverage — while renegotiating a signed split rarely succeeds because the advantaged side holds a veto ([Hellmann & Wasserman](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=1805427)). A floor written today needs no one's permission later.

**"Medians aren't rules; traction forgives cap tables."**
True. Exceptions pay for unusual cap tables with exceptional traction. Volunteering to need an exception — by accident — is not a strategy.

## Recommendation

1. **Start counsel-led employment/wage remediation now, across all four jurisdictions** (MA, TX, UK, India; current and departed workers) — it gates everything, including the signatures below.
2. **Settle all six departures in writing** — same-formula numbers for the two real contributors (cash buyout at today's near-nominal valuation preferred), token settlements for the two minimal ones, releases and IP confirmations from all six.
3. **Paper the professor** (~1% advisor grant conditional on Yale COI/IP clearance) **and the fifth partner** (5% base with pool offset, or cofounder-pool-only — written either way).
4. **Extend the freeze trigger** to cover SAFEs and add a date-certain backstop.
5. **Adopt the floor-and-collar structure** (20/40/25/15, forfeitures to reserve, 50–65% band) in the ratified agreement, with the distributed-team mechanics above (rate-card geography decision; phantom units for non-US residents).
6. **Designate exactly one CEO at ratification** — the plan requires it, and investors read that person's individual line first. Verify in the backfill projection that the CEO's stake lands in the mid-to-high teens at freeze; if it doesn't, fix it with the reserve before the round, not during it.
7. **Run the backfill covering all fifteen past and present contributors, and publish the first pro-forma freeze cap table** — then quarterly. Decide any remaining calibration on those numbers, as a team.
8. **Reconcile all plan documents** to the restructured team (4 cofounders, 5 employees, six settled departures) before anything is signed.

---

## Sources

- [Carta Founder Ownership Report 2026](https://carta.com/data/founder-ownership-2026/) · [2025](https://carta.com/data/founder-ownership/) — 45,000+ startups: founders 56.2% post-seed, 36.1% post-A, 23% post-B; employee pool 12.1% at seed.
- [Carta, State of Private Markets](https://carta.com/data/state-of-private-markets-q1-2025/) — seed-round dilution ~20%.
- [Carta, Option Pool mechanics](https://carta.com/learn/startups/equity-management/option-pool/) — pre-money pool creation.
- [Hellmann & Wasserman, "The First Deal," *Management Science* 63(8) 2016](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=1805427) ([NBER w16922](https://www.nber.org/papers/w16922)) — ~10%-of-equity valuation penalty for non-deliberative splits; stickiness of signed splits.
- [Jensen & Meckling, *JFE* 1976](https://www.sciencedirect.com/science/article/pii/0304405X7690026X) — agency costs and operator ownership.
- [Fahlenbrach, *J. Empirical Finance* 2009](https://ideas.repec.org/a/eee/empfin/v16y2009i1p136-150.html) — founder-CEO firm performance (public-firm scope).
- Practitioner commentary (weighted as such): [SaaStr on departed-founder equity](https://www.saastr.com/how-vcs-think-about-departed-co-founder-equity-stakes/) · [Equity Matrix on cap-table diligence](https://equitymatrix.io/blog/what-investors-look-for-in-cap-tables) · [Qubit Capital on Series A cap-table mistakes](https://qubit.capital/blog/cap-table-mistakes-series-a).
- This repo: [`implementation-plan.md`](implementation-plan.md) (incl. §2 leadership floor, Wage Act flag) · [`merit-formula-and-rate-table.md`](merit-formula-and-rate-table.md) (formula, §1b counsel flags, §6b professor) · [TechCrunch on Snap/Reggie Brown](https://techcrunch.com/2017/02/02/snapchat-reggie-brown/).
