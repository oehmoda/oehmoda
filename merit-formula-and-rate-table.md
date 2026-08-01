# Merit Formula & Market-Rate Table (draft Schedule B to [Plan 1](plan-1-operating-agreement.md))

*The complete, specific formula for allocating the 75% merit pool among founders and employees, designed for a team of software engineers splitting time across coding, management, and business/vision work. Built to be auditable in investor diligence. Sources: [`references.md`](references.md).*

---

## 1. The formula (one line)

For each person, each quarter:

```
Slices earned = Σ over role-buckets [ (market salary for bucket − actual cash salary, prorated) ÷ 2000 × creditable hours in bucket ] × 2
              + unreimbursed cash contributed × 4
```

Your merit-pool share at any time = your cumulative slices ÷ everyone's cumulative slices. Multipliers (2x non-cash, 4x cash) per [Moyer, *Slicing Pie*](https://slicingpie.com/the-magic-of-mutipliers/). Someone paid at or above market accrues zero time slices — nothing at risk.

## 2. Pricing the work, not the worker

Everyone may be a software engineer by background; slices are earned at the rate of the **work actually performed**, in three buckets:

| Bucket | What counts | What does NOT count |
|---|---|---|
| **Engineering (IC)** | Design, coding, review, infra, debugging, technical docs | — |
| **Management** | Running people/processes: 1:1s, hiring pipeline, planning, coordination | Attending meetings someone else runs |
| **Business & vision** | Fundraising prep, customer development, sales, partnerships, business/technical strategy *that produces an artifact* (deck, model, spec, roadmap) | Unstructured "thinking about the company"; ideas without artifacts |

Three rules make this investor-clean:

1. **Ex-ante role split, not retroactive self-classification.** Each person's bucket split (e.g., "70% eng / 20% mgmt / 10% business") is set **in advance** each quarter by the board, following the DRI map — you accrue at the rates of your *assigned* split. Genuine mid-quarter changes are re-approved by the board, never back-dated. This kills the classic failure mode: everyone re-describing their coding hours as "vision" at the highest rate.
2. **Rates come from published benchmarks, not negotiation.** Each rate = the 50th percentile for the role and geography from [Carta compensation data](https://carta.com/data/) / Pave / levels.fyi equivalents, refreshed annually. Nobody argues their own number; you argue the benchmark source once, at ratification.
3. **The premium for leadership work is modest by design.** Market data prices early-stage management and business roles only ~10–25% above senior IC engineering — not multiples. The research backs this: execution dominates, and idea/vision work commands a small premium (~5% of a split, per [Shapiro 2011](https://www.danshapiro.com/blog/2011/04/startup-cofounder-equity-split/)), while YC's argument that long-horizon motivation beats short-term point-scoring cautions against any founder-flattering rate inflation ([Seibel/YC](https://www.michaelseibel.com/blog/how-to-split-equity-among-founders)).

## 3. Example rate table (placeholders — replace with current benchmarks for your geography at ratification)

| Role bucket | Example market salary | Hourly (÷2000) |
|---|---|---|
| Software engineer (mid) | $130,000 | $65 |
| Software engineer (senior) | $165,000 | $82.50 |
| Staff engineer / tech lead / CTO-track vision work | $195,000 | $97.50 |
| Engineering management | $185,000 | $92.50 |
| Product / business strategy | $170,000 | $85 |
| CEO bucket (fundraising, sales leadership, external) | $195,000 | $97.50 |

Deliberate properties: the spread between the lowest and highest rate is **1.5x, not 5x** — a heavy-contributing engineer is never structurally dominated by someone with a leadership label; sustained volume of contribution, not rate, is what moves the needle. Seniority within a bucket is assigned by the board against the benchmark's leveling definitions, once, at ratification (revisable prospectively at annual rate refresh).

## 4. Hours: evidence standards and anti-gaming caps

- **Creditable hours cap: [50]/week.** Prevents hour-inflation contests; beyond the cap you're donating, same as everyone.
- **Contemporaneous logging, lightweight:** a weekly one-line log per bucket (tool of choice), submitted monthly. Late logs (>30 days) credit at 50%.
- **Evidence on request:** commits/PRs for engineering; calendars and hiring records for management; artifacts (decks, models, specs, signed customers) for business/vision. The board certifies quarterly; the Independent Manager resolves disputes finally ([Plan 1 §5.3](plan-1-operating-agreement.md)).
- **Retroactive backfill** (founding → now): same buckets and rates, reconstructed from evidence, self-certified, board-approved, then **final** ([Plan 1 §5.4](plan-1-operating-agreement.md)). Protocol in §4b below.

### 4b. Backfill protocol (the past year — coarse by design)

Hour-by-hour reconstruction of the past year is false precision that manufactures disputes. Instead:

1. **Default-hours convention:** for each active month, credit every person a standard **[45] hrs/week** regardless of actual hours, unless a person claims a material deviation *and* brings evidence. Per person per month, only three facts are needed: active or not (≥[20] hrs/week test), role split, and cash compensation paid.
2. **Evidence already exists:** git/PR history (engineering), calendars and payroll (management, salaries), bank statements (cash). No diaries required.
3. **Sensitivity reality:** ±10% on hours moves a final percentage by well under a point; **active-vs-inactive months and paid-vs-unpaid dominate the outcome**. Negotiate the activity timeline, not hour counts.
4. **Process:** each person submits a months × role-split × pay grid → published to all participants → board approval → Independent Manager resolves disputes → **final and non-reopenable** ([Plan 1 §5.4](plan-1-operating-agreement.md)).
5. **Sequencing:** sign the MOU (rules) **before** running the backfill (numbers). Agreeing on the formula before anyone sees their own result is a veil-of-ignorance fairness device — and prevents rule-negotiation aimed at flattering one's own outcome ([procedural-justice basis: Breugst et al. 2015](https://ideas.repec.org/a/eee/jbvent/v30y2015i1p66-94.html)).

Go-forward logging remains as in §4: one line per week per bucket, submitted monthly — the upside ledger, not a timesheet.

## 5. Worked example (one quarter, 13 weeks)

Assume all unpaid except C (paid $60k against a $165k market rate).

| Person | Assigned split | Hours/wk | Calculation | Slices |
|---|---|---|---|---|
| Founder A (CEO) | 60% CEO / 40% senior eng | 45 | (351h × $97.50 + 234h × $82.50) × 2 | **107,055** |
| Founder B | 100% senior eng | 50 | 650h × $82.50 × 2 | **107,250** |
| Employee C | 100% senior eng, salary gap $105k → $52.50/h | 45 | 585h × $52.50 × 2 | **61,425** |
| Founder D (inactive) | — | 0 | — | **0** |
| Employee E | 100% mid eng + paid $4,000 of expenses | 40 | 520h × $65 × 2 + $4,000 × 4 | **83,600** |

Note what the numbers show: the CEO does *not* dominate (A ≈ B — the title buys ~18% higher rate on some hours, nothing more); the below-market employee (C) meaningfully out-earns the inactive founder (D) automatically; cash out of pocket (E) is rewarded without negotiation. This is the behavior investors want to see documented: equity tracking risk and contribution, mechanically.

## 6. Why investors prefer this over the alternatives

1. **Versus subjective/negotiated splits:** every number traces to a benchmark, a log, or a bank record — diligence is a spreadsheet review, not depositions. Perceived procedural justice is also what keeps the team stable en route ([Breugst et al. 2015](https://ideas.repec.org/a/eee/jbvent/v30y2015i1p66-94.html)).
2. **Versus output/OKR-gated equity:** metric-gated equity invites gaming and sandbagging; input-priced equity with performance governing *role retention* is the cleaner separation ([Doerr](https://www.betterworks.com/magazine/doerr-reveals-his-company-management-secrets-in-measure-what-matters); design decision in [implementation plan §5](implementation-plan.md)).
3. **The one thing they dislike — a moving cap table — is pre-solved:** the automatic freeze at the priced round converts the ledger to fixed units before any investor prices it ([Silicon Hills Lawyer 2015](https://siliconhillslawyer.com/2015/06/01/founder-equity-grunt-funds/); [Moyer freeze](https://support.thepieslicer.com/article/show/112619-how-do-i-freeze-bake-terminate-the-pie)).

## 7. What this formula deliberately does NOT do

- **No idea/vision multiplier.** Vision work earns the strategy-bucket rate on real hours with artifacts — no special premium beyond that. Execution dominance is one of the most consistent findings in the literature ([Shapiro](https://www.danshapiro.com/blog/2011/04/startup-cofounder-equity-split/); [Seibel/YC](https://www.michaelseibel.com/blog/how-to-split-equity-among-founders)).
- **No quality multiplier.** Quality is handled by role assignment (the board routes important work to strong people), annual rate leveling, and role reassignment for underperformance — not by a subjective per-quarter judgment call that would reintroduce politics.
- **No founder premium.** Founder status is already compensated by the 5% set-aside; inside the pool, everyone competes on identical terms — the defining feature of this company's deal.
