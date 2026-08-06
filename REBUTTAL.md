# Rebuttal — The Cofounder-Only Pool Proposal

**Re:** `firas_rebuttal.md` (branch `claude/startup-governance-equity-8webj5`, 14 commits, 2026-08-04 → 08-05)
**Proposal under review:** replace the single shared contribution pool with a cofounder-only pool of 35–40% on top of the 20% founder base, guaranteeing the cofounders 55–60% combined "by structure"
**Method:** 12-agent adversarial workflow — 5 hostile critic lenses, 4 advocates instructed to build the strongest possible case *for* the memo and to attack the consensus, then 3 cross-examiners whose job was to attack **both** cases. Critics were required to file concessions; advocates were told a defence that survives cross-examination beats a maximal one. Plus 2 focused agents on the revised headcount and citation verification.
**Recommendation:** reject the class pool; adopt a two-sided freeze-time band on the *active*-founder class plus a quarterly pro-forma cap table; reopen two consensus rulings; treat the departed-contributor problem as the actual emergency.

**Epistemic note.** Every finding below carries the cross-examination verdict it earned. Roughly a third of the critique did not survive, including two findings that appeared in the first version of this document and one of the two mechanisms it recommended. Findings marked **[refuted]** are recorded rather than deleted so that nobody re-derives them.

---

## 1. Bottom line

Firas has identified a real and serious hole in the consensus design. His mechanism is the wrong instrument for it, for reasons that are mostly *not* the ones a first reading suggests. And both documents are arguing about a smaller quantity than the one that should be occupying everyone's attention.

1. **The diagnosis survives and is the strongest point in the entire dossier — on either side.** Founder aggregate ownership was never a decision point in the consensus. Its admissible range is roughly **37% to 63%** pre-money, it is walked downward monotonically by ordinary hiring, and it is governed by no tally row — guarded only by a single-plan appendix provision. That is a 20+ point range on the line investors read first.
2. **The mechanism fails, decisively, on grounds that hold regardless of contested facts.** It is insurance against cofounder shirking whose premium is paid by the unpaid employees; it is a two-sided band that *caps* the cofounders in the state the memo itself calls best; its cap table does not close; and it cannot implement the pricing function its own risk argument describes.
3. **Both documents are ignoring a bigger term.** The downsizing means roughly 25–44% of the cap table would go to people who have left, carrying crystallised non-curable wage claims. That is worth five to ten times the quantity in dispute.

---

## 2. The proposal, stated as strongly as it can be

Combined founder ownership is the most-read line in seed diligence, and under the consensus it is an *output* of a ledger that does not exist yet, discovered during diligence with a term sheet on the table — at which point it is unfixable, because relative-ownership changes need the consent of everyone they disadvantage. Carta's median founding team holds 56.2% after a seed round. Separately, an hours-times-rate ledger misprices founding risk: the same hour worked at month zero with no product, no team, no validation and no prospect of salary is not the same economic good as an hour worked at month fourteen, and the flat 2.0× multiplier prices neither timing nor the personal liability founders carry. So the class split should be decided deliberately, now, with pools pricing effort within classes and the class boundary pricing risk, liability and permanence.

Two things Firas deserves explicit credit for. He labels his weakest source "(practitioner source)" in his own bibliography — more disclosure than most advocacy memos offer. And his published scenario figures (56 / 48 / 38) round **up** by 0.4, 1.1 and 2.3 points against the underlying arithmetic (55.6 / 46.9 / 35.7), i.e. they make the design he is criticising look *better* than it computes. An advocate massaging numbers rounds the other way.

---

## 3. Why the mechanism fails

### 3.1 "This costs nothing and changes nothing" is false — the band is a ceiling too **[survives — strongest finding in the critique]**

The memo's closing claim is that "if the ledger would have carried us above 50% anyway, this costs nothing and changes nothing… There is no scenario where deciding our own number, now, on the evidence, leaves the company worse off."

A fixed class pool is a **two-sided band**. Crossover is at exactly **1.25×** relative cofounder hours: below it the guarantee helps, above it the cap binds.

| Relative cofounder effort | Shared pool | Class pool (capped) | Cost to cofounders |
|---|---|---|---|
| 1.25× | 60.00% | 60.00% | 0 |
| 1.5× | 63.64% | 60.00% | **−3.6 pts** |
| 2.0× | 69.23% | 60.00% | **−9.2 pts** |

The memo's own scenario table opens with "All four cofounders outwork everyone | ~60%+" — the truncated case. **The document prints the scenario it then declares impossible.** Commit `9f77445` contained the two-sided framing explicitly ("anything above [60%]…"); the final draft deleted it. This finding rests on nothing contested: no rate card, no headcount, no legal doctrine.

### 3.2 It is insurance against cofounder shirking, and the employees pay the premium **[survives — strongest substantive objection]**

The mechanism's payoff rises monotonically as cofounder effort falls: roughly **+2.4 points** at comparable hours, **+8 points** when one cofounder stops, **+14 to +22** when two stop. A payoff schedule that increases as own-side contribution decreases is the formal signature of insurance against own-side shirking — and line 68 concedes the operative range in the memo's own words.

The payers are identified by construction: the states where the guarantee binds are exactly the states where employees generated more of the rate-weighted contribution and absorbed the abandoned work. Employee class transfer: **−1.4 / −10.0 / −21.1 points** across the three states. A fixed class total makes cofounder underperformance structurally uncompensable to the people covering it, where the shared pool reprices it automatically.

This is in tension with the single most-supported equity ruling in the corpus — Q8 at 9/9, Q5 forfeiture destination at 8/9: forfeited value goes "permanently into the Contribution Pool for all participants — nobody's departure enriches the other founders specifically."

### 3.3 A partition cannot implement the pricing function the risk argument describes **[survives — "unanswerable as stated"]**

The risk premise identifies a *pricing function*: price per hour decreasing in contribution date, increasing in liability borne. The proposal implements a *two-bucket partition* using founder status as proxy. It fails in all three directions:

- **Inside the class:** a month-10 cofounder is priced identically to a month-0 cofounder. This is live here — commit `43aec25` describes "4 cofounders + equal partner," i.e. intra-class staggering.
- **Outside the class:** the month-2 unpaid employee who bore the same pre-validation risk gets nothing for it.
- **Going forward:** a cofounder hour at month 30, after validation, still earns the class premium.

And on liability specifically, *Segal v. Genitrix, LLC*, 478 Mass. 551 (2017) holds that c.149 §148 individual liability reaches only those who assume and perform president/treasurer management functions. **A non-managing cofounder carries no more personal exposure than an employee** — yet the class pool pays that person the same liability premium as the CEO who signs payroll. The premise argues for distinguishing *managing* founders, not founders as a class.

### 3.4 The 35–40% parameter is not derived from anything **[survives]**

The number enters at line 61 as a given. No derivation appears anywhere in the memo. Diagnostically: move the founder-attrition hazard rate, the employee start month, or the liability estimate across any plausible range and the ask does not move — a parameter insensitive to every input its stated justification contains is not justified by that justification. The commit history corroborates it: `9328212` is titled "Reframe memo company-first: **55-65% band**, both-tails risk analysis, deliberate calibration." The band was set first and the rationale fitted afterwards. Note also that 20% + 35–40% = 55–60% brackets the Carta median of 56.2% — which is where the number actually comes from.

### 3.5 The cap table does not close **[survives — cleanest structural defect]**

Pure document arithmetic. The memo's table consumes 100% at both endpoints (20 + 40 + 40, and 20 + 35 + 45) with **no advisor line at all**. The words "professor," "advisor" and "freeze" appear **zero times** in the final memo. The consensus carves the professor's fixed 1.0% from the pool and closes at 25 + 74 + 1 = 100. So the proposal either omits the advisor or silently displaces him, and the 55–60% band is underdetermined by ±5 points depending on which.

The same root produces a second defect: line 64 says the residual serves "employees **and future hires**," which conflicts with the adopted design (no unissued buffer at the LLC stage; the 12.5% option pool is created at the freeze and dilutes *everyone*, cofounders included, 7/9). Either employees fund future hires twice, or a 7/9 provision has been displaced without saying so. Functionally, "ensured by structure" operates as an anti-dilution right against every subsequent issuance.

### 3.6 The target is measured with the wrong ruler **[survives — but triple-counted, and discount accordingly]**

The 55–60% is pre-money; Carta's 56.2% is post-money fully diluted. On a common basis, 55–60% at freeze becomes **~39.0–42.5%** post-seed if the 12.5% pool is carved pre-money, or **~44.6–48.6%** if the pool sits inside the freeze percentages. Reaching 56.2% post-seed requires ~69.4% or ~79.3% at freeze. So line 64's "exactly where funded companies stand" is false, and the ladder table's column header "Starting position post-seed" populated with freeze-basis figures is a genuine basis error.

Sharper still: the ladder's "~40% (our weak scenarios)" row is arithmetically the same figure that draft `9f77445` labelled "**~39–41% post-seed** — our best case, current plan." The same number was relabelled from best case to weak case between drafts.

**Discount this criticism, though.** The consensus design fails the same test — 49.7% pre-money becomes ~33.5% post-seed. The basis error is real but it is an error in the *argument*, not a reason the proposal is worse than the status quo on this metric.

### 3.7 Related-class incentives, all premise-light **[survives]**

- **Never admit another cofounder.** Under a fixed class pool, 40/4 = 10% each becomes 40/5 = 8% each: admitting a member is pure dilution to incumbents. Under the shared pool a strong new contributor dilutes all participants and cofounders bear only their points-share. This matters concretely here, because a fifth person has been promised equal partnership — the structure converts that promise into a direct cost to the four incumbents.
- **The rate card becomes economically irrelevant across the boundary.** Once class totals are fixed, only intra-class ratios move money, so no amount of employee effort or rate differential can move value across the class line. This holds for *any* rate card, which is why it stands where the quantitative rate-card claims collapse (§3.10). The memo's line 46 is precise about this without flagging it: an excellent employee "out-earns every *other employee*" — never a cofounder.
- **Senior recruits land entirely on the employees' balance sheet.** Under the shared pool, a high-rate outside participant (the professor, future senior hires) dilutes cofounders pro rata, so whoever holds hiring authority bears part of the cost. Under a fixed class total they bear none — which predicts over-recruiting of high-rate outsiders funded entirely by the employee class.

### 3.8 Firas's own branch contains the correct version of his central citation **[survives — strongest citation finding]**

The memo says Hellmann & Wasserman deliver "a valuation penalty on the order of 10% of company value at first financing," "paid by the *company*… every holder, employee and founder alike, absorbs it," making a clean structure "free money at the round."

Both halves are wrong, and the correct version is in the same git tree (`6ca5e9c`):

> `research/academic-literature.md`: "The authors estimate stronger founders who accept an equal split leave ~10% of firm equity / ~25% of the average founder stake / ~$450K NPV **'on the table.'**"
>
> Same file: "Important caveat the authors themselves stress: the fundraising penalty appears to be **selection, not causation**."
>
> `references.md`: "the fundraising penalty for equal splits is selection, not causation — the authors say so themselves."

So the ~10% is an **intra-team transfer from stronger to weaker cofounders**, not company value destroyed and absorbed pro rata — the "25% of the average founder stake" denomination is only coherent on that reading. And the causal claim is the one the authors explicitly disclaim. The "free money at the round" pillar of the "What the company gains" section does not survive.

Additionally: "renegotiating a split after signing rarely succeeds" is a model assumption in that paper, not an empirical finding — the empirical version belongs to Hellmann, Schure, Tergiman & Vo, *SEJ* 13(3) 2019, which this repo cites correctly elsewhere.

### 3.9 Remaining citation findings

| Claim | Verdict | What is true |
|---|---|---|
| Carta 56.2% / 36.1% / 23% / 12.1%, 45,000+ startups | **Verified** | All four correct. The memo's real contribution. A descriptive median of companies that closed priced rounds, not a threshold investors impose. |
| Jensen & Meckling 1976 for "operators with large personal stakes perform better" | **Misstated** | Pure theory, no sample — "the evidence says" misdescribes the genre. Under either design total insider ownership is 100% pre-round, so its owner-manager-vs-outside-claimholder mechanism is silent on how insiders divide it. Its own logic (residual claims should sit with those bearing the effort) supports a contribution ledger. |
| Fahlenbrach 2009, *Journal of Empirical Finance* | **Misattributed** | Fahlenbrach 2009 is *JFQA* 44(2). The cited RePEc handle is Adams, Almeida & Ferreira, *JEF* 16(1) — different authors. Both study large public firms and both treat founder-CEO *status*, not stake size. `plan-1-provenance.md`, same tree, records this exact citation flagged unverified and "deliberately **kept out of** references.md." A quarantined citation was promoted to load-bearing with the wrong journal attached. |
| "~40–45% vs 12.1% median pool, roughly triple" | **Category error ~3×** | Wrong denominator (pre-investor vs post-seed), wrong instrument (entire residual vs unissued reserve), and decisively wrong reference class — a 12.1% option pool exists at companies that *met payroll*. The genuinely comparable object in the consensus design is the 12.5% freeze-time pool. On the memo's own logic (its rate-card annex calls unpaid work "investing $82.50 of forgone salary per hour, the same way a cash investor invests dollars") the unpaid workers are co-investors of forgone wages, not option holders. |
| Carta's 56.2 : 12.1 as "the market's revealed structure" | **Refutes the proposal** | That pair is a 4.6 : 1 founder-to-employee ratio. The proposal is 1.3 : 1 — roughly 3.5× more employee-weighted than the structure invoked two lines earlier as decisive. A consistent reading calibrates nearer 80/20. |
| Equity Matrix as authority for a diligence red flag | **Cited selectively** | The same page's red-flag list also condemns "complex structures with multiple share classes" and "unclear ownership" — the memo quotes one clause while the rest cuts the other way, and a two-class pool with a guaranteed floor sits squarely inside the flag it omits. |
| "Investors won't underwrite a ledger-derived cap table" (advocates' sharpened version) | **Refuted** | The same practitioner page says teams "freeze at least 2–4 weeks before closing," that dynamic-equity-then-freeze-then-raise *is* the standard workflow, and that "investors actually prefer this to a cap table built on day-one guesses, because the numbers reflect what actually happened." |

### 3.10 Findings that did **not** survive — recorded so nobody re-derives them

- **"The guarantee cancels itself"** (a class share cannot be both ensured and earned) — **largely refuted.** There is a third reading the critics missed and it reproduces the memo exactly: a *fixed-size* class pool allocated pro rata among cofounders by relative points, with forfeited base flowing **out** to the shared side. That yields precisely 60.0% with four active and 55.0% with one inactive. The memo is coherent; it just never says which reading it means.
- **"The rate card already delivers 62%, so the guarantee is a ceiling"** — **refuted.** No rates are adopted anywhere in the consensus; the rate schedule is a placeholder annex authored by an agent on 1 August, not by Firas. Critically, it assigns bands "per role performed, **not per title held**," and employees are eligible for senior-engineer and staff bands exactly as founders are — the annex's own worked example has employees in high bands. Assigning founders the top buckets and employees the bottom is not what the design says. The narrow observation survives: the memo omits the rate term entirely ("Rate Card" appears zero times), so its table is pure headcount. But no quantitative conclusion follows.
- **"No individual cofounder is ever better off"** — **weakened.** The base-case cost (−0.59 points per cofounder) is right, but the tail payoff figures assumed in-class capture. Under the reading that actually reproduces the memo: one-gone is +0.36 (essentially neutral), two-gone +3.79. The true shape is a small certain cost for a modest tail payoff — still a bad trade, but not the sign-flip originally claimed.
- **"The cofounders cannot assert both legal defences"** (Wage Act bona-fide-member defence vs *Wilkes* fiduciary duty) — **refuted as fatal; survives as a flag for counsel.** The remediation sorts workers **per person**, not by company-wide election, so there is no pincer. Status under c.149 §148B turns on control, service outside the usual course and independent business — not on equity class or percentage. And unanimity cuts the other way: because adoption requires every member's signature, each employee-member holds an adoption veto, which is an *answer* to the freeze-out theory rather than an aggravating fact.
- **§148A retaliation exposure** — **refuted.** The statute requires an employee action to seek wage rights; no complaint, claim or protected action appears anywhere in this record, so the predicate is absent.
- **"The memo violates the MOU-first veil-of-ignorance rule"** — **weakened to rhetoric.** That provision says sign the *rules* before running the *numbers*, to prevent rule-negotiation flattering one's own outcome. Firas is proposing a rule before the backfill, which is what the provision asks. His table is a class-level projection from headcount; he cannot know his own share relative to the other three cofounders from it.
- **"The deleted Wage Act section is a litigation exhibit"** — **weakened to a governance point.** *Wilkes* attaches to conduct toward a minority, not to superseded drafts of an unadopted proposal by one member; pre-signature iteration is ordinary drafting. The omission itself is still worth raising: "Wage," "treble," "forfeit" and "freeze" return zero hits in the final memo, and commit `624c2c3` deleted both the full wage-exposure workstream and the author's own sentence that "the ownership question this memo raises is **fourth** on the list." That is a credibility and prioritisation point to put to him directly — not evidence of anything.
- **"The proposal creates a permanent unamendable veto"** — **weakened.** Directionally right (a guaranteed 55–60% is an unconditional blocking position against a 66⅔% threshold, where the consensus version is contingent on continuing to work), but the single-class ruling it collides with is 3/4 and flagged low-confidence — one of the thinnest in the tally. He is attacking a weak plank, not settled consensus.

---

## 4. What Firas is right about — including things he does not claim

### 4.1 The diagnosis, stated narrowly, is the strongest point on either side **[survives]**

`CONSENSUS_PLAN.md` §2 fixes the decision list at Q1–Q30, and **not one question covers cap-table shape at financing or founder aggregate ownership.** So `tally.md` has zero rows on the number investors read first. Independent modelling puts the admissible range at roughly **37% to 63%** pre-money, driven mostly by two variables nobody has fixed — headcount and paid-versus-unpaid status. The only guard in the entire document is a single-plan (1/1) appendix provision.

### 4.2 Hiring drift walks the number down monotonically, with no floor **[survives]**

The consensus explicitly has "no unissued buffer at the LLC stage," so every hire dilutes the founder class irreversibly — and the company *must* hire to reach a $1M round:

| Team | Founder total at comparable hours |
|---|---|
| 5F / 10E (the briefed team) | 49.7% |
| 5F / 15E | 43.5% |
| 5F / 20E | 39.8% |
| 5F / 25E | 37.3% |

There is no date-certain terminus and no cap on participants. This is the surviving half of the time-backstop objection, and it is independent of any claim about who controls the freeze vote.

### 4.3 The 2.0× multiplier genuinely misprices founding risk **[survives — verified stronger than argued]**

The design's own annex defines the 2.0× as a risk premium — "investing $82.50 of forgone salary per hour (**doubled for risk**), the same way a cash investor invests dollars," and "someone paid at or above market accrues zero time slices — **nothing at risk**." So the document varies its multiplier along two risk axes (asset form; at-risk-or-not) and along **zero time axes**, while invoking a cash-investor analogy from a market that prices stage risk steeply. Two contributors with identical hours and identical roles, one working months 0–6 before there was a product and one months 30–36 with a term sheet in view, earn identical points.

Correctly repriced, this is worth **+0.9 to +5.2 points** to the founding cohort — not 35–40%. And the 25% reserve the memo dismisses as "only a 20% base" is already a larger founding-risk premium than proper repricing would award.

### 4.4 His own baseline contradicts his own argument, in his favour **[survives]**

The "~56% at comparable hours" figure assumes employees are identical to cofounders in start date, hours and rate — the exact opposite of the risk argument the memo makes two sections later. Take his stage premise seriously and the *single* pool moves toward him: **51.4%** if employees started at month 2, **61.9%** if month 12. A memo cannot claim early hours are economically special and then price its own baseline as though they were not.

### 4.5 One unmodelled risk larger than the dispute: cash × 4.0 **[survives]**

Neither document models this. At a $64/hr rate with the 2.0× multiplier, $100k of member cash buys ~1.5 engineer-FTE-years of points; $500k buys ~11.5% of a fifteen-person four-year pool. It is an uncapped, unpriced, rolling equity issuance available to whichever member has money — and the design's own gating item (paying wages) creates the cash need. The largest single determinant of the cap table is currently who happens to have savings.

### 4.6 Doing the legally mandatory thing raises the founder number anyway **[survives, magnitude corrected]**

Wage Act remediation itself moves the founder total, because paid time earns no risk multiplier. At the $15/hr floor the consensus actually specifies, against an $82.50 benchmark: 49.7% → **53.1%, i.e. +3.4 points**. (An +8.3-point version circulated in the dossier; it requires a $30/hr remediation wage, double the stated floor.) Neither document had modelled this.

---

## 5. Defects in the consensus that this exercise exposed

The consensus is mine. These are defects in it.

1. **Founder aggregate ownership was never a decision point** (§4.1). Plurality can only count answers to questions someone thought to ask. The one plan that converted the concern into a *mechanism* — plan-1's leadership-ownership floor — survived only as a 1/1 appendix line. **Verified; genuine method defect.**
2. **A tie was declared without applying the mandatory tie-break.** `tally.md` Q4 missing-records handling is 3 (default-hours: plans 1, 5b, 7) / 3 (audited statements only: 2, 3, 5a) / 2 (graded evidence discounts: 9, 10) — a genuine tie for first place. `CONSENSUS_PLAN.md` §5 makes tie-breaking mandatory and deterministic; the tie-break log covers only the three Q6 ties. **That ruling is unadjudicated, not decided.** (A claim that it is worth 8–16 points of the company is inflated — it used hour inputs the annex's 50 hr/week creditable cap forbids.)
3. **The Q8 no-buyout ruling is a Condorcet failure.** None: 4 (plans 2, 3, 5a, 9) against offered-never-forced FMV buyout: 3 (4, 7, 10) and company call option: 2 (1, 5b). **Five of nine wanted some mechanism**; two variants of yes split and lost to a four-vote no. The consequence is load-bearing: inactive founders hold earned units with votes forever, no call, and transfers locked — 2.6% dead equity at one inactive founder, 5.5% at two, all of it enfranchised.
4. **The plurality method inflates mechanical rulings and starves strategic ones** (**survives; most useful structural criticism in the dossier**). Every 7–9 vote ruling is either a legal question with one defensible answer (83(b), MA LLC, Wage Act gating, single CEO, manager-managed, IP assignment, supersession) or market boilerplate (66⅔%, arbitration ladder, 12.5% pool). Every ruling that determines *who ends up owning what* is thin: pool size 5/8, Year-1 gap convention 3/8 and tied, activity threshold 4/9, no-buyout 4/9. Read the headline vote counts with that asymmetry in mind.
5. **The time-backstop tie-break survives, but for a different reason than recorded.** The "captured off-switch" theory fails — an early elective freeze is share-*neutral* to employees at constant cohort mix, so the 66⅔% is not adverse-interest and the recorded reasoning is not falsified. What is wrong is narrower and still serious: there is no date-certain terminus and no participant cap (§4.2). **[Corrects a claim in the first version of this document.]**
6. **A correlated-source claim I published was wrong.** The first version of this rebuttal asserted that the 8/9 and 8/8 rulings were one practitioner source counted eight times, with plan-10 citing Slicing Pie 12 times. Actual counts across `all-plans`: plan-1 22, plan-2 11, plan-3 28, plan-5 33, plan5 22, plan-7 25, plan-9 33, plan-review 2, **plan-4 zero, and plan-10 zero.** Plan-10 cites it zero times and still voted with the eight, so "the eight that voted together are exactly the eight that read the same source" is **false**. Effective independent N is not 1. **[Refuted; correction published here.]**

---

## 6. The problem both documents are ignoring

The company has downsized from ~10 employees to 4 — roughly six employees and possibly one founder departed, after working unpaid.

Under the consensus as written, pool points are **unconditional once earned**, and the Year-1 retroactive settlement covers every participant who submits an evidence-backed statement. The only forfeiture rules attach to the founder *reserve*. Searching all nine plans for treatment of departed non-founder contributors returns essentially nothing — the corpus's leaver analysis is entirely about inactive founders who *remain* members. The consensus inherited that blind spot. Excluding the departed would be a **new decision**, not an application of the design.

Modelled at one unpaid person-year each:

| Freeze at | Departed (7) | Each departed employee | 4 active founders | 4 active employees |
|---|---|---|---|---|
| T = 1 yr (now) | **44.1%** | 6.1% | 30.2% | 24.4% |
| T = 2 yrs | **27.7%** | 3.8% | 41.1% | 30.0% |
| T = 3 yrs | 19.8% | 2.6% | 47.5% | 31.7% |
| T = 4 yrs | 15.2% | 2.0% | 51.9% | 31.9% |

Sensitivity at T=2: 13.1% low, ~24.9% central, 26.3% if the departed held above-average bands. The aggregate does not fall under the 10–15% dead-equity band until roughly year seven, and the design freezes at the *earliest* trigger — most likely T ≈ 1.5–3, exactly where the number is 20–28%. On the stricter practitioner test in the plans' own references (any single uninvolved holder above 5%), each departed employee is individually over the line at settlement, and there are six.

**This corrects a figure given earlier in conversation.** The claim that downsizing lifted founder ownership to ~60% holds only if the departed are removed from the ledger denominator, which the design forbids. Counted correctly the four active founders are nearer **30% today**.

Three consequences worth more than the entire class-pool dispute:

- **The drag-along and conversion covenant bind only OA signatories.** A departed holder who never signs cannot be dragged into a sale and has not pre-consented to the Delaware conversion. One unsigned 3–5% holder can hold up a change of control.
- **Departed wage claims are crystallised and non-curable.** *Reuter v. City of Methuen*, 489 Mass. 465 (2022): all accrued wages fell due on the day of discharge, and late payment does not cure. At the $15/hr floor with §151 §1A overtime, trebled: **~$540k–945k for the six departed alone**, mandatory fees on top, personally guaranteed as to managing members, limitations running to ~2029. (Figures on the wage floor, not on the $82.50 rate-card benchmark — the Wage Act remedies wages *owed*, not forgone market opportunity, and a version of this estimate inflated ~5× by using the benchmark did not survive cross-examination.) If anyone was promised a salary above minimum wage, *Stanton* treats deferred salary as wages at the promised rate and the number moves 3–8×. These are also the people most likely to sue.
- **The consensus overstates one legal point in a way that removes the only cure.** Q15's "not privately releasable" is too absolute. *Prospective* waiver and equity-for-wages are void §148 special contracts (*Stanton*); but settlement of an already-existing bona fide dispute is enforceable if the release is plainly worded and **specifically names the Wage Act rights waived** (*Crocker v. Townsend Oil Co.*, 464 Mass. 1 (2012); *Lipsitt v. Plaud*, 466 Mass. 240 (2013) on the survival of contract claims). So the departed *can* be closed out — with cash, individual counsel-drafted Wage-Act-specific releases, separate consideration. **Not with equity.**

The sharpest drafting hazard: Q18 conditions equity on IP assignments "as a condition of receiving any equity," while Q4 settles Year 1 for everyone. Presented to an unpaid ex-worker that is functionally *"sign this to get your shares."* If the package bundles units with anything release-shaped, or any recital implies the equity accounts for the unpaid year, you have created a void special contract **and** manufactured evidence of intent.

**Ranked by leverage on founder ownership:** departed contributors **~20–30 points**; headcount and hiring policy ~10–13; paid-vs-unpaid status ~3–4; rate-band assignment a few; reserve size 5. The class pool addresses none of the top three.

---

## 7. Recommendation

**Reject** the cofounder-only pool. It caps the cofounders in the state the memo calls best (§3.1); it is shirking insurance paid for by the unpaid employees (§3.2); it cannot implement its own pricing function and pays non-managing cofounders a liability premium they do not bear (§3.3); its parameter is underived (§3.4); its cap table does not close (§3.5); and it creates a standing incentive against admitting the fifth partner already promised equal terms (§3.7).

**Adopt instead:**

1. **A quarterly pro-forma freeze cap table.** This is Firas's own deleted v2 rule 5. It costs **zero equity**, fits inside the already-adopted quarterly transparency regime (Q22), and fully answers his actual stated grievance — that the number is an unknowable output discovered in diligence. An information defect does not need a distributive remedy, and this is the highest-value, lowest-cost item in the entire dossier.
2. **A two-sided band on the *active*-founder class, 50/65, capped at 8 points of adjustment, delivered as a pre-consented conversion-ratio adjustment agreed *now*.** Best-engineered proposal in the dossier and it survived cross-examination. It amends nothing high-confidence: the floor already exists as plan-1's appendix provision, the 50 and 65 are Firas's own numbers from `9f77445`, and it touches none of Q2 (8/9), Q3 (8/8), Q7 (8/9) or Q8 (9/9). Restricting it to *active* founders and never topping up inactive ones is precisely what defeats the dead-equity objection the class pool cannot answer. Two-sided matters: it also stops the cofounders capturing a windfall in the states where the employees carried the company. **Do it now, not at the freeze** — a freeze-time top-up in profits interests carries a hurdle at then-current FMV and is worth roughly nothing on day one, which is Firas's own v2 objection and it is correct.
3. **A participant cap or date-certain terminus on the ledger**, addressing §4.2 — the surviving half of the backstop objection.
4. **Cap or price the cash × 4.0 multiplier** (§4.5) before signing.

**Do not adopt** a calendar-period decaying risk multiplier — which the first version of this document recommended as the primary mechanism. It is **mathematically near-inert**, worth +0.1 to +2.0 points. The founder pool share Σmₜ·Fₜ / Σmₜ·(Fₜ+Eₜ) is invariant to the multiplier vector whenever the founder-to-employee point ratio is constant across periods: vectors [1,1,1], [4,3,2], [10,1,1] and [1,1,10] all return exactly 0.555556 on identical inputs. It bites only where cohort mix varies by period — i.e. a genuine pre-formation window in which founders worked alone. Since ~15 people worked unpaid from early on, that window is small here. A **join-cohort coefficient** was offered as an alternative and also fails: indexing all of a person's hours to their join date prices a month-30 hour differently for two people at identical company risk, which is a seniority premium, not a risk premium. If the risk mispricing is to be addressed at all, do it through a **pre-formation window** only, and price it honestly at 1–5 points.

**Reopen two rulings:** Q8's no-buyout (§5.3) — you need a lawful way to retire a departed founder's units and to buy the departed founder's consent to the restatement; and Q4's missing-records handling (§5.2), which was never adjudicated.

**Also fix:** scope OA adoption to persons who are members immediately before adoption, so departed contributors cannot hostage the founding document; condition every unit issuance on signature so unsigned holders are either bound or unissued; decouple the breakeven freeze trigger from the market-comp remediation, since doing the legally mandatory thing currently pushes toward a trigger that crystallises the departed's 25–44%; and restate Year-1 finality honestly — final among signatories, on equity questions only, never against a non-signatory's wage claim.

**Sequence.** The four current employees onto lawful ≥$15/hr payroll or completed counsel-validated member restructuring **this week** — that violation accrues daily and the liability is personal. Departed-worker settlement is a separate workstream on a different clock: gating it on signing freezes the company indefinitely, so gate it on financing and conversion, with exposure quantified and reserved before anyone signs.

---

## 8. Plain-language summary

The company is a pizza with 100 slices. The agreed plan says you get slices for work you actually do, recorded in a notebook, same rules for founders and employees.

Firas wants to promise the four founders 55–60 slices up front instead of letting the notebook decide. His worry: if founders hold less than half, investors will think the founders aren't really in charge.

**Why the promise is a bad deal — including for him.** A fixed promise is a *ceiling* as well as a floor. If the four founders work harder than everyone else, the notebook would have given them 64 or 69 slices — and the promise takes those away. His own memo has a line saying "all four cofounders outwork everyone: ~60%+," and then declares that case impossible. He is proposing to sell the upside to insure the downside.

And the downside it insures is the case where founders *stopped working*. That's where the promise pays: +2 slices if everyone works, +8 if one founder quits, +14 to +22 if two quit. The people who pay are the employees who covered the abandoned work. Investors have a name for slices held by people who quit — dead equity — and it's a reason to say no.

**Why the target is wrong too.** The 56 he's aiming at is counted *after* investors take their cut; his 55–60 is counted before. Once investors take theirs, his proposal lands near 40. He'd miss his own target — and so would the current plan, which is the honest caveat.

**What he's right about, and it's important.** Nobody ever asked what the founders' total would be. That question is missing from the whole plan, and the answer could be anywhere from 37 to 63 slices — and it drops every time you hire someone, with nothing to stop it. He's also right that an hour of work back when there was no product and no pay was worth more than the same hour today. Both worth fixing. Neither needs a separate founder pool.

**The cheapest fix is free.** Publish a one-page "if we froze today, here's the cap table" every quarter. That was in his own earlier draft and he deleted it. His actual complaint is that the number is unknowable until diligence — so make it knowable. You don't need to move any slices to fix a problem about not knowing.

**And the thing nobody was looking at.** Six workers left. Under the plan as written they keep every slice they earned — possibly 25 to 44 slices held by people who aren't here. That's the real problem, five to ten times bigger than this argument, and those same six people are owed roughly half a million to a million dollars in unpaid wages that must be settled in cash, not equity.

---

## 9. Method and limitations

**Method.** 12 agents: five hostile critic lenses (citations, arithmetic, internal consistency, Massachusetts law, incentives); four advocates instructed to build the strongest case for the memo and to attack the consensus; three cross-examiners tasked with attacking *both* prior stages and marking each finding survives / weakened / refuted. Plus two focused agents on the downsizing and citation verification. Roughly a third of the critique did not survive cross-examination, and those results are published in §3.10 and §5 rather than dropped.

**Limitations.**

- **Citation verification was degraded.** The environment's proxy denied CONNECT for every host, so no primary source was fetched. Findings rest on search-index content with excerpts, verbatim quotation from files inside this repository, and arithmetic reconciliation. The three places this matters most: the exact wording of the Hellmann & Wasserman "value at stake" sentence, EquityList's measurement point, and Carta's precise definition of "employee pool." The in-repo cross-checks in §3.8 need no network and are the most reliable evidence in this document.
- **Team composition is contested and load-bearing, and the sign of the proposal flips on it.** The nine plans were briefed on 5 founders + ~10 employees (65 corpus mentions of "five founders," 26 of "~10 employees"). The memo asserts 4 cofounders + 5 employees, revised mid-drafting (`43aec25`, `8f81cf3`); the founders have since stated 4 + 4. At 4F/10E the single pool yields 42.6%, so the class pool would be worth **+12 to +17 points**; at 4F/5E it yields 55–63%, so it is roughly **neutral to negative**. Same mechanism, opposite sign, and the memo never discloses the sensitivity. Base case by configuration: 49.7% (5+10), 55.6% (4+5), 59.5% (4+4). The revision is best read as *not decision-ready* rather than manufactured — pre-signature iteration is ordinary, and the same commit that lowered the count also, correctly, sharpened the finding that the best case has no margin.
- **The departed-contributor model is a model.** Everything in §6 turns on the departed workers' actual tenure, hours and bands, and above all on whether anyone was promised a salary above minimum wage. Hence the 13%–26% and $540k–945k+ ranges.
- **Open facts that change conclusions:** was the departed founder an original member, and did they perform management functions (determines both a signature dependency and personal liability under *Segal*); were departures voluntary or terminations (*Reuter* turns on it); *Crocker*'s exact standard, recited from memory and load-bearing for the whole settlement strategy; and whether the AG's Fair Labor Division will respect a private settlement program.
- **Not legal advice.** Every authority here needs counsel verification against primary sources.

**Falsifiability.** All arithmetic is reproducible from the formula in `consensus/CONSENSUS.md` §1; disagree by changing a stated assumption, not the conclusion. The §3.1 crossover (1.25×), the §3.2 payoff schedule, the multiplier-invariance proof in §7 and the §4.2 hiring-drift table are the load-bearing computations and were each independently reproduced by two agents. The citation findings should be re-run by anyone with unrestricted network access.
