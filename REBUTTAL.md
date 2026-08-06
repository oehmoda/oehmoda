# Rebuttal — The Cofounder-Only Pool Proposal

**Re:** `firas_rebuttal.md` (branch `claude/startup-governance-equity-8webj5`, 14 commits, 2026-08-04 → 08-05)
**Subject of the memo:** replace the single shared contribution pool with a cofounder-only pool of 35–40% on top of the 20% founder base, guaranteeing the cofounders 55–60% combined "by structure"
**Method:** 12 adversarial agents (5 hostile critic lenses, 4 advocates instructed to build the strongest possible case *for* the memo, 3 cross-examiners) plus 2 focused agents on the new headcount facts and citation verification. Advocates were told a defence that survives cross-examination is worth more than a maximal one; critics were required to file concessions.
**Recommendation:** do not adopt the class pool. Adopt two narrower mechanisms that follow from the memo's valid premise. Reopen one consensus ruling. Treat the departed-contributor problem as the actual emergency.

---

## 1. Bottom line

Firas has identified a real hole in the consensus design, is measuring it with the wrong instrument, and is proposing a fix that makes his own stated goal worse. The hole is real enough that it justifies amending the design. The proposed mechanism is not the amendment.

Three things are true simultaneously, and any honest reading has to hold all three:

1. **The proposal fails on its own terms.** It cannot deliver what it promises, it pays out only in the states where cofounders did not work, and measured against the benchmark it invokes it lands the cofounders *below* where the current design lands them.
2. **The underlying concern is legitimate and the consensus never addressed it.** Founder aggregate ownership was never a decision point in the consensus at all. Four of the nine source plans had already performed that calibration; the tally deleted it. That is a genuine defect in my work, not a rhetorical concession.
3. **Both documents are arguing about the wrong term.** The downsizing means roughly 25–44% of the cap table would go to people who have left the company. That is five to ten times larger than the quantity in dispute.

---

## 2. What the memo argues, stated fairly

The strongest version of the argument, which the memo makes in part and which our advocates sharpened:

Combined founder ownership is the single most investor-visible number on a cap table. Under the consensus design it is not a term of the agreement — it is an *output* of a work ledger that does not exist yet. You would discover its value during diligence, with a term sheet on the table, at which point it is unfixable: Hellmann & Wasserman observe that relative-ownership changes require the consent of everyone they disadvantage, so whoever the structure favours holds a veto. Carta's median founding team holds 56.2% after a seed round; teams entering the ladder materially below that arrive at Series B where the median company sits two rounds later. Separately, an hours-times-rate ledger prices founding risk badly: the same hour worked at month zero with no product, no team, no validation and no prospect of salary is not the same economic good as an hour worked at month fourteen, and the flat 2.0× unpaid-time multiplier prices neither the timing nor the personal liability that founders alone carry. Therefore the class split should be a deliberate decision made now, and the pools should price effort within classes while the class boundary prices risk, liability and permanence.

The memo also makes a company-first case: the ~10% penalty for badly structured splits is borne by every holder; founder ownership headroom is what keeps the next two rounds raisable; and a bounded share of a fundable company beats a larger share of an unfundable one.

---

## 3. Where the proposal fails

### 3.1 It cannot deliver a guarantee and remain earned — the two halves cancel

The memo's deliverable is "Cofounders combined | **55–60% — ensured by structure**." Two lines later: "every share in every layer is still earned, nothing is granted, and inactivity still costs you."

These are mutually exclusive. If the base stays activity-gated and the class pool is earned by hours, then when cofounders under-contribute the class total falls below 55% — no guarantee. If the class total is genuinely fixed at 55–60%, then forfeitures and unearned pool shares must be recaptured *inside the class*, which means an inactive cofounder's forfeited equity is redistributed to other cofounders rather than to everyone. That silently reverses the one ruling that was unanimous across all nine plans (Q5/Q8: forfeited value goes "permanently into the Contribution Pool for all participants — nobody's departure enriches the other founders specifically").

The memo never states which of the two it means. Both readings defeat one of its own claims.

### 3.2 It pays out only when cofounders under-perform, and the payers are the unpaid employees

Modelled on the memo's own team and calibration (4 cofounders + 5 employees, 20% base, ~79% pool, equal hours and rates, an inactive cofounder earning ~0 and forfeiting base):

| State | Consensus (shared pool) | Class pool | Transfer to cofounders |
|---|---|---|---|
| All four cofounders active | 55.1% | ~57.5% | **+2.4 pts** |
| One cofounder inactive | 46.5% | 55–60% | **+11 pts** |
| Two cofounders inactive | 35.4% | 55–60% | **+22 pts** |

The mechanism's value rises monotonically as cofounder effort falls. It is insurance against cofounder shirking, and the premium is paid by the employees who absorbed the abandoned work — roughly −2.0 and −4.2 percentage points *per employee* in the two divergence states.

This is also where the dead-equity problem appears. A shared pool dilutes an inactive cofounder against the whole team's person-years; a fenced pool dilutes them against only the remaining cofounders. Shrinking the denominator makes the non-contributor's slice *grow*: on the memo's own downside scenario the class fence pays an inactive cofounder ~12.0% of the cap table instead of ~8.3%, crossing the ≥10% dead-equity threshold documented in the plans' own research files. The proposal cures one diligence red flag by manufacturing another.

### 3.3 No individual cofounder is made better off

Per-capita, under the shared pool with the rate card applied, each surviving cofounder holds:

- 15.6% each when all four are active
- 18.0% each when one leaves
- 21.2% each when two leave

Monotonically increasing for every survivor, because forfeited reserve and the vacated pool share flow back to whoever is still working. There is no state in the space where a working cofounder's personal stake is higher under the class pool than under the shared pool. The thing being protected is a class aggregate that no individual holds.

### 3.4 The scenario table omits the rate card — the load-bearing term in the adopted formula

The memo models the pool as "hour for hour" and concludes "the employees are the majority of contributors." But the adopted formula is hours × rate *for the role actually performed*, and the memo's 44.4% pool share is 4/9 — pure headcount, with no rate term at all.

Applying the rate card from `merit-formula-and-rate-table.md` — a document on Firas's own branch — with cofounders in a senior band against mid-band employees:

| Scenario | Memo's figure | With the rate card |
|---|---|---|
| All cofounders active | ~56% | **62.4%** |
| One falters | ~48% | **53.9%** |
| Two falter | ~38% | **42.4%** |

The specific crisis the memo is built on — "~48%, below the line" — does not survive the plan's own rate card. Note also that "one cofounder falters" only produces 48% if that cofounder does roughly 12% of a full load; the table is internally consistent, but "falters" means "almost entirely stops," not "has a bad quarter."

### 3.5 The target is measured with the wrong ruler, and the proposal misses it

This was found independently by two auditors and is the cleanest disqualifying error.

The 55–60% figure is **pre-money and pre-option-pool**. Carta's 56.2% is measured **after** the option pool and after investor dilution. Run the memo's own number through the memo's own design — the 12.5% pool created at the freeze, then ~20% seed dilution — and 55–60% at freeze becomes roughly **38–42% post-seed**. Firas's own v2 draft (commit `9f77445`) performed this translation correctly for the *consensus* design ("56% at freeze → ~39–41% post-seed") and the final memo dropped it.

The deeper point: reallocating equity between two groups of working insiders does nothing whatsoever to the founders-versus-investors ratio Carta measures. The benchmark question is *who counts as the founding team*. Four people who worked a year unpaid pre-product alongside four cofounders sit in Carta's founding-team bucket, not in an option pool. Counted that way the company is already far above the median. The 12.1%-versus-40% comparison in the memo is a category error of roughly 3× in the direction that flatters the proposal — Carta's 12.1% is a *future-hire reserve*, unissued, at FMV strike, on a post-investor cap table.

Used consistently, the memo's own pair of numbers refutes it: Carta's 56.2 : 12.1 is a founder-to-employee-pool ratio of about 4.6 : 1; the memo's 55–60 : 40–45 is about 1.3 : 1, roughly 3.5× more employee-weighted than the "revealed structure" it invokes two lines earlier as decisive.

### 3.6 It hands the cofounders a permanent veto — the thing the memo's own citation warns about

Reserved matters need 66⅔% (Q12), so a blocking position requires only >33⅓%. A structurally guaranteed 55–60% class share gives four people a permanent, non-contingent veto over every reserved matter, including any future amendment to the ledger. The memo cites Hellmann & Wasserman for the proposition that whoever the structure favours holds a veto, as a reason to act now. The proposal creates exactly that condition and makes it unamendable.

### 3.7 The sequencing violates the design's own fairness device

`merit-formula-and-rate-table.md`, on Firas's own branch, prescribes signing the rules **before** running the numbers: "Agreeing on the formula before anyone sees their own result is a veil-of-ignorance fairness device — and prevents rule-negotiation aimed at flattering one's own position." The memo runs the numbers first, discovers its own class is exposed, and then bids on the rules. That is a procedural objection, not a motive accusation — but it is the specific failure mode the plans built a guard against, and the guard is in a file the memo's author has read.

### 3.8 The legal trap: the cofounders cannot assert both defences

This is the most serious finding and it is structural.

The Wage Act remediation has exactly two lawful paths for the unpaid workers: they were **employees** (owed wages, mandatory treble damages, personal liability for managing founders, no valid waiver), or they were **bona fide members/partners** (not employees, no wage claim). Every one of the nine plans identifies these as the only two cures.

Path B — the defence the cofounders would want — makes those workers *members*. Members of a Massachusetts close company are owed utmost good faith and loyalty under the *Donahue → Wilkes → Pointer → Allison* line. Capping the maximum attainable share of the minority members, by a vote of the controlling group, is the textbook freeze-out fact pattern. *Wilkes* step two requires the controlling group to show a legitimate business purpose, and step three lets the minority defeat it by showing the objective was achievable through a less harmful alternative — and the less harmful alternatives are documented in the proponent's own drafting history (the abandoned floor-and-collar).

So the class pool converts a curable wage problem into a wage problem *plus* a fiduciary claim, and forecloses the reclassification path the remediation depends on. A document stating in writing that the people you did not pay also get less equity, placed next to a year of unpaid timesheets, is the plaintiff's opening exhibit. Reducing the prospective equity of the exact cohort holding live unwaivable claims, while those claims are outstanding, also raises a §148A retaliation question.

One further documentary risk worth knowing about: commit `624c2c3` ("Narrow memo to single topic") removed 119 lines, including the v2 summary's own statement that "the ownership question this memo raises is FOURTH on the list, not first — items one through three are legal exposures that could kill a round outright," along with the acknowledged wage exposure and the six departed workers. The narrowing is a defensible editorial choice for a single-topic memo. But git preserves it, and in litigation a deleted acknowledgement reads worse than one never written. Anyone advancing this proposal should know that the record shows the author identifying the wage exposure as more urgent than the ownership question, and then removing it.

---

## 4. Citation audit

Network egress for full-page fetches was blocked in this environment (proxy denied CONNECT for every host), so verification rests on search-index content and verbatim snippets, plus internal arithmetic reconciliation. No source in the memo is fabricated; every URL resolves to a real, topically relevant document.

| Claim | Verdict | What is actually true |
|---|---|---|
| Carta: 56.2% post-seed, 36.1% post-A, 23% post-B, 12.1% seed employee pool, 45,000+ startups | **Verified** | All four figures correct. This is the memo's real contribution. Caveat: a descriptive median of VC-backed companies that closed priced rounds, not a threshold investors impose. |
| Hellmann & Wasserman: "valuation penalty on the order of 10% of company value," "paid by the company" | **Misstated** | The paper's sentence is "approximately 10% of the firm equity, 25% of the average founder stake, or $450K in NPV" — three denominations of *one* quantity (they reconcile arithmetically), and that quantity is the equity a *stronger founder forgoes by accepting an equal split*. An intra-founder redistribution, not a company-wide valuation loss. Two other plans in this repo characterise it correctly. |
| Same paper: causal ("badly structured splits **cost** real money") | **Misstated** | Authors explicitly disclaim causality, attributing the association to a reverse-causal "stakes effect" and an unobserved-heterogeneity "negotiator effect." |
| Same paper: "renegotiating a split after signing rarely succeeds" | **Wrong paper** | That finding belongs to Hellmann, Schure, Tergiman & Vo, *SEJ* 13(3) 2019, which this repo already cites correctly. In the cited paper it is motivating prose plus a modelling assumption. |
| Jensen & Meckling 1976 for "operators with large personal stakes perform better" | **Misstated** | Purely theoretical; contains no empirical test of firm performance and no startup data. Its mechanism is insider-versus-*outside*-investor. Applied properly it argues for keeping equity with the people doing the work — against the memo. |
| Fahlenbrach 2009, *Journal of Empirical Finance* | **Misattributed** | Fahlenbrach 2009 is in *JFQA* 44(2). The URL cited resolves to Adams, Almeida & Ferreira, *JEF* 16(1) — different authors. Both study large US public firms, and both treat founder-CEO *status*, not stake size. `plan-1-provenance.md` in this repo records this exact citation being flagged unverified and deliberately excluded. |
| "~70% entering seed," "~50% through the round" | **Reframed** | EquityList says 60–70% *after* seed; CRV recommends retaining ~70% after seed — a *higher* bar than the memo attributes to it. |
| "Founders owning less than investors combined" is a diligence red flag | **Vendor opinion** | Practitioner blog, no survey or empirical work — and contradicted by another of the memo's own sources: EquityList describes investors owning more than founders by Series B as the ordinary trajectory, as does Carta's own 23% figure. |
| 12.1% pool vs ~40% employee share, "roughly triple" | **Category error ~3×** | Wrong bucket (future-hire reserve vs founding-team equity), wrong instrument (unissued reserve vs consideration for delivered unpaid labour), wrong denominator (post-investor vs pre-investor), and team-total vs per-head. Correcting it inverts the conclusion. |

**Summary:** an accurate empirical core (Carta) wrapped in support that is oversold in the direction of the argument, with the two load-bearing academic citations both misused. The governance concern stands on its own merits and would be better argued without them.

---

## 5. What the memo gets right — including things it does not know it is right about

Our advocates were instructed to improve the argument, not restate it. Four findings survived cross-examination and are stronger than the memo's own version.

### 5.1 The consensus never made founder aggregate ownership a decision point at all

`CONSENSUS_PLAN.md` §2 fixed the decision-point list. There is no question anywhere in Q1–Q30 on cap-table shape at financing, founder aggregate ownership, or dead-equity cleanup. The consensus optimised internal fairness and never once checked the number investors actually look at. Worse: four of the nine source plans *had* performed that calibration, and the decomposition-and-tally method dropped it, because a question only gets tallied if it appears on the seeded list or is raised as a discrete position. **This is Firas's best point and he understates it.** He argues the number is uncontrolled; the sharper claim is that it was never a question.

### 5.2 The design is self-locking — the fix becomes unavailable exactly when it is needed

The only mechanism that can crystallise the cap table before a raise is the elective freeze, which requires Board majority **plus 66⅔% of units**. Founders at 49.7% must persuade holders of ~17 further points; at 41.8% (one founder inactive) they need ~25; at 33.1% (two inactive) they need ~34. In every state where the founders would want to freeze, they lack the votes to do it. The 2–1 blind re-vote that deleted the 36-month time backstop relied explicitly on the reasoning that "the elective vote already provides the exit" — and the elective vote is structurally unavailable in precisely those states. **That tie-break was decided on a premise that does not hold.** It should be revisited on the merits.

### 5.3 The flat 2.0× multiplier genuinely misprices founding risk

The design's own documents call the 2.0× a risk premium, then hold it constant across the one dimension in which risk actually varies. The multiplier already varies by asset form (cash 4.0× vs time 2.0×) and by at-risk-or-not (paid time 0×) — but not by *when*. A flat nominal premium is steeply regressive in risk-adjusted terms: annualised to a month-36 freeze, 2.0× is ~26%/yr for an hour worked at month 0 and ~300% for an hour at month 30. The decisive internal counterexample: two contributors, identical hours, identical role, one working months 0–6 when there was no product and no company, the other months 30–36 on a functioning team with a term sheet in view, earn identical points.

**But the correction is worth 1–5 percentage points to the founding cohort, not 35–40%.** And the 25% reserve the memo dismisses as "only a 20% base" is already a larger founding-risk premium than proper repricing would award. The premise is sound; the requested remedy is off by an order of magnitude.

### 5.4 The liability asymmetry is real, large, and priced at exactly zero

M.G.L. c.149 §148 deems officers and agents having management responsibility to be the employer *personally*; §150 makes treble damages and fees mandatory. Managing founders carry uninsurable personal exposure that employees do not — and here the counterparties holding those claims are the same people sharing the pool. The ledger prices this at zero. That is a defensible basis for a narrow premium; it is not a basis for a class guarantee, and note that it argues for differentiating *managing* founders from passive ones, not founders from employees.

### 5.5 One unmodelled risk larger than the dispute: the cash × 4.0 multiplier

Neither document models this. At a $64/hr contributor rate, $100k of member cash buys ~1.5 engineer-FTE-years of points; $500k buys ~7.5, or roughly 11.5% of a 15-person-year ledger. It is an uncapped, unpriced, rolling equity issuance for cash, available to whichever member has money. It is the largest single swing factor on the cap table and it should be capped or priced before signing.

---

## 6. Errors in the consensus that this exercise exposed

Recorded because the consensus is mine and these are defects in it, not debating points.

1. **Founder aggregate ownership was never a decision point** (§5.1). The most consequential omission.
2. **A tie was declared without applying the mandatory tie-break.** `tally.md` Q4 records "coarse default-hour conventions 3/8 **LC**" against "graded evidence-tier discounts (9, 10)" and "committee-audited statements only (2, 3, 5a)" — that is 3–3–2, a tie for first place. `CONSENSUS_PLAN.md` §5 makes tie-breaking mandatory and deterministic. It was not invoked. The Year-1 missing-records ruling is therefore unresolved, not decided.
3. **The Q8 no-buyout ruling is a vote-splitting artifact.** "No buyout mechanism" won with 4 against "offered-never-forced FMV buyout" (3) and "company call option" (2). Five of nine plans wanted *some* mechanism to retire a departed founder's units; the plurality rule awarded the ruling to none of them. This is the one ruling the new facts make actively harmful — see §7.
4. **The 8/9 and 8/8 rulings are not eight independent confirmations.** Slicing Pie / Moyer citation counts per plan: plan-1 (33), plan-2 (21), plan-3 (43), plan-5a (55), plan-5b (31), plan-7 (33), plan-9 (46), plan-10 (12) — and plan-4, the lone dissenter, **zero**. The eight plans that voted together for "identical terms," "hours × rate × 2.0" and "cash × 4.0" were reading the same practitioner source. That is one position counted eight times, correlated error rather than convergent evidence. The plurality method cannot detect this, and any headline vote count in `tally.md` should be read with it in mind.
5. **The 36-month-backstop tie-break rests on a false premise** (§5.2).

None of these vindicate the class pool. Several of them strengthen the case for amending the design in other ways.

---

## 7. The problem both documents are ignoring

The company has downsized from ~10 employees to 4. Roughly six employees, and possibly one founder, have departed — after working unpaid.

Under the consensus as written, pool points are **unconditional once earned** (§1), and the Year-1 retroactive settlement covers "every participant" who submits an evidence-backed statement. The only forfeiture rules attach to the *founder reserve*. There is no textual basis for excluding departed contributors; excluding them would be a new decision, not an application of the design. Searching all nine plans for treatment of departed non-founder contributors returns essentially nothing — the corpus's leaver analysis is entirely about inactive founders who *remain* members. The consensus inherited that blind spot.

Modelled at one unpaid person-year each, if the ledger froze at time T:

| Freeze at | Departed (7 people) | Each departed employee | 4 active founders | 4 active employees |
|---|---|---|---|---|
| T = 1 yr (now) | **44.1%** | 6.1% | 30.2% | 24.4% |
| T = 2 yrs | **27.7%** | 3.8% | 41.1% | 30.0% |
| T = 3 yrs | **19.8%** | 2.6% | 47.5% | 31.7% |
| T = 4 yrs | 15.2% | 2.0% | 51.9% | 31.9% |

Sensitivity at T=2: 13.1% low, ~24.9% central, 26.3% if the departed were engineers on above-average bands. The aggregate does not fall below the 10–15% dead-equity red-flag band until roughly year seven, and the consensus deliberately deleted the time backstop and freezes at the *earliest* trigger — most likely T ≈ 1.5–3, exactly where the number is 20–28%. On the stricter practitioner test in the plans' own references (any single uninvolved holder above 5%), each departed employee sits individually over the line at settlement, and there are six of them.

**This corrects a figure I gave earlier.** The claim that downsizing moved founder ownership up ~10 points to ~60% holds only if the departed are removed from the ledger denominator — which the design forbids. Counted correctly, the four active founders are nearer **30% today**, not 60%.

Three consequences worth more than the entire class-pool dispute:

- **The drag-along and conversion covenant bind only OA signatories.** A departed holder who never signs cannot be dragged into a sale and has not pre-consented to the Delaware conversion. A single unsigned 3–5% holder can hold up a change of control. That is a hard veto, not a diligence frown.
- **Departed workers' wage claims are crystallised and non-curable.** Under *Reuter v. City of Methuen* (489 Mass. 465, 2022) all accrued wages were due on the day of discharge and late payment does not cure. Estimated at $15/hr minimum with §151 §1A overtime, trebled: **$540k–945k for the six departed alone**, mandatory fees on top, personally guaranteed, 3-year limitations running to ~2029. If anyone was promised a salary rate above minimum wage, *Stanton* treats deferred salary as wages at the promised rate and the number moves 3–8×. These are also the people most likely to sue: no job, no relationship, no equity upside to protect, no retaliation exposure.
- **The consensus overstates one legal point in a way that removes the only available cure.** §6/Q15 says wage claims are "not privately releasable." Too absolute. *Prospective* waiver and equity-for-wages are void §148 special contracts (*Stanton*) — but settlement of an already-existing bona fide wage dispute is enforceable if the release is plainly worded and **specifically refers to the Wage Act rights being waived** (*Crocker v. Townsend Oil Co.*, 464 Mass. 1 (2012); recited from memory, counsel must verify). So the departed cohort *can* be closed out — with cash, individual counsel-drafted Wage-Act-specific releases and separate consideration. **Not with equity.**

And the sharpest drafting hazard in the whole file: §9 conditions equity on IP assignments "as a condition of receiving any equity," while §1 settles Year 1 for everyone. Presented to an unpaid ex-worker that is functionally *"sign this to get your shares."* If the package bundles units with anything release-shaped, or any recital implies the equity accounts for the unpaid year, you have created a void special contract **and** manufactured evidence of intent.

**Ranked by leverage on founder ownership:** resolving departed contributors, **~20–30 points**; hours actually logged, several points; rate-card bands for the roles founders perform, a few points; reserve size, 5 points. A founder genuinely worried about ownership should be spending this energy on the first item, which is worth three to six times the fourth.

---

## 8. Recommendation

**Reject** the cofounder-only pool: it cannot deliver its guarantee while remaining earned, it pays out only when cofounders under-contribute, it makes no individual cofounder better off, it lands below the benchmark it invokes once translated post-money, it creates a permanent unamendable veto, and it forecloses the bona-fide-member path the wage remediation depends on while writing the plaintiff's opening exhibit.

**Adopt instead**, both of which follow from the memo's valid premise and raise the founder number *through* contribution rather than around it:

1. **A time-decaying risk multiplier inside the single pool.** Higher for pre-formation and Year-1 hours (e.g. 3.5–4×), decaying to 2.0× by the freeze. Prices founding risk on the axis where risk actually varies, awards nothing to non-contributors, needs no class boundary, and survives fiduciary scrutiny because it applies to anyone who was there early — including the four employees who were.
2. **An executive band on the rate card** for the leadership, strategy and fundraising work founders actually perform. Q30's no-idea-premium ruling (3/3, thin) currently prices that work at standard engineering bands. Market comp data has an executive band; using it is not an idea premium. Narrow, defensible, and it does not touch the pool structure.

**Reopen one ruling:** Q8's "no buyout mechanism" (4/9, and a vote-splitting artifact per §6.3). You need a lawful way to retire a departed founder's units and to buy the departed founder's consent to the restatement. That ruling deleted the tool, and five of nine plans wanted one.

**Also fix, on the evidence above:** cap or price the cash × 4.0 multiplier (§5.5); re-decide the Q4 missing-records tie under the actual tie-break rule (§6.2); revisit the time-backstop tie-break now that its premise is known false (§5.2); scope OA adoption to persons who are members immediately before adoption, so departed contributors cannot hostage the founding document; make every unit issuance conditional on signature so unsigned holders are either bound or unissued; decouple freeze trigger (c) from the market-comp remediation, since doing the legally mandatory thing currently pushes you toward a trigger that crystallises the departed's 25–44%; and restate the Year-1 finality claim honestly — final among signatories, on equity questions only, never against a non-signatory's wage claim.

**Sequence, because this part is not optional:** the four current employees go onto lawful ≥$15/hr payroll or completed counsel-validated member restructuring *this week* — that violation accrues daily and the liability is personal. Departed-worker settlement is a separate workstream on a different clock; making it a gate on signing freezes the company indefinitely, so gate it on financing and conversion instead, with the exposure quantified and reserved before anyone signs anything.

---

## 9. Plain-language summary

The company is a pizza with 100 slices. The agreed plan says you get slices for work you actually do, recorded in a notebook, same rules for founders and employees.

Firas wants to stop hoping the notebook gives the four founders enough slices, and instead promise them 55–60 slices up front. His worry: if founders end up holding less than half, investors will think the founders aren't really in charge.

Why it doesn't work. If all four founders work hard, the notebook already gives them about 60 slices — so the promise changes nothing. The promise only *does* something when a founder stopped working, and then it says "you didn't do the work, here are the slices anyway." That is the exact thing investors penalise, and it is paid for by the employees who covered the abandoned work. His scary numbers also left out one of the notebook's rules — that harder, more senior work counts for more per hour — and putting that rule back turns his "48%, below the line" into about 54%. And the 56% target he is aiming at is measured *after* investors take their slices, while his 55–60% is measured before; once investors take their share his proposal lands around 40%, so he would miss his own target.

What he's right about. Nobody ever checked what the founders' total would be — that question was never asked. And an hour of work back when there was no product, no money and no promise of pay really was worth more than the same hour today; the plan treats them as equal and shouldn't. Both are worth fixing. Neither needs a separate founder pool.

The thing nobody was looking at. Six workers left. Under the plan as written they keep every slice they earned — possibly 25 to 44 slices held by people who aren't here. That is the real problem, it is five to ten times bigger than this argument, and those same six people are owed roughly half a million to a million dollars in unpaid wages that must be settled in cash, not equity.

---

## 10. Method, and what is not settled

**Method.** 12-agent adversarial workflow: five hostile critic lenses (citations, arithmetic, internal consistency, Massachusetts law, incentives), four advocates instructed to build the strongest case for the memo and to attack the consensus, three cross-examiners; plus two focused agents on the downsizing consequences and citation verification. Critics were required to file concessions; advocates were told a defence that survives cross-examination beats a maximal one.

**Limitations, stated because they bear on how much weight this carries.**

- **Citation verification was degraded.** Full-page fetches were blocked for every host by the environment's proxy. Findings rest on search-index content, verbatim snippets and internal arithmetic reconciliation. The Hellmann & Wasserman abstract sentence is quoted verbatim from index content and reconciles arithmetically, but no primary source was opened directly.
- **The team composition is contested and load-bearing.** The nine plans were briefed on 5 founders + ~10 employees. The memo asserts 4 cofounders + 5 employees, revised mid-drafting (commits `43aec25`, `8f81cf3`), and the same commit that reduced the count also sharpened the framing from "could land above 60% or below 50%, nobody can compute it" to "the best case barely reaches the median." The founders have since stated the current team is 4 founders + 4 employees. Base case at comparable hours by configuration: 49.7% (5+10), 55.6% (4+5), 59.5% (4+4), 67.4% (4+4 with the rate card).
- **The departed-contributor model is a model.** Everything in §7 is sensitive to the departed workers' actual tenure, hours and rate bands, and above all to whether anyone was promised a salary rate above minimum wage. The range spans 13%–26% of the cap table and $540k–945k+ trebled for that reason.
- **Open factual questions that change conclusions:** was the departed founder an original member, and did they have management responsibility (this determines both a signature dependency and personal wage liability); were the departures voluntary or terminations (*Reuter* and §148A turn on it); *Crocker*'s exact standard, which is load-bearing for the whole settlement strategy and is recited from memory; and whether the Attorney General's Fair Labor Division will respect a private settlement program.
- **Not legal advice.** Every authority cited here needs counsel verification against primary sources before anyone relies on it.

**Falsifiable claims.** The arithmetic in §3.2–3.5 and §7 is reproducible from the formula in `consensus/CONSENSUS.md` §1 and the rate card in `merit-formula-and-rate-table.md`; disagree by changing a stated assumption, not by changing the conclusion. The citation findings in §4 are checkable against primary sources by anyone with unrestricted network access, and should be re-run.
