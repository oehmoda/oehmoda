# Plan 5 — Amended & Restated Operating Agreement (Business-Terms Draft)

**[Company Name], LLC — a Massachusetts limited liability company**

> **Status of this document.** This is a business-terms draft prepared by the plan5 team
> for counsel. It states the deal the members intend; it is deliberately written in plain
> business language, article by article, so counsel can convert it into a statutorily
> compliant Amended and Restated Operating Agreement under M.G.L. c. 156C. Text in
> **[BRACKETS]** marks open decision points for the founders, and items labeled
> **⚖ COUNSEL** are legal questions we are expressly not resolving ourselves. The
> rationale and evidence for every mechanism here are in `plan-5-design.md`.

---

## Article I — Formation, Purpose, and Definitions

1.1 **Continuation.** The Company continues as a Massachusetts LLC under M.G.L. c. 156C.
This Agreement amends and restates all prior oral or informal understandings, which are
superseded in their entirety. **⚖ COUNSEL:** obtain from every Member and every current
contributor a signature acknowledging supersession of all prior equity promises (including
the informal "equal partners" arrangement and the informal promise to the Advisor described
in Article XI), and advise on any promissory-estoppel exposure from those prior promises.

1.2 **Purpose.** Any lawful business, principally the development and commercialization of
the Company's software and machine-learning technology.

1.3 **Key definitions** (full definitions list for counsel to formalize):

- **Contribution Ledger** — the Company's master record of Contribution Slices (Art. IV).
- **Contribution Slice ("Slice")** — the unit of measured contribution: 1 Slice = US $1.00
  of Adjusted Contribution Value (Art. IV).
- **Contribution Units** — Units issued quarterly in respect of Slices (Art. V).
- **Founder** — the five individuals listed in Schedule A.
- **Reserved Founder Allocation ("RFA")** — each Founder's conditional, earn-only
  allocation capped at 5.0% (Art. VI).
- **Active Service** — a calendar month in which a person renders at least
  **[120] hours** of approved-workstream services to the Company (roughly 30 h/week).
- **Freeze Event** — the earliest of: (a) closing of a Qualified Financing; (b) conversion
  to a corporation (Art. XII); (c) a Change of Control; (d) the **[36th]** month after the
  Effective Date; or (e) election by the Board plus a 66⅔% Unit vote.
- **Qualified Financing** — a priced equity financing of at least **[US $1,000,000]** from
  one or more non-Member investors.
- **Benchmark Rate Table** — Schedule B: the role-based fair-market hourly rates (Art. IV.3).
- **Cause** — (for counsel to tighten) fraud, embezzlement, material and uncured breach of
  this Agreement or of an IP/confidentiality obligation, conviction of a felony involving
  dishonesty, or knowing falsification of Ledger entries.

---

## Article II — Units and Members

2.1 **Single economic class.** The Company has one class of **Units**. Each Unit carries
one vote and identical economic rights. There are no special founder classes, no
super-voting units, and no unit-holder veto held by any individual. (Design rationale:
investor-cleanliness and the fixed requirement that founders and employees compete on
identical terms — see design §3, §6.)

2.2 **Sub-series for tax only.** Units may be issued in sub-series solely so that each
grant can carry its own distribution threshold (profits-interest mechanics, Art. V.4);
sub-series never differ in voting or in relative go-forward economics.

2.3 **Admission of Members.** Every person holding at least one Unit is a Member with
information rights (Art. IX.5) and voting rights. All current active contributors
(founders and the ~10 employees) are intended to be admitted as Members at the Retroactive
Settlement (Art. VII). **⚖ COUNSEL:** advise on the employment-law characterization of
unpaid contributors who become Members (partner/member vs. employee under the FLSA and the
Massachusetts Wage Act) — see Article XIV.2, which is the single most urgent legal item in
this engagement.

2.4 **No obligation to contribute capital.** No Member is required to make cash capital
contributions. Cash contributions are voluntary and are credited through the Ledger
(Art. IV.4).

---

## Article III — The Two Equity Pools

3.1 **Contribution Pool — 75%.** Seventy-five percent (75%) of the Company's pre-Freeze
fully-diluted equity is distributed exclusively through the Contribution Ledger system of
Articles IV–V, on terms identical for every participant: founder, employee, advisor, or
consultant. No equity is issued outside Articles IV–VI except as expressly stated in
Art. XII (financing-related issuances after a Freeze Event).

3.2 **Reserved Founder Allocations — up to 25%.** Up to twenty-five percent (25%) —
5.0% per Founder — is issuable only under the earn-only RFA rules of Article VI. Any RFA
percentage not earned is **never issued**: it is not redistributed to other founders; it
simply enlarges every Ledger participant's pro-rata share (the Contribution Pool absorbs
it automatically under the Art. VI.5 formula).

3.3 **No other equity.** The Company shall not promise, grant, or reserve equity by any
other route before a Freeze Event. Any purported oral promise of equity is void.

---

## Article IV — The Contribution Ledger

*(This Article is the measurement engine. It is written so a spreadsheet can compute every
number; the worked example is design §5.6.)*

4.1 **What counts.** A contribution is creditable only if it is (a) hours of service on an
**Approved Workstream**, (b) cash paid to or for the Company, or (c) tangible/intangible
property accepted by the Board at an appraised or documented value. Approved Workstreams
are set quarterly in the Company's plan (Art. VIII.4); work outside them earns zero unless
ratified by the Board within 30 days.

4.2 **Slice formula.**

```
Time:      Slices = Hours × BenchmarkRate(role) × 2.0     (non-cash multiplier)
Cash:      Slices = Dollars × 4.0                          (cash multiplier)
Property:  Slices = Accepted FMV × [2.0]                   (Board-accepted valuation)
```

The 2.0×/4.0× multipliers are the Slicing Pie risk multipliers (unpaid work and at-risk
cash are compensated for risk, not just time — design §5.2). They apply identically to
every participant.

4.3 **Benchmark Rate Table (Schedule B).**

- Rates are **role-based, not person-based**: each Approved Workstream assignment carries a
  role/level (e.g., Software Engineer L3–L6, Engineering Manager, Product/Business Lead,
  Executive/CEO, Designer, ML Research Consultant).
- Each rate = the **[50th]** percentile Boston-market total cash compensation for that
  role/level from a named published source **[Carta Total Compensation / Levels.fyi /
  Pave — pick one primary source]**, divided by 2,080 hours.
- **External specialists** (including the Advisor, Art. XI) are credited at their
  **documented, arms-length market rate** (e.g., an invoiced consulting rate actually
  charged to third parties within the past 24 months), capped at **[5×]** the highest
  internal Schedule B hourly rate. Same rule for anyone; no named-person exceptions.
- The Table is refreshed annually by the Board from the named source and takes effect only
  prospectively; changing the *methodology* (source, percentile, multipliers) requires
  75% of Units (Art. X.2).
- A person may hold different roles for different workstreams in the same month (e.g., 60%
  coding at L5, 40% engineering management), logged separately.

4.4 **Logging, attestation, audit.**

- Hours are logged **monthly, within 10 days** of month-end, per workstream, with a
  one-line description. Late entries beyond 60 days are void.
- Each workstream has a **Lead** who attests the entries of everyone on it (the Lead's own
  entries are attested by another Lead or a Manager).
- Hours cap: at most **[250]** creditable hours per person per month.
- The **Ledger Committee** (Art. IX.4) audits a random **[10%]** sample of entries
  quarterly and every entry flagged by any Member. Knowing falsification is Cause
  (Art. I.3) and forfeits **[2×]** the falsified Slices.
- Entries unchallenged **60 days** after quarterly publication become final and
  incontestable (repose — keeps the cap table quiet, design §5.4).

4.5 **Outcome bonus (bounded subjectivity).** **[OPTIONAL — DECIDE]** The Board may award
bonus Slices for exceptional outcome events (shipped milestone, signed revenue, funding
secured), capped at **[10%]** of the total Slices otherwise accrued Company-wide that
quarter, allocated by unanimous Board resolution with written reasons published to all
Members. If the founders prefer a purely mechanical system, strike this section; the
design works without it (design §5.3 discusses the trade-off).

4.6 **What is *not* credited.** Ideas as such, seniority as such, the fact of being a
founder, social capital, and titles earn zero Slices. Vision/strategy/management work *is*
credited — as hours in the appropriate Schedule B role. (Design §5.3: price the role, don't
score the brilliance.)

---

## Article V — Quarterly Issuance of Contribution Units

5.1 **Mechanic.** Within 30 days after each quarter, the Company issues to each participant
**one Contribution Unit per Slice** earned that quarter (Units are never re-priced,
clawed back, or rebalanced; the growing denominator is what makes the split dynamic —
each person's percentage at any time is their cumulative Units ÷ total Units, which
equals their share of cumulative Slices; design §5.4).

5.2 **Identical terms.** Founders, employees, and consultants receive the same Unit-per-
Slice rate, the same class, and the same paperwork. This is the requirement-2 mechanism.

5.3 **No vesting on Contribution Units.** Contribution Units are issued fully earned —
the work has already happened at risk. (Forward-looking retention is handled by the RFA
(Art. VI), the Freeze-Event refresh grants (Art. XII.4), and expected investor re-vesting
(Art. XII.5).)

5.4 **Tax mechanics.** Each quarterly issuance is intended to be a **profits interest**
(Rev. Proc. 93-27 / 2001-43 safe harbor) with a per-series distribution threshold equal
to then-current Company value, and holders will make protective 83(b) elections within
30 days of each issuance. **⚖ COUNSEL:** implement threshold-setting and 83(b) mechanics;
advise whether early grants while value is nominal should instead be capital interests;
advise on partner-status consequences (K-1s, self-employment tax, no-W-2 rule) for the
~15 recipients — and whether this argues for accelerating the Art. XII conversion.

5.5 **Distribution waterfall.** Non-liquidating distributions (unlikely pre-Freeze) and
liquidation proceeds follow the thresholds in 5.4, then pro rata by Units.

---

## Article VI — Reserved Founder Allocations (earn-only, capped at 5% each)

6.1 **Cap.** Each Founder's RFA is capped at **5.0%** of post-Freeze fully-diluted equity
(before the financing-related issuances of Art. XII); 25% across all five. This implements
fixed requirement 1.

6.2 **Earning schedule — use it or lose it.** The RFA accrues **1/36th per month of
Active Service** (≥ [120] h/month, Art. I.3) over the 36 months following the Effective
Date, with **retroactive credit** for each month of the pre-Effective-Date year in which
the Founder rendered Active Service (as established in the Retroactive Settlement,
Art. VII). Months without Active Service earn nothing and **cannot be made up**; the
earning window closes permanently at month 36. A Founder who never returns to Active
Service keeps only the fraction already accrued.

6.3 **No transfer of unearned RFA.** Unearned RFA lapses to the benefit of the whole
Contribution Pool (Art. III.2). Founders cannot gift, sell, or reassign RFA.

6.4 **Status, not units, until Freeze.** The RFA is a contractual entitlement tracked on
the Ledger; the corresponding Units/shares are issued only at the Freeze Event (or the
Founder's earlier death/disability, at the then-accrued fraction). **⚖ COUNSEL:** paper so
that accrual is taxed favorably (profits-interest or restricted-equity treatment rather
than deferred compensation; consider §409A once converted).

6.5 **Freeze-Event arithmetic.** At the Freeze Event, with `E_f` = Founder f's earned
fraction (accrued months ÷ 36, capped at 1):

```
Founder f's RFA stake      = E_f × 5% of post-Freeze fully-diluted equity
Total RFA issued           = Σ_f (E_f × 5%)            (≤ 25%)
Contribution Pool share    = 100% − Total RFA issued   (≥ 75%)
Each participant p's total = (p's cumulative Slices ÷ all Slices) × Pool share
                             + p's RFA stake (if a Founder)
```

A spreadsheet with two inputs per person (Slices; Active-Service months if a Founder)
computes the entire cap table.

6.6 **RFA is the only founder-specific term.** Outside this Article, the word "Founder"
confers nothing: no board seat, no veto, no rate premium, no title.

---

## Article VII — Retroactive Settlement of Year One

7.1 **One-time reconstruction.** Within **[45] days** of the Effective Date, every person
who contributed since inception submits a Year-One statement: monthly hours per
workstream, role claimed, cash outlays, and supporting evidence (git history, PR reviews,
commit logs, calendars, design docs, email/Slack records, testimony of co-workers).

7.2 **Evidence weighting.** Hours supported by contemporaneous artifacts are credited at
100%. Hours supported only by after-the-fact estimation are credited at **[50%]**.
Claimed average hours above **[60/week]** are capped at that level. The same Schedule B
rates and 2.0× multiplier apply as for go-forward work. Git metrics are **evidence of
work, not the measure of it** — the Ledger Committee corroborates, it does not count
commits (design §5.5).

7.3 **Adjudication.** The initial Ledger Committee (Art. IX.4, with its independent
member) scores all statements, publishes a draft Year-One Ledger to all participants,
takes objections for **21 days**, resolves them with written reasons, and the result is
ratified by a **75% Unit vote counted after** provisional issuance **[ALTERNATIVE: ratified
by a 75% headcount vote of all participants before issuance — DECIDE; headcount avoids
bootstrapping objections]**. Unresolved individual disputes go to Art. XIII mediation/
arbitration without holding up everyone else's issuance.

7.4 **Effect.** The Year-One Ledger seeds everyone's opening Unit balances and each
Founder's retroactive Active-Service months (Art. VI.2). Inactive founders receive
exactly what their Year-One evidence supports — nothing else. This, plus Art. VI, is the
complete answer to founder inactivity: the past is paid at the same rate as everyone
else's past, and the future accrues only while active.

---

## Article VIII — Management: Board, CEO, Domain Leads

8.1 **Manager-managed.** The Company is manager-managed under c. 156C. Authority sits in
a **Board of three (3) Managers**, elected **annually** by the Members (one Unit, one
vote; **[DECIDE: cumulative voting to protect minority holders — recommended]**). No
Manager seat is reserved for founders. A Manager may be removed at any time, with or
without cause, by a majority of Units.

8.2 **CEO.** The Board appoints, evaluates annually, and may remove a **Chief Executive
Officer** — the single accountable executive. The CEO need not be a founder or a Manager
**[DECIDE: whether the CEO is automatically one of the 3 Managers — recommended yes]**.
The CEO runs day-to-day operations and makes any operating decision not reserved below,
after the consultation duty of 8.3.

8.3 **Decision protocol ("consult, then decide").** For significant operating decisions,
the CEO must (a) solicit written or recorded input from the affected Domain Leads and any
Member who requests to be heard, within a defined window (≤ 5 business days), then
(b) decide and record the decision and reasons in the decision log (Art. IX.6). Failure of
consensus never blocks the decision; failure to consult is reviewable by the Board.
(Evidence basis — fast-decision and shared-leadership research: design §4.)

8.4 **Domain Leads.** The CEO appoints Leads for each major domain (e.g., Product,
Platform, Research, Operations) with real, published decision authority within their
domain and their quarterly Approved Workstreams. Leads attest Ledger entries (Art. 4.4).
Leadership work is compensated only through the Ledger at the corresponding Schedule B
role rate — leadership is a job here, not a rank.

8.5 **Board reserved matters (majority of the Board required):** annual plan and budget;
Approved Workstream plan; adopting/refreshing Schedule B from the named source; hiring or
terminating any person; admitting a new Ledger participant; property-contribution
valuations (4.2); bonus-Slice awards (4.5); litigation; contracts > **[US $25,000]** or
> 12 months; IP licenses outside the ordinary course.

8.6 **Supermajority member matters — 66⅔% of Units:** sale/merger/dissolution; conversion
(pre-approved in Art. XII); any equity issuance not mandated by Articles V–VI; debt
> **[US $100,000]**; related-party transactions (also requiring disinterested-Board
approval); amendment of this Agreement except the entrenched articles.

8.7 **Entrenched matters — 75% of Units:** amendment of Articles III–VII, X.2, or this
8.7 (the equity engine and its amendment rules); changes to Schedule B *methodology*;
waiver of the Art. XII conversion obligation.

8.8 **Deadlock.** With a three-person Board and Unit-majority elections, standing
deadlock is structurally unlikely; if the Board cannot fill a vacancy or pass the annual
plan for 60 days, any Manager may put the question to a Unit vote, which decides. There
are no individual vetoes anywhere in this Agreement.

---

## Article IX — Committees, Records, Transparency

9.1 The Board may form committees; two are mandatory:

9.4 **Ledger Committee.** Three people: one Manager, one non-founder Member elected by
Members annually, and one outside independent (a fractional CFO/accountant engaged for
this purpose) **[DECIDE: outside member optional to save cost, but recommended for the
Retroactive Settlement at minimum]**. Runs Art. IV.4 audits and Art. VII adjudication.
Members with a conflict on an entry are recused.

9.5 **Information rights.** Every Member receives: quarterly Ledger reports (all
participants' Slices and running percentages — **the Ledger is transparent to all
participants by default**; design §5.4), quarterly financials, the annual plan, and the
decision log. **[DECIDE: whether rate-table role assignments are also published — 
recommended yes; transparency is the fraud-control.]**

9.6 **Decision log.** All CEO significant decisions (8.3) and all Board resolutions are
logged and visible to Members.

---

## Article X — Transfers and Departures

10.1 **No transfers** of Units without Board consent, except to estate-planning vehicles;
right of first refusal to the Company, then Members; **tag-along** on any permitted sale
> 5% of Units; **drag-along** if holders of ≥ 66⅔% approve a sale (every Member
pre-agrees to sell on the same terms). **⚖ COUNSEL:** standard package, plus spousal
consents (Massachusetts).

10.2 **Departure outcomes.**

| Scenario | Contribution Units | RFA |
|---|---|---|
| Voluntary resignation | Keeps all (earned) | Accrual stops; keeps accrued fraction |
| Termination without Cause | Keeps all | Accrual stops; keeps accrued fraction |
| Termination for Cause | Company option, for **[90] days**, to repurchase **all** of the person's Units at the **lower** of Ledger value (1 Slice = $1) or appraised FMV | Forfeits entirely, including accrued |
| Death / permanent disability | Keeps all; estate takes subject to this Article | Accrued fraction settles in Units immediately |
| Ledger fraud (proven) | Forfeits 2× falsified Slices (4.4); Cause treatment applies | Forfeits entirely |

Earned equity is deliberately **not** repurchasable in no-fault departures — clean but
harsh forfeiture regimes invite litigation and chill honest logging; the RFA and refresh
grants carry the retention load (design §6.4). **[DECIDE: optional Company FMV-repurchase
right on no-fault departures — investors mildly prefer it; we recommend against, see
design §6.4.]**

10.3 **Continuing obligations.** Every participant signs, as a condition of any Unit
issuance: confidentiality + IP assignment (PIIA) covering all work since inception
(**⚖ COUNSEL: confirmatory assignments back to day one — a known diligence killer if
missing**), a 12-month non-solicit, and — only where enforceable and desired —
a Massachusetts-compliant non-compete (**⚖ COUNSEL: G.L. c. 149 § 24L garden-leave/
consideration requirements; do not use for anyone terminated without cause**).

---

## Article XI — The Advisor (the ML Professor)

11.1 **One system, honestly priced.** The Advisor participates in the Contribution Ledger
on **exactly the terms of Articles IV–V** — the identical-terms requirement admits no
carve-out. His "higher rate" is honored the only objective way available: his Schedule B
rate is his **documented arms-length ML-consulting market rate** (Art. IV.3), which will
substantially exceed engineering rates. His "decent share" is whatever that rate × his
actual part-time hours earns — no floor, no cap other than the rate cap of Art. IV.3.

11.2 **Retroactive credit.** His pre-Effective-Date contributions run through Article VII
like everyone else's, at the same documented rate.

11.3 **Role.** Title **[Chief Scientific Advisor / SAB Chair]**; no Units-for-title; the
title is free. **[DECIDE: if the founders additionally want to lock in his affiliation for
signaling, the market-norm instrument is a small separate advisor option grant at the
Freeze Event, 0.10%–0.50%, 2-year monthly vesting, from the post-Freeze pool — this is
OUTSIDE the pre-Freeze system and therefore requires the 66⅔% vote of Art. 8.6. Market
norms and our recommendation (participate-in-ledger only, walk if refused): design §7.]**

11.4 **⚖ COUNSEL (all before signature):** (a) Yale conflict-of-interest disclosure and
approval; (b) Yale consulting-time limits; (c) Yale patent-policy carve-out — a written
agreement that his Company work uses no Yale resources, funds, or students, and a
representation that Company IP is outside any Yale assignment obligation; (d) consultant
classification (1099) and equity-compensation tax; (e) supersession of the informal
promise (Art. 1.1).

---

## Article XII — Conversion to a Delaware C-Corporation (pre-agreed)

12.1 **Obligation.** Upon the earlier of (a) Board determination that a financing or
accelerator requires it, (b) a Qualified Financing term sheet, or (c) **[24] months**
after the Effective Date, the Company **shall** convert into a **Delaware C-corporation**,
and every Member pre-consents (this Article is the drag for conversion; no re-vote).
**[DECIDE — see design §8: our recommendation is to convert promptly (within ~6–12
months, after the Retroactive Settlement stabilizes the ledger), not to wait for a term
sheet: it starts the QSBS holding clock while asset values are trivial, replaces K-1
complexity with ordinary equity comp, and removes the last diligence objection.]**

12.2 **Mechanics.** **⚖ COUNSEL:** choose the conversion route from Massachusetts
(statutory conversion if available to a foreign corporation, otherwise merger into a new
DE corp or interest-for-stock exchange), tax-free under §351/368; preserve the Ledger
percentages exactly; QSBS qualification of the newly issued stock (asset test at
conversion, per-issuer cap, post-July-2025 §1202 rules).

12.3 **Effect on the system.** Conversion is a Freeze Event: Art. VI.5 arithmetic fixes
the cap table; the Ledger stops; each holder receives common stock pro rata.

12.4 **Go-forward compensation.** Post-conversion the company adopts a standard equity
incentive plan with an initial pool of **[15%]** post-money **[10–20% band; negotiate
with lead investor]**; future contribution is compensated by salary (once funded) plus
refresh option/RSA grants under the plan — the dynamic ledger is a bootstrap-phase
instrument and deliberately does not survive institutional financing (design §5.4, §8).

12.5 **Expected re-vesting.** Members acknowledge that a lead investor will likely
require service-based re-vesting of a portion of founder/employee stock; Members
pre-commit to accept re-vesting of up to **[25%]** of their then-held shares over up to
**[2]** years with double-trigger acceleration, if the Board and 66⅔% of Units approve
the financing. (Bounded pre-commitment beats an open fight at term-sheet time; design §8.)

---

## Article XIII — Dispute Resolution

13.1 **Ladder.** (1) Written issue to the CEO/Board → response within 10 business days;
(2) non-binding **mediation** (JAMS/AAA, Boston) within 30 days; (3) final, binding
**arbitration** (single arbitrator, JAMS, Boston; expedited rules; each side bears own
costs unless the arbitrator shifts for bad faith). Carve-outs: injunctive relief for
IP/confidentiality breaches may go directly to court. **⚖ COUNSEL:** enforceability;
whether Ledger-entry appeals should have a lighter fast-track (we recommend a 1-page
submission, documents-only arbitration for disputes < $25k of Slices).

13.2 **No withdrawal remedy.** A Member may resign services at any time (Art. X) but has
no right to force dissolution or redemption. **⚖ COUNSEL:** confirm default c. 156C rules
are properly overridden; address any close-corporation-style fiduciary claims
(Massachusetts *Donahue* line) in drafting.

13.3 **Fiduciary scope.** Managers owe the Company good faith and loyalty; competing with
the Company while a Member receiving Ledger credit is prohibited. **⚖ COUNSEL:** the
extent to which c. 156C permits tailoring fiduciary duties in Massachusetts (contrast
Delaware); draft conflict-transaction safe harbor (disinterested approval per Art. 8.6).

---

## Article XIV — Urgent Compliance Items (flagged, not resolved)

14.1 This Article is a to-do list for counsel, priced into the design (design §9):

14.2 **Unpaid workers.** ~10 people have worked ~a year unpaid. For-profit companies
cannot use volunteers; equity does not satisfy minimum wage; the Massachusetts Wage Act
carries **mandatory treble damages, attorney's fees, and personal liability** for
responsible managers. Counsel must advise **immediately** on: member/partner
characterization of Ledger participants; whether wage claims survive Member admission;
release/settlement mechanics (Wage Act claims are not waivable by ordinary release);
starting minimum cash compensation (and the fundraising this forces); and statute-of-
limitations posture. **This risk dwarfs every equity-design question in this document.**

14.3 **Securities.** Unit issuances to ~16 people: federal exemption (Rule 701 /
§4(a)(2)) and Massachusetts blue-sky compliance.

14.4 **Tax.** Profits-interest implementation (V.4); 83(b) discipline (30-day,
non-extendable); partner K-1/SE-tax consequences; conversion tax (XII.2); §409A once a
corporation.

14.5 **IP chain.** Confirmatory PIIAs from every past contributor (X.3); Advisor/Yale IP
(XI.4); open-source audit of the codebase before diligence.

14.6 **Insurance & basics.** D&O/EPLI once payroll starts; workers' comp (mandatory in
MA once employees are paid); registered agent, annual reports.

---

## Article XV — Miscellaneous

15.1 Governing law: Massachusetts (Delaware after conversion). 15.2 Amendment: per
Art. 8.6/8.7 only, in writing. 15.3 Entire agreement; supersedes all prior oral equity
arrangements (1.1). 15.4 Severability; counterparts; e-signature. 15.5 Spousal consent
riders. 15.6 Schedules: **A** Founders; **B** Benchmark Rate Table + named source +
refresh procedure; **C** Approved Workstreams (initial); **D** Year-One Settlement
procedures & evidence rubric; **E** Form PIIA; **F** Form Advisor agreement.

---

*Prepared by plan5. Every mechanism above is justified, with evidence quality stated
honestly, in `plan-5-design.md`; sources in `plan-5-references.md`.*
