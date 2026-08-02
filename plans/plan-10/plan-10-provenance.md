# plan-10 — Provenance Report

Written 2026-08-02 by the plan-10 integration session. This report distinguishes
between **two separate sessions**, because they were different agent instances
with no shared memory:

- **Session A (authoring)** — the session that produced the plan-10 deliverable,
  committed 2026-08-02 09:04:23 UTC as orphan commit `9ed8bb8` on branch
  `claude/llc-governance-equity-design-10j7h7`.
- **Session B (integration, this session)** — a fresh session started 2026-08-02
  on branch `claude/llc-governance-equity-design-n0nzpb`, tasked only with
  migrating plan-10's work into `all-plans` and writing this report. Session B
  has **no memory of Session A** and reconstructed everything about it from git
  metadata only.

## What Session B (this session) did, step by step, in order

1. Ran `git branch -a` / `git ls-remote origin` to see the repository state.
   Found orphan branches `plan-1`, `plan-2`, `plan-5`, `plan-9`, `plan-review`,
   the shared `all-plans` branch, and several `claude/*` session branches. No
   `plan-10` ref existed on the remote.
2. Identified its own team: the session branch name stem
   `llc-governance-equity-design` exactly matches
   `claude/llc-governance-equity-design-10j7h7`, whose single orphan commit is
   titled `plan10: draft article-by-article operating agreement business terms`
   and contains one file, `plan-10-operating-agreement.md`. Therefore N=10.
3. To rule out ambiguity, inspected **commit metadata only** (hashes, authors,
   dates, subjects, and file *names* via `git log` / `git ls-tree`) of the other
   plan branches, mapping plan-1 → `claude/startup-governance-equity-8webj5`,
   plan-4 → `claude/founder-governance-equity-inactivity-sgxk74`,
   plan-5 → `claude/plan5-llc-governance-equity-*`. **No file contents of any
   other team's branch or `plans/plan-*` directory were opened, read, or
   diffed.**
4. Read the shared `README.md` on `all-plans` (top-level, not inside any team's
   directory) to confirm the integration rules.
5. Read plan-10's own deliverable (`git show 9ed8bb8:plan-10-operating-agreement.md`).
6. Created local ref `plan-10` pointing at `9ed8bb8` (the authoring session had
   pushed its orphan commit under its session branch name but never created the
   `plan-10` ref; creating the ref changes no content).
7. `git checkout -B all-plans origin/all-plans`, `mkdir -p plans/plan-10`, and
   copied the deliverable with `git show plan-10:plan-10-operating-agreement.md`;
   verified the copy byte-identical with `diff`.
8. Wrote this provenance file.
9. Committed `plans/plan-10/` on `all-plans` and pushed with the prescribed
   fetch–rebase retry loop.
10. Mirrored this provenance file onto branch `plan-10` (as a child commit of
    `9ed8bb8`, leaving the original commit intact) and pushed `plan-10`.

## What is known about Session A (authoring)

Known only from git records: it committed `9ed8bb8` (orphan, no parent) on
2026-08-02 09:04:23 UTC containing `plan-10-operating-agreement.md` — a 225-line
article-by-article business-terms term sheet for a five-founder Massachusetts
LLC operating agreement (contribution-ledger pool, founder reserve, advisor
settlement, crystallization, appraisal, Wage Act flags). Session A's internal
process — its searches, tools, subagents, and reasoning effort — left no record
in the repository and **cannot be truthfully reported here**. Session A appears
not to have completed a full deliverable set (no design doc, one-pager, or
references file was committed, unlike some other teams).

## Agents / subagents

- Session B: **1 agent, no subagents.**
- Session A: 1 agent session as far as git shows (single author "Claude
  <noreply@anthropic.com>", single commit); whether it used subagents is
  unknown.

## Web search queries, verbatim, in execution order

- Session B: **none.** Zero web searches and zero web fetches were run during
  integration.
- Session A: unknown — not recoverable, and not invented here. Note that the
  deliverable's citations (e.g., M.G.L. ch. 156C, the Massachusetts Wage Act)
  were therefore **not verified by fetching any URL in this session**.

## Model and reasoning effort

The harness for this session prohibits writing the model identifier into
repository files, so it is disclosed in the accompanying chat message instead,
as this task's instructions permit. The reasoning-effort setting is not exposed
to the session by the harness and is therefore not stated; no effort override
was requested by the user.

## Tools used (Session B)

- `git` via the Bash tool (ls-remote, fetch, log, ls-tree, show, branch,
  checkout, diff, add, commit, push, rebase) — the only substantive tool.
- File Read/Write tools for authoring this report.
- **No** web search, web fetch, GitHub API tools, or subagents were used. No
  cited URL was fetched; nothing was even seen in search results, since no
  searches were run.

## Commits

| Hash | Branch | Content |
|---|---|---|
| `9ed8bb8` | `claude/llc-governance-equity-design-10j7h7` (now also ref `plan-10`) | Session A's orphan commit: `plan-10-operating-agreement.md` |
| (this commit — a commit cannot embed its own hash; see `git log origin/all-plans`) | `all-plans` | `plans/plan-10/plan-10-operating-agreement.md` (byte-identical copy) + this provenance file |
| (see `git log origin/plan-10`) | `plan-10` | Mirror of this provenance file, child of `9ed8bb8` |

## Honest limitations

- The integration agent (Session B) is not the author of the deliverable and
  cannot vouch for Session A's research process, search queries, or source
  verification; anything not in git is reported as unknown rather than
  reconstructed.
- Team identity (N=10) was inferred from the exact branch-name stem match and
  the `plan10:` commit subject; no other team's branch shares that stem, and no
  other unclaimed plan number matches, but the inference is circumstantial
  rather than declared by the task message, which referred generically to
  "plan-{N}".
- The plan-10 deliverable set is a single document (the operating-agreement term
  sheet); it lacks the companion design/one-pager/references documents some
  other teams produced. This report does not pad or embellish that fact.
- The legal citations inside the deliverable were not re-verified during
  integration.
