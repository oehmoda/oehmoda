# Implementation Plan: 5%-Base + 75% Merit Pool

*Tailored framework: each founder guaranteed 5% max (25% total); the remaining 75% earned competitively by founders and employees on identical contribution-based terms. Optimized for investability. Companion to the [one-pager](founder-governance-and-equity-one-pager.md); inline citations link to primary sources, with the full annotated bibliography in [`references.md`](references.md).*

---

## 1. The capital structure

### Layer 1 — Founder Base Units: 5% per founder, 25% total

- **Vesting, not a gift:** each founder's 5% reverse-vests over 4 years, monthly, 1-year cliff, **retroactive to the founding date** — so every founder is already ~25% vested (~1.25% of the company each). The 4yr/1yr-cliff standard and reverse-vesting mechanics: [Carta](https://carta.com/learn/equity/stock-options/vesting/), [Capbase](https://capbase.com/founder-vesting-schedules-best-practices/), [Seibel/YC](https://www.michaelseibel.com/blog/how-to-split-equity-among-founders). Vesting **pauses when a founder stops actively working** (defined objectively: fewer than X hours/week for 2+ consecutive months, certified quarterly by the board) — vesting as the commitment device, per [Wasserman 2012](https://press.princeton.edu/books/paperback/9780691158303/the-founders-dilemmas).
- **Why this is investor-friendly:** an inactive founder ends up with only their vested ~1.25%, not 5% — total possible "dead equity" stays in low single digits even if two founders walk. Investors treat >10–15% dead equity as a diligence red flag ([Capbase](https://capbase.com/founder-vesting-schedules-best-practices/)); this design caps it by construction.
- **Leaver terms:** unvested base units repurchased at cost automatically on departure or sustained inactivity. Bad leaver (cause, breach, abandonment) → company may repurchase *vested* units at the lower of cost or fair value; good leaver → keeps vested units, subject to ROFR and drag-along ([Bird & Bird](https://www.twobirds.com/en/insights/2025/leaver-provisions-the-terms-that-founders-fear-the-most); [Ashfords](https://www.ashfords.co.uk/insights/blog/leaver-provisions-balancing-founder-fairness-and-company-protection)).

### Layer 2 — Merit Pool: 75%, dynamic until freeze

Everyone — founders and employees alike — earns from the same pool by the same formula (Slicing Pie mechanics, [Moyer](https://slicingpie.com/the-magic-of-mutipliers/) — the only widely-adopted framework for exactly this situation; note it has practitioner adoption but no peer-reviewed validation, per the evidence review in [`research/academic-literature.md`](research/academic-literature.md) §3):

- **Slices = fair market value of at-risk contribution × multiplier** ([Moyer's canonical multipliers](https://slicingpie.com/the-magic-of-mutipliers/)):
  - Unpaid or below-market **time**: (market salary − actual salary) ÷ 2000 hrs × hours worked × **2**
  - **Cash** in (expenses, capital beyond agreed contributions): amount × **4**
  - Ideas/IP/relationships brought in: appraised FMV × 2
- **Your % of the pool = your slices ÷ total slices**, recalculated quarterly from a shared ledger.
- **Someone paid full market rate accrues nothing** — nothing at risk, no slices ([Moyer](https://slicingpie.com/the-magic-of-mutipliers/)). This is what makes "employees compete equally with founders" true and fair: a below-market employee grinding nights outearns a checked-out founder automatically, with no politics. The stabilizing force is *perceived procedural justice*, which formula-driven transparency provides ([Breugst et al. 2015](https://ideas.repec.org/a/eee/jbvent/v30y2015i1p66-94.html)).
- **Backfill from founding:** the first ledger entry reconstructs everyone's contributions from day one using an agreed market-rate table (§4). This is the renegotiation moment — do it once, sign it, never reopen it. Contingent/deferred allocation under uncertainty is exactly what theory recommends ([Hellmann & Thiele](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=1968696)); waiting longer only hardens positions ([Hellmann & Wasserman 2016](https://pubsonline.informs.org/doi/10.1287/mnsc.2016.2474) on failed renegotiations).
- **Freeze event:** at the earlier of (a) a priced equity round, or (b) two consecutive quarters of profitability with market-rate salaries ([Moyer's freeze guidance](https://support.thepieslicer.com/article/show/112619-how-do-i-freeze-bake-terminate-the-pie)). At freeze, pool percentages become fixed units; **new-hire equity thereafter comes from a conventional 10–15% option/profits-interest pool** carved at the round ([Carta](https://carta.com/data/founder-ownership/); [Index Ventures](https://www.indexventures.com/rewarding-talent/)).

### Post-freeze vesting

Frozen merit-pool units are 50% vested at freeze, remainder over 24 months. Rationale: Series A investors routinely demand founder re-vesting anyway ([Capbase](https://capbase.com/founder-vesting-schedules-best-practices/)) — pre-building it removes a negotiation and signals sophistication. Double-trigger acceleration (change of control + termination without cause within 12 months) on everything — the investor-standard form ([Carta](https://carta.com/learn/equity/stock-options/vesting/)).

## 2. The two investability risks in this design — and the fixes

1. **Dynamic equity is a diligence problem if it's still moving at fundraise time.** VCs will not price a cap table that changes quarterly — the standard legal critique of grunt funds ([Silicon Hills Lawyer 2015](https://siliconhillslawyer.com/2015/06/01/founder-equity-grunt-funds/)). Fix: the freeze trigger is *automatic and pre-signed* — the term sheet itself freezes the pie. Keep the ledger clean and exportable from day one; it becomes your diligence artifact instead of your liability.
2. **Leadership can end up too thin.** If 15 people split 75% and the CEO lands at 8%, seed investors will worry about long-horizon motivation — founder teams hold a median ~56% post-seed ([Carta Founder Ownership Report 2025](https://carta.com/data/founder-ownership/)), and equity-driven motivation is a core YC argument ([Seibel](https://www.michaelseibel.com/blog/how-to-split-equity-among-founders)). Fix: monitor a **leadership-ownership floor** — if at freeze the CEO + top 2 executives would hold under ~30% combined, the board rebalances with top-up grants from the new option pool before the round. Don't distort the formula; patch at the edges.

## 3. Entity strategy: LLC now, Delaware C-corp at the round

- **Stay an MA LLC while the pie is dynamic** — quarterly reallocation is clean in an LLC (capital accounts) and a nightmare in a corporation (repeated grants, 83(b) chaos) ([Silicon Hills Lawyer](https://siliconhillslawyer.com/2015/06/01/founder-equity-grunt-funds/), which notes dynamic models fit LLCs pre-financing).
- **Grant employees profits interests** (tax-free at grant under Rev. Proc. 93-27/2001-43, capital-gains treatment; [Carta](https://carta.com/learn/startups/compensation/equity-incentive-plans/profits-interest/); [Lyons Gaddis](https://www.lyonsgaddis.com/profits-interests-in-llcs-a-tax-friendly-alternative-to-stock-options/)) for merit-pool participation. Note the friction: holders become K-1 partners, not W-2 employees ([Carta](https://carta.com/learn/startups/compensation/equity-incentive-plans/profits-interest/)). If that's too heavy for ~10 employees, use **phantom units** tracking the ledger until conversion ([Startup Law Blog](https://www.thestartuplawblog.com/the-complete-guide-to-equity-compensation-for-startups/)).
- **Convert to a Delaware C-corp at (or just before) the freeze/priced round.** Institutional investors expect it: standard NVCA docs, stock options, and QSBS eligibility — LLC interests can never qualify under §1202, and the 5-year exclusion clock starts at conversion, so don't convert *later* than the round ([Carta](https://carta.com/learn/startups/compensation/equity-incentive-plans/profits-interest/); [Startup Law Blog](https://www.thestartuplawblog.com/the-complete-guide-to-equity-compensation-for-startups/)). LLC interests map to common stock per the frozen ledger.

## 4. The market-rate table (sign it before the backfill)

Agree these *before* anyone computes their own number: a market salary per role (use Carta/[Index OptionPlan](https://www.indexventures.com/optionplan/)-style benchmarks for your geography, mid-band), an hourly rate = salary ÷ 2000 ([Moyer's convention](https://slicingpie.com/the-magic-of-mutipliers/)), and evidence standards for retroactive hours (calendars, commits, deliverables — good-faith estimates certified by each person and approved by the board). Cash contributions verified against bank records. Disputes → the independent board member decides (casting-vote pattern, [Jacobs Law](https://thejacobslaw.com/preventing-business-standstills/)). Lock multipliers at 2x/4x.

## 5. Governance (unchanged from the one-pager, now with teeth)

- Manager-managed LLC; **board of 3** (CEO + one active founder elected by members + one independent chosen unanimously) — pre-seed norm of small founder-controlled boards ([NYU](https://entrepreneur.nyu.edu/blog/2026/07/20/startup-board-structure/); [Rho](https://www.rho.co/blog/startup-board-composition); LLC board mechanics per [UpCounsel](https://www.upcounsel.com/llc-board-of-managers)).
- **One CEO**, DRI map for every function ([CRV](https://www.crv.com/content/what-is-a-co-founder); [Pilot](https://pilot.com/tactical-guide/cofounders)), titles reassignable by board vote ([Wasserman 2012](https://press.princeton.edu/books/paperback/9780691158303/the-founders-dilemmas); [HSG](https://www.hsgcap.com/article/founder-to-ceo-transition/)).
- Tiered decision rights ([ABA](https://www.americanbar.org/groups/gpsolo/publications/gpsolo_ereport/2022/july-2022/llc-agreement-checklist/); [LegalClarity](https://legalclarity.org/llc-supermajority-voting-for-amendments-how-it-works/)): CEO discretion (< $25–50K) → board majority → 75% member supermajority (new members, unit issuance, manager removal, asset sales) → unanimity only for fundamental economic rights and dissolution.
- Quarterly: OKR review + contribution-ledger certification in the same meeting; annual 360 founder reviews; board reviews CEO ([Doerr](https://www.betterworks.com/magazine/doerr-reveals-his-company-management-secrets-in-measure-what-matters)).
- Deadlock ladder: negotiation → mediation → independent's casting vote → Texas-shootout buy-sell ([Jacobs Law](https://thejacobslaw.com/preventing-business-standstills/); [LegalClarity](https://legalclarity.org/texas-shootout-clause-how-it-works-risks-and-tax-rules/)).

## 6. 90-day roadmap

| Phase | When | What |
|---|---|---|
| **1. Ratify** | Weeks 1–2 | All-founder meeting. Sign a 2-page MOU: 5% bases with retroactive vesting, 75% merit pool with 2x/4x formula, freeze triggers, one named CEO, board of 3, market-rate table process. Get all five signatures **now** — the framework needs unanimity, the 5% base is what makes it palatable to inactive founders, and renegotiation gets monotonically harder ([Hellmann & Wasserman 2016](https://pubsonline.informs.org/doi/10.1287/mnsc.2016.2474)). |
| **2. Backfill** | Weeks 2–4 | Build the retroactive ledger (founding → today) for all 15 people. Each person self-certifies; board approves; publish internally — transparency is the fairness mechanism ([Breugst et al. 2015](https://ideas.repec.org/a/eee/jbvent/v30y2015i1p66-94.html)). |
| **3. Paper it** | Weeks 4–8 | Lawyer drafts: amended & restated operating agreement (manager-managed, board, tiered voting, vesting, leaver/deadlock/transfer terms per the one-pager's [MA notes](founder-governance-and-equity-one-pager.md#massachusetts-specific-notes-for-the-lawyer)), profits-interest or phantom plan, IP assignments + confidentiality from **everyone** (the Snapchat lesson, [TechCrunch 2017](https://techcrunch.com/2017/02/02/snapchat-reggie-brown/)), noncompetes tied to equity sale, not employment ([Beck Reed Riden](https://beckreedriden.com/quick-guide-to-massachusetts-new-noncompete-law/)). |
| **4. Operate** | Weeks 8–12 | First quarterly cycle: OKRs set, ledger certified, percentages published. Communicate the full system to employees — the pitch writes itself: *you earn ownership on the same terms as the founders.* |
| **Ongoing** | Quarterly | Ledger + OKR cadence. Re-check the leadership-ownership floor (§2). At term sheet: freeze, convert to Delaware C-corp, carve new option pool. |

## 7. What to bring the lawyer

The MOU from Phase 1, the market-rate table, the backfilled ledger, the one-pager's MA-specific notes (c. 156C §63 fiduciary tailoring, ROFR/tag/drag, deadlock definitions — sources in [`references.md`](references.md) §D), and this document. Ask them to draft, not design — the design decisions are made here.
