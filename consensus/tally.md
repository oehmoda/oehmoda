# Tally — plurality rule, 9 voters

Voters: 1, 2, 3, 4, 5a, 5b, 7, 9, 10 (see `CONSENSUS_PLAN.md` §1).
Rule: most votes wins, no minimum threshold. Abstentions shrink the
denominator. Compound questions are tallied per component. Rulings with ≤3
supporting plans are marked **LC** (low confidence) but stand.

Positions were extracted by one independent agent per plan (each read only its
own plan's files; within-plan precedence OA > design > one-pager). Full
structured extractions are preserved in the session record; sources cited per
position there.

---

## Q1 Equity model
| Position | Votes | Plans |
|---|---|---|
| Hybrid: earn-only founder reserve + dynamic Slicing-Pie-style contribution pool | 8 | 1, 2, 3, 5a, 5b, 7, 9, 10 |
| Fixed split via one-time structured retrospective negotiation | 1 | 4 |

**Ruling: hybrid reserve + dynamic contribution ledger (8/9).**

## Q2 Founder reserve
| Position | Votes | Plans |
|---|---|---|
| 25% total, exactly 5% per founder, equal, earned not granted ("use it or lose it") | 8 | 1, 2, 3, 5a, 5b, 7, 9, 10 |
| 70% founder block, differentiated by peer scoring | 1 | 4 |

**Ruling: 25% total / 5% each / equal / earn-only (8/9).**

## Q3 Contribution pool — components (plan-4 abstains throughout: no pool)
| Component | Winning position | Votes | Plans | Losing positions |
|---|---|---|---|---|
| Pool size | 75% | 5/8 | 1, 5a, 5b, 7, 10 | 65% (2); 62% (3); residual ≥~72% (9) |
| Time formula | unpaid hours × market rate for role performed × 2.0 | 8/8 | all pool plans | — |
| Cash multiplier | invested cash × 4.0 | 8/8 | all pool plans | — |
| Rate source | Board-adopted published Rate Card, ~50th-percentile market data for the role actually performed | 8/8 (variants merged) | all pool plans | variants: BLS-OEWS (7), Carta/Pave (1), Boston median (2, 9) |
| Quality/discretion factor | none | 6/8 | 1, 3, 5b, 7, 9, 10 | quality 0.8–1.2 (2); capped outcome bonus (5a) |
| Property/IP | approved FMV × 2.0 | 6/6 voting | 1, 3, 5a, 5b, 9, 10 | — |
| Unreimbursed expenses | × 4.0 | 3/3 voting **LC** | 3, 5b, 9 | — |
| Participation | founders, employees, advisor on identical terms | 8/8 | all pool plans | — |

**Ruling: 75% pool; hours × rate-card rate × 2 (unpaid), cash × 4, property FMV × 2, expenses × 4; no quality factor; identical terms for everyone.**

## Q4 Year-1 retroactive settlement
| Component | Winning position | Votes | Plans | Losing positions |
|---|---|---|---|---|
| Method | one-time, evidence-backed claims scored through the same formula | 8/9 | 1, 2, 3, 5a, 5b, 7, 9, 10 | blind peer scoring, no formula (4) |
| Missing-records handling | coarse default-hour conventions / bands | 3/8 **LC** | 1, 5b, 7 | graded evidence-tier discounts 100/85/50 (9, 10); committee-audited statements only (2, 3, 5a) |
| Adjudication | committee (with independent/neutral member) + publication + objection window, then FINAL | 8/9 | 1, 2, 3, 5a, 5b, 9, 10 (+7 via arbiter) | — |
| Ratification | committee decision final; no separate member ratification vote | 5/9 | 1, 2, 3, 5b, 9 | unanimous signing (4, 7); 75% vote (5a); 66⅔% + non-founder majority (10) |

**Ruling: one-time same-formula reconstruction from evidence with default-hour conventions for gaps, committee-adjudicated, published with objection window, then final and non-reopenable.**

## Q5 Founder-reserve vesting
| Component | Winning position | Votes | Plans | Losing positions |
|---|---|---|---|---|
| Length | 4 years | 7/9 | 1, 3, 4, 5b, 7, 9, 10 | 3 years (2); 36 months (5a) |
| Frequency | quarterly tranches (16 over 4 yrs) | 5/9 | 2, 3, 5b, 9, 10 | monthly (1, 4, 5a, 7) |
| Cliff | none (year one already elapsed) | 6/9 | 2, 3, 5a, 5b, 7, 10 | 12-month cliff (1, 4, 9) |
| Activity gate | tranche vests only if objective activity test met that period | 8/9 | 1, 2, 3, 5a, 5b, 7, 9, 10 | pause-then-forfeit (4) |
| Activity test | hours-based only (~≥20 hrs/wk ≈ 250 hrs/qtr) | 4/9 | 1, 3, 7, 10 | hours + quarterly objectives (2, 3*) ; higher thresholds (2: 400/qtr, 5a: 120/mo) |
| Forfeiture destination | contribution pool (all participants) | 8/9 | 1, 2, 3, 5a, 5b, 7, 9, 10 | unissued buffer (4) |
| Start date | retroactive to founding, credited only for evidenced active months | 5/9 | 1, 4, 5a, 5b, 7 | forward-only from signing (2, 9, 10) |

*plan-3 counted once for the hours-based threshold band and once against on the
objectives condition (it conditions tranches on objectives too — that component
loses 2/9 vs 5+ hours-only designs).

**Ruling: 16 quarterly tranches over 4 years, no cliff, retroactive to founding for evidenced active months; each tranche gated on an hours-based activity test (~≥20 hrs/week verified); missed tranches forfeit permanently into the contribution pool.**

## Q6 Freeze Event (plan-4 abstains: no ledger)
| Component | Winning position | Votes | Plans | Losing positions |
|---|---|---|---|---|
| Priced-financing trigger | qualified priced round ≥ $1M | 6/8 | 2, 3, 5a, 7, 9, 10 | no floor (1); ≥$2M (5b) |
| Elective freeze | Board + ~66⅔% supermajority vote | 6/8 include; 4/6 at 66⅔ | 3, 5a, 5b, 10 (66⅔); 9 (75%); 2 (unspec.) | not included (1, 7) |
| Sale / change of control | include | tie 4–4 → **tie-break rule 3** | 2, 5a, 5b, 7 | 1, 3, 9, 10 |
| Breakeven trigger | include (~2 consecutive cash-flow-positive quarters with market comp) | tie 4–4 → **re-vote 2–1 for include** | 1, 5b, 7, 9 | 2, 3, 5a, 10 |
| Fixed time backstop (~36 mo) | exclude | tie 4–4 → **re-vote 2–1 for exclude** | 1, 2, 5b, 7 | 3, 5a, 9, 10 |
| Effect | ledger freezes permanently into fixed percentages; converts pro rata to Delaware C-corp common stock | 8/8 | all pool plans | — |

Tie-break log: Sale/CoC resolved by compatibility (rule 3) — the adopted
drag-along (Q19) requires fixed percentages at a sale, so a sale must
crystallize the ledger. Breakeven and time-backstop went to a 3-judge blind
re-vote (rule 4): T1 breakeven A-B-A → include; T2 backstop B-A-B → exclude
(majority reasoning: breakeven is the natural terminus of an at-risk ledger;
an arbitrary clock can freeze while contributions are still at risk, and the
elective vote already provides the exit).

**Ruling: freeze at the earliest of (a) priced financing ≥ $1M, (b) sale/change of control, (c) two consecutive cash-flow-positive quarters with everyone at ~market compensation, or (d) Board + 66⅔% elective vote; no fixed time backstop.**

## Q7 Employee equity
| Component | Winning position | Votes | Plans | Losing positions |
|---|---|---|---|---|
| Mechanism | employees earn through the same ledger on identical terms | 8/9 | 1, 2, 3, 5a, 5b, 7, 9, 10 | separate 15% benchmark-grant pool (4) |
| Instrument | profits interests (Rev. Proc. 93-27/2001-43) | 7/9 | 1, 3, 4, 5a, 5b, 7, 10 | capital interests, PI rejected (2); phantom units default (9) |
| W-2 fallback | phantom/UAR parallel track available for workers who can't take K-1 status | 4/9 | 1, 7, 9, 10 | not offered (others silent) |
| Post-freeze option pool | ~12–15% (modal point 12.5%) | 7/9 | 1, 3, 5a, 5b, 7, 9, 10 | buffer-becomes-pool (2); unstated (4) |

**Ruling: same-ledger participation; profits interests with a phantom-unit fallback for W-2 retention; 12.5% (12–15%) option pool created at the freeze.**

## Q8 Inactive founders
| Component | Winning position | Votes | Plans |
|---|---|---|---|
| Keep everything earned (economics + votes), no confiscation | unanimous | 9/9 | all |
| Unearned reserve forfeits automatically (to pool; plan-4: to buffer) | unanimous | 9/9 | all |
| No reserved board seat / founder privileges | unanimous | 9/9 | all |
| Buyout mechanism | none — inactive founders simply stop earning and dilute | 4/9 | 2, 3, 5a, 9 | offered-never-forced FMV buyout (4, 7, 10); company call option (1, 5b) |

**Ruling: earned-is-kept, unearned auto-forfeits, no founder privileges, and no buyout mechanism — natural dilution does the work.**

## Q9 Professor / advisor
| Component | Winning position | Votes | Plans | Losing positions |
|---|---|---|---|---|
| Structure | hybrid: fixed ~1.0% advisor grant PLUS ledger participation at his benchmarked expert rate | 4/9 | 1, 3, 9, 10 | ledger-only with ~2% cap (5a, 5b, 7); fixed grant only (2, 4) |
| Fixed-grant size | 1.0% | 4/6 granting | 2, 3, 4, 9 | ~1% (1); 0.5–1.0% (10) |
| Grant vesting | monthly over 24 months | 6/6 granting | 1, 2, 3, 4, 9, 10 | — |
| Written agreement superseding the oral "decent share" promise | unanimous | 9/9 | all | — |
| Yale COI clearance + IP handling as condition | unanimous | 9/9 | all | — |
| Ledger rate | documented external expert consulting rate (~$350–500/hr band) | 7/7 addressing | 1, 3, 5a, 5b, 7, 9, 10 | — |

**Ruling: written advisor agreement (superseding the oral promise, conditioned on Yale COI/IP clearance): fixed 1.0% grant vesting monthly over 24 months, plus ledger participation at his documented expert rate. Funding: see Coherence.**

## Q10 Board
| Component | Winning position | Votes | Plans | Losing positions |
|---|---|---|---|---|
| Manager-managed LLC, Board of Managers | unanimous | 9/9 | all | — |
| Size | 3 | 8/9 | 1, 2, 4, 5a, 5b, 7, 9, 10 | 5 (3) |
| CEO ex officio seat | yes | 5/9 | 1, 2, 3, 4, 9 | all seats elected (5a, 5b, 7, 10) |
| Independent seat | yes | 4/9 | 1, 2, 3, 4 | non-founder seat instead (9, 10); none required (5a, 5b, 7) |
| Elections | non-ex-officio seats elected annually | 8/9 | 1, 2, 3, 5a, 5b, 7, 9, 10 | 2-yr independent term (4) |
| Electorate | members voting in proportion to units/ledger shares | 6/9 | 1, 5a, 5b, 7, 9, 10 | per-capita active founders (2); plurality of units (3); founder vote (4) |

**Ruling: 3-seat Board — CEO ex officio + one annually member-elected seat + one independent seat; member votes proportional to units.**

## Q11 CEO
| Component | Winning position | Votes | Plans | Losing |
|---|---|---|---|---|
| Exactly one CEO (no co-CEOs) | unanimous | 9/9 | all | — |
| Selected by the Board | 8/9 | 2, 3, 4, 5a, 5b, 7, 9, 10 | unanimous ratification (1) |
| Removable by Board majority at any time | 8/9 | 2, 3, 4, 5a, 5b, 7, 9, 10 | 75% of units (1) |
| CEO's own seat abstains / non-CEO managers decide removal | 3/9 **LC** | 2, 3, 4 | unspecified (others) |
| Removal never touches earned equity or member status | 3/3 addressing **LC** | 3, 5b, 4 | — |

**Ruling: single Board-appointed CEO, removable at any time by majority of the non-CEO Managers; office fully decoupled from equity.**

## Q12 Voting thresholds
| Component | Winning position | Votes | Plans | Losing |
|---|---|---|---|---|
| Tiered decision structure (CEO / Board / member supermajority) | unanimous | 9/9 | all | — |
| Supermajority threshold | 66⅔% of voting units | 8/9 | 2, 3, 4, 5a, 5b, 7, 9, 10 | 75% (1) |
| Unanimity requirements | none anywhere (ongoing) | 7/9 | 2, 3, 5a, 5b, 7, 9, 10 | narrow unanimity tier (1); guardrail consent (4) |
| Earned-unit protection | affected-member written consent for amendments reducing earned units | 2/9 **LC** | 7 (+1 analog) | not included (others) |
| Non-founder-majority approval for ledger-formula changes | not adopted | 2/9 against 7 | 9, 10 | — |
| Initial adoption | unanimous signature of the restated OA | 3/9 **LC** (uncontradicted) | 4, 7, 10 | — |

**Ruling: three tiers; reserved matters at Board majority + 66⅔% of units; no ongoing unanimity; adopted by unanimous signing.**

## Q13 Disputes
| Component | Winning position | Votes | Plans | Losing |
|---|---|---|---|---|
| Ladder: negotiation (10–15d) → JAMS/AAA mediation, Boston (30d) → binding single-arbitrator arbitration, Boston, MA law | 8/9 | 1, 2, 3, 5a, 5b, 7, 9, 10 | ladder ends in buyout (4) |
| Fast-track final-offer ("baseball") mechanism for ledger/valuation disputes | include | 4/9 | 2, 3, 5b, 7 | none (5a, 9, 10, 4); casting vote (1) |
| Shotgun clause | none | 6/9 | 2, 3, 4, 5a, 9, 10 | last-resort shootout (1, 5b, 7) |
| Persistent-deadlock endgame | appraised fair-value buyout (no minority discounts) | 4/9 | 2, 4, 9, 10 | company call (3); none (5a); shootout (1, 5b, 7) |

**Ruling: standard ladder ending in binding arbitration; baseball-style expert determination for ledger disputes; no shotgun; appraised fair-value buyout for persistent reserved-matter deadlock.**

## Q14 Entity path
| Component | Winning position | Votes | Plans | Losing |
|---|---|---|---|---|
| Stay a Massachusetts LLC now | unanimous | 9/9 | all | — |
| Delaware C-corp conversion pre-authorized/pre-consented in the OA | unanimous | 9/9 | all | — |
| Timing | at the Freeze Event / first priced round | 7/9 | 1, 3, 4, 5b, 7, 9, 10 | proactively early, before financing (2, 5a) |

**Ruling: MA LLC now; pre-consented Delaware C-corp conversion executed at the Freeze Event.**

## Q15 Wage Act
**Unanimous (9/9): counsel-led remediation is the urgent gating item preceding/accompanying signing** — sort every worker into lawful ≥$15/hr payroll or bona fide member status (7/9 explicit), quantify treble-damage lookback exposure, equity never substitutes for wages, wage claims not privately releasable.

## Q16 Tax execution
| Component | Winning position | Votes | Plans | Losing |
|---|---|---|---|---|
| Issue Year-1 equity NOW at provably-nominal FMV with contemporaneous valuation | 8/9 | 1*, 2, 3, 4, 5a, 5b, 9, 10 (*via counsel item) | — |
| Protective 83(b) elections within 30 days of every grant | 9/9 | all | — |
| Ongoing grants as profits interests under Rev. Proc. 93-27/2001-43 | 7/9 | 1, 3, 5a, 5b, 7, 9, 10 | rejected/capital interests (2); Year-1-as-capital (7 nuance) |
| QSBS: conversion timing starts the §1202 clock (post-OBBBA regime) | 7/9 | 1, 2, 3, 5a, 7, 9, 10 | unaddressed (4, 5b partial) |

**Ruling: settle Year 1 now at nominal FMV + valuation + 83(b)s; go-forward profits interests; convert with QSBS clock in view.**

## Q17–Q30 (added points)
| Q | Ruling | Votes | Plans for | Against |
|---|---|---|---|---|
| Q17 | No noncompetes — confidentiality, IP assignment, 12-mo non-solicit only | 4/5 | 2, 3, 9, 10 | equity-tied noncompetes (1) |
| Q18 | Present-assignment IP + confidentiality from every contributor, retroactive to inception, condition of any equity | 6/6 | 2, 3, 4, 5a, 5b, 10 | — |
| Q19 | Transfer lock: Board consent (estate exception), company-then-member ROFR, tag-along, drag-along on Board+66⅔%-approved sale | 5/5 | 2, 4, 5a, 7, 10 | — |
| Q20 | OA supersedes all prior oral/informal equity understandings (incl. professor's promise); signed acknowledgments | 5/5 | 2, 3, 4, 5a, 10 | — |
| Q21 | Standing elected Ledger/Contribution Committee separate from the Board (≥1 non-founder, founder-minority), annual member election, verification-only powers | 5/5 | 2, 3, 5b, 9, 10 | — |
| Q22 | Full ledger + cap-table statements to all members at least quarterly | 4/5 | 2, 3, 5a, 9 | monthly (7) |
| Q23 | Single class of voting units, one-unit-one-vote, no super-voting/founder class | 3/4 **LC** | 3, 5a, 10 | ledger-share-weighted voting (9) |
| Q24 | Retain default c.156C fiduciary duties (no §63 tailoring) | 2/3 **LC** | 7, 9 | tailored duties (1) |
| Q25 | Written founder role charters + quarterly objectives with CEO/Board review | 2/2 **LC** | 2, 4 | — |
| Q26 | DRI operating model (named owner per function; one-way/two-way-door test) | 2/2 **LC** | 1, 5b | — |
| Q27 | Grants papered as a written compensatory plan under Rule 701 + MA blue-sky exemption | 3/3 **LC** | 3, 5a, 10 | — |
| Q28 | Pre-agreed investor accommodations (re-vesting consent, standard first-round package) | 2/2 **LC** | 5a, 5b | — |
| Q29 | Governance articles sunset automatically at financing into NVCA-standard structures | 2/2 **LC** | 7, 9 | — |
| Q30 | No idea/vision premium — leadership/vision work priced at standard band rates | 3/3 **LC** | 1, 5b, 7 | — |

## Coherence re-tally (CONSENSUS_PLAN.md §6)

Q3 (75% pool) + Q9 (fixed 1.0% advisor grant) + Q2 (25% reserve) would sum to
101%. Joint re-tally of the full architecture combination: plans funding a
fixed advisor grant from within the pool side of the cap table (residual or
carve) — 1, 3, 9, 10 = 4 — beat pure ledger-only advisor architectures (5a,
5b, 7 = 3) and buffer architectures (2; 4). **Resolution: the 1.0% advisor
grant is carved from the 75% Contribution Pool** (pool participants share the
remaining 74% + the advisor's own ledger earnings draw from the pool as
normal). Cap table sums to 100%: 25 + 74 + 1.

## Appendix — single-plan positions (1/1, adopted by default per the plurality
rule, lowest confidence)
- MOU-first sequencing: ratify rules before computing anyone's backfill (plan-1)
- Cash-contribution recovery floor: documented cash always recoverable at face value before any forfeiture (plan-1)
- Leadership-ownership floor monitored at freeze (~30% CEO+top-2, top-up from pool) (plan-1)
- Anti-gaming penalty: knowingly inflated ledger entries forfeit 3× points; repeat = Cause (plan-5b)
- No mandatory capital calls; voluntary cash earns points, never units directly (plan-5b)
- No SAFEs/convertibles at the LLC stage (plan-9)
