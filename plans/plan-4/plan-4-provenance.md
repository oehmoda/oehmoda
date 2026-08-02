# Plan 4 — Provenance Report

**Branch holding original deliverables:** `claude/founder-governance-equity-inactivity-sgxk74`
(note: no branch literally named `plan-4` exists; this was the working branch assigned
to this session, and the plan was named "plan-4" at the user's request).

---

## 1. What the session did, step by step, in order

1. **Turn 1 — user asked for a two-line summary of "the plan" (governance, equity,
   founder inactivity).** The local clone was empty (a branch with no commits), so the
   session ran `git fetch origin`, discovered the remote branches `plan-1`, `plan-2`,
   and `claude/startup-governance-equity-8webj5`, listed each branch's files with
   `git ls-tree`, viewed commit history with `git log`, and read **one** file from
   another team's work: `plan-2-one-pager.md`, via
   `git show origin/plan-2:plan-2-one-pager.md`. It then summarized plan-2 to the user.
2. **Turn 2 — user instructed: "name your plan plan4 and do not read the rest."**
   The session wrote two new documents from scratch — `plan-4-one-pager.md` and
   `plan-4-design.md` — without reading any further repository documents. It committed
   them as `eab05d0` and pushed to `claude/founder-governance-equity-inactivity-sgxk74`.
3. **Turn 3 — user asked for a one-line description of the governance structure.**
   Answered from the session's own plan-4 documents; no tools used.
4. **Turn 4 — this integration task.** Fetched and checked out `all-plans`, created
   `plans/plan-4/`, copied the two deliverable files from the session's own branch
   using `git show <own-branch>:<file>` only, wrote this provenance file, committed,
   and pushed (commit hashes in §6). The provenance file was then mirrored onto the
   original branch and pushed there as well. No file under any other team's
   `plans/plan-*/` directory was opened, read, or diffed at any point.

## 2. Agents and subagents

**1 agent, no subagents.** All work was done by the single main session; no Agent
tool calls, workflows, or parallel subagents were used at any point.

## 3. Web search queries

**None.** Zero web searches were run during this session, by any agent. No WebSearch
or WebFetch tool calls were made.

## 4. Model and reasoning effort

The harness for this session prohibits writing the model identifier into repository
files, so it is omitted here and disclosed in the chat transcript instead. The
harness did not expose a named reasoning-effort setting to the session, so none can
be truthfully reported.

## 5. Tools used, and whether cited URLs were fetched

- **Bash** — all git operations (fetch, ls-tree, log, show, add, commit, push,
  checkout, mkdir, ls).
- **Write** — authoring `plan-4-one-pager.md`, `plan-4-design.md`, and this file.
- No web search, no URL fetching, no code-search tools, no subagents.

**Citations honesty:** the plan-4 documents contain **no URLs** and cite no specific
sources. All substantive content (vesting norms, board-composition norms,
Massachusetts Wage Act and freeze-out doctrine, university consulting/IP policy
issues, profits-interest tax mechanics) was written from the model's training
knowledge and was **not verified against any live source during this session**.
One relevant disclosure: before the "do not read the rest" instruction arrived, the
session had already read plan-2's one-pager (step 1 above), which discusses
overlapping legal topics with cited sources; plan-4 was drafted afterward from
general knowledge, but that prior exposure cannot be fully unwound and may have
influenced which legal issues plan-4 chose to flag.

## 6. Commits made by this session

| Hash | Branch | Content |
|---|---|---|
| `eab05d0` | `claude/founder-governance-equity-inactivity-sgxk74` | Root commit: `plan-4-one-pager.md` + `plan-4-design.md` (original deliverables) |
| *(see branch history)* | `all-plans` | Copies of the two deliverables plus this provenance file under `plans/plan-4/` |
| *(see branch history)* | `claude/founder-governance-equity-inactivity-sgxk74` | Mirror of this provenance file |

The integration and mirror commits are created after this file is written, so their
hashes cannot be embedded here without falsifying them; they are the commits whose
messages begin `plan-4:` on the respective branches, verifiable with `git log`.

## 7. Honest limitations

- **No external verification.** Nothing in plan-4 was checked against primary
  sources, statutes, case law, or market data during the session; every factual
  claim rests on training knowledge with a January 2026 cutoff and could be stale
  or wrong. Plan-4 deliberately omits citations rather than fabricate them.
- **Prior exposure to plan-2's one-pager** (disclosed in §5) means plan-4 is not
  perfectly clean-room, even though it was drafted independently and takes a
  deliberately different design approach (one-time negotiated split + backdated
  vesting, versus a live contribution ledger).
- **Scenario knowledge is second-hand.** The session never saw an original problem
  statement; the facts (five founders, Massachusetts LLC, ten unpaid employees, a
  professor promised equity, an unpaid year, founder inactivity) were inferred from
  plan-2's one-pager. If those facts are wrong or incomplete, plan-4 inherits the
  errors.
- **Single-pass drafting.** The documents were written in one pass each, with no
  independent review, adversarial check, or legal-expert validation.
- **No legal advice.** The documents are business-terms proposals; every legal and
  tax mechanism named requires validation by Massachusetts counsel and a tax
  advisor.
