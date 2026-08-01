# Implementation Plan: 5%-Base + 75% Merit Pool

*Tailored framework: each founder guaranteed 5% max (25% total); the remaining 75% earned competitively by founders and employees on identical contribution-based terms. Optimized for investability. Companion to the [one-pager](founder-governance-and-equity-one-pager.md).*

---

## 1. The capital structure

### Layer 1 — Founder Base Units: 5% per founder, 25% total

- **Vesting, not a gift:** each founder's 5% reverse-vests over 4 years, monthly, 1-year cliff, **retroactive to the founding date** — so every founder is already ~25% vested (~1.25% of the company each). Vesting **pauses when a founder stops actively working** (defined objectively: fewer than X hours/week for 2+ consecutive months, as certified quarterly by the board).
- **Why this is investor-friendly:** an inactive founder ends up with only their vested ~1.25%, not 5% — total possible "dead equity" stays in low single digits even if two founders walk. Investors treat >10–15% dead equity as a diligence red flag; this design caps it by construction.
- **Leaver terms:** unvested base units are repurchased at cost automatically on departure or sustained inactivity. Bad leaver (cause, breach, abandonment) → company may repurchase *vested* units at the lower of cost or fair value. Good leaver → keeps vested units, subject to ROFR and drag-along.

### Layer 2 — Merit Pool: 75%, dynamic until freeze

Everyone — founders and employees alike — earns from the same pool by the same formula (Slicing Pie mechanics, the only widely-adopted framework for exactly this situation):

- **Slices = fair market value of at-risk contribution × multiplier.**
  - Unpaid or below-market **time**: (market salary − actual salary) ÷ 2000 hrs × hours worked × **2**
  - **Cash** in (expenses, capital beyond agreed contributions): amount × **4**
  - Ideas/IP/relationships brought in: appraised FMV × 2
- **Your % of the pool = your slices ÷ total slices**, recalculated quarterly from a shared ledger.
- **Someone paid full market rate accrues nothing** — they have nothing at risk. This is the feature that makes "employees compete equally with founders" true and fair: a below-market employee grinding nights outearns a checked-out founder automatically, with no politics.
- **Backfill from founding:** the first ledger entry reconstructs everyone's contributions from day one using an agreed market-rate table (see §4). This is the renegotiation moment — do it once, sign it, never reopen it.
- **Freeze event:** at the earlier of (a) a priced equity round, or (b) two consecutive quarters of profitability with market-rate salaries. At freeze, pool percentages become fixed units; **new-hire equity thereafter comes from a conventional 10–15% option/profits-interest pool** carved at the round.

### Post-freeze vesting

Frozen merit-pool units are 50% vested at freeze, remainder over 24 months. Rationale: investors at a priced round routinely demand founder re-vesting anyway — pre-building it removes a negotiation and signals sophistication. Double-trigger acceleration (change of control + termination without cause within 12 months) on everything.

## 2. The two investability risks in this design — and the fixes

1. **Dynamic equity is a diligence problem if it's still moving at fundraise time.** VCs will not price a cap table that changes quarterly. Fix: the freeze trigger is *automatic and pre-signed* — the term sheet itself freezes the pie. Keep the ledger clean and exportable from day one; it becomes your diligence artifact instead of your liability.
2. **Leadership can end up too thin.** If 15 people split 75% and the CEO lands at 8%, seed investors will worry about motivation (Carta medians: founder teams hold ~56% post-seed). Fix: monitor a **leadership-ownership floor** — if at freeze the CEO + top 2 executives would hold under ~30% combined, the board rebalances with top-up grants from the new option pool before the round. Don't distort the formula; patch at the edges.

## 3. Entity strategy: LLC now, Delaware C-corp at the round

- **Stay an MA LLC while the pie is dynamic** — quarterly reallocation is clean in an LLC (capital accounts) and a nightmare in a corporation (repeated grants, 83(b) chaos).
- **Grant employees profits interests** (Rev. Proc. 93-27: tax-free at grant, capital-gains treatment) for merit-pool participation. Note the friction: holders become K-1 partners, not W-2 employees. If that's too heavy for ~10 employees, use **phantom units** tracking the ledger until conversion.
- **Convert to a Delaware C-corp at (or just before) the freeze/priced round.** Every institutional investor expects it: standard NVCA docs, stock options, QSBS (§1202 — the 5-year exclusion clock starts at conversion, so don't convert *later* than the round). LLC interests map to common stock per the frozen ledger.

## 4. The market-rate table (sign it before the backfill)

Agree these *before* anyone computes their own number: a market salary per role (use Carta/Pave/levels.fyi benchmarks for your geography, mid-band), an hourly rate = salary ÷ 2000, and evidence standards for retroactive hours (calendars, commits, deliverables — good-faith estimates certified by each person and approved by the board). Cash contributions verified against bank records. Disputes → the independent board member decides. Lock multipliers at 2x/4x.

## 5. Governance (unchanged from the one-pager, now with teeth)

- Manager-managed LLC; **board of 3** (CEO + one active founder elected by members + one independent chosen unanimously).
- **One CEO**, DRI map for every function, titles reassignable by board vote.
- Tiered decision rights: CEO discretion (< $25–50K) → board majority → 75% member supermajority (new members, unit issuance, manager removal, asset sales) → unanimity only for fundamental economic rights and dissolution.
- Quarterly: OKR review + contribution-ledger certification in the same meeting. Annual: 360 founder reviews; board reviews CEO.
- Deadlock ladder: negotiation → mediation → independent's casting vote → Texas-shootout buy-sell.

## 6. 90-day roadmap

| Phase | When | What |
|---|---|---|
| **1. Ratify** | Weeks 1–2 | All-founder meeting. Sign a 2-page MOU: 5% bases with retroactive vesting, 75% merit pool with 2x/4x formula, freeze triggers, one named CEO, board of 3, market-rate table process. Get all five signatures **now** — the framework needs unanimity, the 5% base is what makes it palatable to inactive founders, and every month of delay hardens positions. |
| **2. Backfill** | Weeks 2–4 | Build the retroactive ledger (founding → today) for all 15 people. Each person self-certifies; board approves; publish internally. |
| **3. Paper it** | Weeks 4–8 | Lawyer drafts: amended & restated operating agreement (manager-managed, board, tiered voting, vesting, leaver/deadlock/transfer terms per the one-pager's MA notes), profits-interest or phantom plan, IP assignments + confidentiality from **everyone**, noncompetes tied to equity sale (not employment — avoids the MA garden-leave rule). |
| **4. Operate** | Weeks 8–12 | First quarterly cycle: OKRs set, ledger certified, percentages published. Communicate the full system to employees — the pitch writes itself: *you earn ownership on the same terms as the founders.* |
| **Ongoing** | Quarterly | Ledger + OKR cadence. Re-check the leadership-ownership floor. At term sheet: freeze, convert to Delaware C-corp, carve new option pool. |

## 7. What to bring the lawyer

The MOU from Phase 1, the market-rate table, the backfilled ledger, the one-pager's MA-specific notes (c. 156C §63 fiduciary tailoring, ROFR/tag/drag, deadlock definitions), and this document. Ask them to draft, not design — the design decisions are made here.
