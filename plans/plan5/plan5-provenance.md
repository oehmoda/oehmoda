# plan5 — Provenance Report

Truthful account of how team plan5's deliverables were produced. Written for the
neutral reviewer comparing teams.

## ⚠ Directory-collision disclosure (read first)

When this session checked out `all-plans` to integrate (2026-08-02), the branch
**already contained `plans/plan-5/`** with a full set of files committed by a
different session (`plan-5-design.md`, `plan-5-one-pager.md`,
`plan-5-operating-agreement.md`, `plan-5-references.md`, `plan-5-conclusions.md`,
`plan-5-provenance.md`; commits `5b2a7d1` and `a582798` on `all-plans`). Those
files are **not ours** and **we did not open, read, or diff any of them** — we
observed only file names and commit subjects (`git ls-tree` / `git log --oneline`),
which was unavoidable to diagnose the collision. Because our team identity is
**plan5** (assigned working branch `claude/plan5-llc-governance-equity-jx79r1`;
all our files are prefixed `plan5-`), and because writing into `plans/plan-5/`
would have overwritten another team's deliverables — including their provenance
file — we integrated under **`plans/plan5/`** instead and left `plans/plan-5/`
byte-for-byte untouched. During the first (aborted) copy step, four of our
`plan5-*.md` files briefly existed untracked inside `plans/plan-5/`; they were
deleted before any commit, and nothing in that directory was staged or committed
by us. The reviewer should treat `plans/plan-5/` and `plans/plan5/` as two
different teams.

We also confirm the original isolation rule was honored throughout the research
phase: our working branch began with no commits and an empty tree, and we never
checked out, read, diffed, or browsed any other team's branch or files.

## 1. What the session did, step by step

1. Received the task; confirmed the assigned branch
   `claude/plan5-llc-governance-equity-jx79r1` was empty (no commits, empty
   tree — orphan-equivalent), satisfying the isolation requirement without
   creating a second branch.
2. Launched three research subagents in parallel (details in §2), each instructed
   to verify every URL before citing.
3. While subagents ran: drafted `plan5-operating-agreement.md` (the design's
   business terms were decided by the main agent, not delegated), and computed
   the worked-example equity table with a small Python script (arithmetic in
   §5).
4. Legal/tax subagent returned; its finding that profits interests can evaporate
   at C-corp conversion forced an edit to OA §3.6. Committed and pushed
   (`db69d7f`; the initial OA draft had been committed as `536ca64` after a
   stop-hook reminder to commit untracked files).
5. Academic subagent returned; wrote `plan5-references.md` Parts A–B from the
   legal + academic streams.
6. Industry subagent returned; completed references Part C, wrote
   `plan5-design.md` (full framework with inline citations), wrote
   `plan5-one-pager.md`, fixed one cross-reference in the OA, committed and
   pushed (`3088dd8`).
7. Integration task: fetched `all-plans`, discovered the `plans/plan-5/`
   collision described above, restored that directory to its remote state,
   copied our four deliverables from our own branch via
   `git show claude/plan5-llc-governance-equity-jx79r1:<file>` into
   `plans/plan5/`, extracted verbatim search queries from the three subagent
   transcripts (regex extraction of the `query` fields, in order), wrote this
   file, committed to `all-plans`, pushed, and mirrored this file onto our own
   branch.

## 2. Agents and subagents

**4 total: 1 main agent + 3 subagents** (general-purpose type, launched in
parallel, each a single-shot research task):

| Subagent | Task |
|---|---|
| Academic | Peer-reviewed evidence on founder equity division, dynamic vs. static splits, shared vs. vertical leadership, co-CEOs, free-riding, founder-CEO succession, venture boards, organizational justice, team conflict — with numbers, samples, and strength ratings |
| Industry | Practitioner/data evidence: Slicing Pie mechanics and criticisms, FAST agreement, Carta datasets (splits, pools, vesting, advisor grants), YC guidance, investor dead-equity/vesting writing, Index/Holloway benchmarks, DRI/two-door/RAPID provenance, deadlock mechanisms, failure-cause data, comp benchmarks |
| Legal/tax | Statutes/cases/regulator sources: DE C-corp preference, QSBS §1202 incl. 2025 OBBBA, conversion mechanics, profits interests, 83(b), MA Wage Act (incl. *Reuter*, *Cook*), FLSA, §148B, c.156C, MA noncompete act, Yale COI/patent policies, Rule 701/409A, foreign qualification, NVCA reverse vesting |

The main agent made all design decisions, wrote all four deliverables, and ran no
web searches itself.

## 3. Every web search query, verbatim, in execution order

Each subagent's first tool query was a ToolSearch harness call
(`select:WebFetch,WebSearch`) to load tool schemas — listed for completeness; all
subsequent entries are WebSearch queries. Extracted mechanically from the
subagents' transcripts (order preserved; quotes unescaped).

### Academic subagent (31 WebSearch queries)
1. Hellmann Wasserman "The First Deal" founder equity Management Science
2. Hellmann Wasserman "First Deal" founder equity equal split percentage "quick" negotiation sample 511 teams valuation lower
3. Breugst Patzelt Rathgeber 2015 "How should we divide the pie" equity distribution entrepreneurial teams Journal of Business Venturing findings justice
4. Wasserman "Founder's Dilemma" HBR 2008 statistics "rich" "king" percent founders replaced CEO board forced out
5. D'Innocenzo Mathieu Kukenberger 2016 meta-analysis shared leadership team performance effect size rho Journal of Management
6. Nicolaides 2014 Leadership Quarterly shared leadership meta-analysis team performance rho .35 team confidence moderators
7. Wang Waldman Zhang 2014 Journal of Applied Psychology meta-analysis shared leadership team effectiveness overall effect size task complexity moderator
8. "D'Innocenzo" shared leadership meta-analysis overall corrected correlation ".19" OR ".21" OR ".24" team performance complexity moderator
9. Nicolaides "shared leadership of teams" meta-analysis 2014 "3,198" OR "43 studies" OR "41 studies" corrected correlation team performance task interdependence moderator
10. Krause Priem Love 2015 "Who's in charge here" co-CEOs power gaps firm performance Strategic Management Journal sample 71 findings
11. "shared leadership" meta-analysis D'Innocenzo "ρ = .19" OR "rho = .19" OR ".19)" team performance
12. Nicolaides et al. 2014 shared leadership meta-analysis Leadership Quarterly "team performance" corrected correlation value team confidence mediates incremental over vertical leadership
13. Feigen Jenkins Warendh "Is It Time to Consider Co-CEOs" HBR 2022 87 companies 9.5% average annual shareholder returns 6.9% index
14. Holmström 1982 "Moral Hazard in Teams" Bell Journal of Economics free rider budget breaker Nash equilibrium sharing rules
15. Wasserman 2003 "Founder-CEO succession and the paradox of entrepreneurial success" Organization Science sample findings percent replaced
16. Garg 2013 "Venture boards" Academy of Management Review distinctive monitoring implications firm performance venture capitalists
17. dynamic founder equity split renegotiation study peer-reviewed "equity split" founders renegotiate vesting contingent agreement citing Hellmann Wasserman
18. Colquitt 2001 "On the dimensionality of organizational justice" construct validation AND Colquitt Conlon Wesson Porter Ng 2001 meta-analysis 25 years organizational justice procedural justice outcomes correlations
19. de Wit Greer Jehn 2012 "paradox of intragroup conflict" meta-analysis Journal of Applied Psychology task conflict relationship conflict correlations team performance numbers 116 studies
20. Wasserman "Founder's Dilemmas" book "73%" OR "within a month" equity split dataset "10,000 founders" statistics Princeton
21. "dynamic equity split" OR "renegotiating the split" founders academic study journal entrepreneurship vesting agreements Wasserman follow-on research
22. de Wit 2012 meta-analysis relationship conflict "-.16" OR "-.18" task conflict "group performance" rho top management teams positive
23. NBER digest "Division of Founder Equity" ventures equal split "one third" OR "a third" negotiate day survey Kauffman CompStudy
24. Garg 2013 Academy of Management Review venture board abstract "venture boards" CEO monitoring propositions differ from public firm boards
25. "equity split" founding teams study 2020 OR 2021 OR 2022 journal "equal split" new venture performance vesting dynamic agreement empirical follow-up Hellmann
26. Nicolaides "The shared leadership of teams" abstract "team performance" "team confidence" collective efficacy "3,882" OR "samples" number teams
27. Hellmann Wasserman founder equity "vesting" percent of teams dynamic agreements static "quick handshake" hours negotiating
28. Hellmann Thiele "Contracting Among Founders" Journal of Law Economics Organization vesting renegotiation founder departure theory
29. "Ownership dynamics within founder teams" "external financing" journal authors year abstract equity stakes change
30. "Colquitt" 2001 "Justice at the millennium" procedural justice correlation job satisfaction organizational commitment performance values meta-analytic table
31. de Wit Greer Jehn 2012 meta-analysis "relationship conflict" rho value group performance "task conflict" "process conflict" corrected correlations proximal outcomes trust cohesion

### Industry subagent (32 WebSearch queries)
1. Slicing Pie model slices multiplier 2x non-cash 4x cash recovery framework
2. slicingpie.com recovery framework what happens slices resign fired with cause without cause buyout
3. Slicing Pie pie freezes "breakeven" OR "Series A" termination of the Grunt Fund when to stop slicing
4. Slicing Pie slice definition "fair market value" formula "individual's share" total slices percentage royalty commission sales
5. Slicing Pie criticism problems tax implications investors lawyers dynamic equity drawbacks
6. FAST agreement Founder Institute advisor equity matrix 0.10% 0.25% 0.50% 1.00% idea startup growth stage vesting
7. Carta data percentage founder teams split equity equally two founders
8. Carta data employee option pool size median seed Series A percentage fully diluted
9. Carta data vesting schedule "4-year" "one-year cliff" percentage of grants standard
10. Carta data median advisor equity grant percentage Peter Walker advisors 0.2%
11. "dead equity" cap table investor problem former founders percentage Carta OR data OR diligence
12. Y Combinator blog splitting equity among founders Michael Seibel equal split vesting
13. Fred Wilson AVC founder vesting post OR Brad Feld founder vesting dead equity cap table
14. Index Ventures OptionPlan rewarding talent employee equity benchmarks engineer percentage seed Series A
15. Holloway Guide to Equity Compensation typical equity ranges employee number hire engineer percent
16. Apple DRI "directly responsible individual" Fortune Adam Lashinsky citable source
17. Bezos 2015 shareholder letter "one-way door" "two-way door" Type 1 Type 2 decisions "high-velocity"
18. Bain RAPID decision framework bain.com recommend agree perform input decide
19. Bezos 2016 shareholder letter "disagree and commit" Day 1 high-velocity decision making
20. shotgun clause "Texas shootout" buy-sell deadlock closely held company law firm explainer mechanics
21. Noam Wasserman 65% startups fail cofounder conflict Founder's Dilemmas source
22. CB Insights top reasons startups fail post-mortem percentage "not the right team" OR disharmony
23. levels.fyi 2025 end of year report median total compensation senior software engineer US
24. FAST agreement matrix exact percentages "0.25" "0.50" "1.00" idea stage "0.20" "0.40" "0.80" startup "0.10" "0.25" "0.60" growth
25. Slicing Pie royalty ideas commission sales relationships "fair market value" rules Moyer
26. FAST agreement "strategic" advisor "0.40%" OR "0.30%" matrix standard strategic expert three levels
27. Brad Feld feld.com founder vesting "reverse vesting" post why vesting matters founders
28. deadlock resolution LLC operating agreement mediation then arbitration "baseball arbitration" buy-sell law firm
29. "Dutch auction" deadlock shareholders agreement sealed bid mechanism "Texas shootout" difference law firm
30. "Slicing Pie" recovery "terminated for cause" loses slices "cash" slices "no multiplier" OR "multiplier removed" resign good reason keeps
31. Carta founder ownership report ex-founder equity departed founders percentage cap table data
32. Carta compensation benchmark median salary senior software engineer startups 2025 data

### Legal/tax subagent (29 WebSearch queries)
1. Cooley GO why Delaware C corporation venture capital LLC
2. Orrick OR Cooley why venture capital investors won't invest in LLCs UBTI K-1 qualified small business stock option plans
3. Y Combinator SAFE documents "Delaware corporation" safe financing documents ycombinator.com
4. One Big Beautiful Bill Act QSBS section 1202 changes stock issued after July 4 2025 tiered exclusion 50% three years 75% four years 100% five years $15 million cap $75 million gross assets law firm
5. LLC to C corporation conversion QSBS 5-year holding period starts basis fair market value at conversion 10x basis section 1202 law firm
6. Delaware DGCL section 265 conversion of other entities to Delaware corporation statute text delcode.delaware.gov
7. Massachusetts LLC convert to Delaware corporation chapter 156C merger no conversion statute foreign entity law firm explainer
8. Rev. Rul. 84-111 three methods LLC partnership incorporation section 351 nonrecognition assets-over assets-up interests-over law firm explainer
9. Rev. Proc. 93-27 Rev. Proc. 2001-43 profits interest safe harbor not taxable at grant two years substantially certain income stream
10. profits interest threshold value hurdle liquidation value zero protective 83(b) election what happens on conversion to C corporation profits interests convert to stock law firm
11. IRS 83(b) election 30 days deadline restricted stock irs.gov instructions Form 15620
12. Reuter v. City of Methuen 489 Mass. 2022 mandatory treble damages Wage Act M.G.L. c.149 section 150 late payment
13. Cook v. Patient EDU LLC 465 Mass. 548 2013 personal liability LLC managers Massachusetts Wage Act
14. DOL FLSA volunteers for-profit private sector employers may not use unpaid volunteers fact sheet elaws minimum wage
15. Massachusetts independent contractor law ABC test M.G.L. c.149 section 148B three prong presumption employee
16. equity stock options not wages minimum wage FLSA must be paid in cash free and clear 29 CFR 531.27 DOL startup founders unpaid
17. Massachusetts LLC Act chapter 156C manager-managed operating agreement section 63 fiduciary duties expand restrict eliminate liability malegislature.gov
18. Massachusetts Noncompetition Agreement Act M.G.L. c.149 section 24L garden leave 50% twelve months exclusions nonsolicitation not covered 2018
19. Yale University faculty conflict of interest policy outside consulting one day per week provost.yale.edu equity startup
20. Yale Patent Policy university owns inventions made with university funds facilities Office of Cooperative Research ocr.yale.edu ventures.yale.edu royalty sharing
21. NSF NIH current and pending other support disclosure requirements outside activities startup company faculty failure to disclose consequences
22. Rule 701 compensatory benefit plan exemption securities $10 million 15% limits explainer Cooley OR Fenwick OR Carta; Rule 506(b) accredited investors
23. 409A valuation requirement stock options deferred compensation penalties why profits interests are not subject to 409A explainer
24. foreign corporation registration Massachusetts sec.state.ma.us chapter 156D section 15.03 registration within 10 days transacting business
25. NVCA model legal documents stock purchase agreement founder stock reverse vesting Series A repurchase "dead equity" investors impose vesting
26. Cooley GO founder stock vesting reverse vesting repurchase right investors require at financing "founder vesting"
27. Massachusetts Wage Act c.149 148 pay within six days termination pay discharged employee paid in full on day of discharge text
28. "156C" Massachusetts LLC "Section 24" management of limited liability company vested in members managers certificate of organization
29. Yale faculty policy equity startup company officer role "new ventures" students involvement conflict of interest guidance Yale Ventures

The main agent ran **zero** web searches.

## 4. Model and reasoning effort

The harness running this session **prohibits writing the model identifier into
repository files**; per that instruction, the model identifier is disclosed in the
chat transcript accompanying this session instead of here. All four agents (main +
3 subagents) ran on the same session model. The harness did not expose a
numeric/named reasoning-effort setting to the agent, so none is reported —
we decline to guess.

## 5. Tools used, and fetch honesty

- **Main agent:** Bash (git; one Python script that computed the worked-example
  table in `plan5-design.md` §2.6 — 2,870,320 total points, per-person
  percentages, reserve tranche math), Write/Edit (all four deliverables),
  Agent-launch for the three subagents, ToolSearch. No WebSearch/WebFetch calls.
- **Subagents:** ToolSearch (1 each, to load WebSearch/WebFetch), WebSearch
  (31/32/29 queries as listed), WebFetch (attempted **10 / 8 / 5** times
  respectively — **every attempt was blocked** with HTTP 403 by the sandbox's
  egress policy, confirmed against a control URL and the proxy status endpoint).
- **Consequence, stated plainly: no cited URL was ever actually fetched.** Every
  URL in `plan5-references.md` is "SEARCH-CONFIRMED": it appeared in live
  search-engine results whose payload showed matching page content (title,
  authors, journal/section, and usually the specific numbers quoted). Nothing is
  cited from memory alone, but nothing is fetch-verified either. This is
  disclosed in the references file itself, the design doc, and the one-pager,
  with a recommendation to spot-check load-bearing URLs from an unrestricted
  environment.

## 6. Commits

| Hash | Branch | Content |
|---|---|---|
| `536ca64` | `claude/plan5-llc-governance-equity-jx79r1` | `plan5-operating-agreement.md` — initial business-terms draft (committed mid-session after a stop-hook reminder) |
| `db69d7f` | `claude/plan5-llc-governance-equity-jx79r1` | OA §3.6 rewritten after legal research surfaced the profits-interest conversion-evaporation trap |
| `3088dd8` | `claude/plan5-llc-governance-equity-jx79r1` | `plan5-design.md`, `plan5-one-pager.md`, `plan5-references.md`; OA cross-reference fix |
| *(this commit)* | `all-plans` | `plans/plan5/` — the four deliverables copied unmodified from `claude/plan5-llc-governance-equity-jx79r1` via `git show`, plus this provenance file |
| *(mirror commit)* | `claude/plan5-llc-governance-equity-jx79r1` | This provenance file added to our own branch |

Our original branch is intact and was not force-pushed. No pull request was
opened.

## 7. Honest limitations

1. **No URL was directly fetched** (§5). Search-result corroboration is one notch
   weaker than fetch verification; five specific statistics we could not surface
   are named in `plan5-references.md` and were left unreported rather than
   recalled from memory.
2. **The four deliverables were written in one session by one main agent.** No
   independent adversarial review pass ran over the final documents; internal
   consistency was checked by the author only.
3. **The worked example uses assumed facts** (hours patterns, levels, one $20K
   cash contribution) because the real team's records don't exist yet; the rate
   table dollar figures are placeholders pending signing-date benchmark pulls,
   and are labeled as such in the OA.
4. **Some design parameters are choices, not findings** — the 2×/4× multipliers
   (adopted convention), the 240-hour/50%-of-median activity thresholds, the 2.0%
   advisor cap, quarterly recomputation, baseball arbitration for valuations.
   The design doc's §10 lists these explicitly rather than dressing them as
   evidence-driven.
5. **Legal conclusions are flags, not advice**: MA-side conversion filing
   mechanics had conflicting secondary sources; Reg D 506(b) was corroborated at
   explainer level only; both are marked lower-confidence in the references.
6. **Subagent transcripts were mined only mechanically** for this report (regex
   extraction of query strings and WebFetch call counts); we did not re-read full
   transcripts, so subagent-internal dead ends beyond what their reports state
   are not itemized.
7. **The directory collision** (top of this file) means the reviewer must
   disambiguate `plans/plan-5/` (another team) from `plans/plan5/` (us). We chose
   deviation from the literal `plans/plan-$N` template over overwriting another
   team's committed work; if the reviewer intended `plans/plan-5/` for us, the
   other team's files were there first and we defer to the reviewer to
   adjudicate.
