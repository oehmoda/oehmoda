# plan5 — Branch & Isolation Note (read first)

1. **Isolation compliance.** This work was produced on an empty orphan branch created
   immediately at session start (`git checkout --orphan` + `git rm -rf .`). At no point
   did this team read, checkout, diff, fetch, or browse any other branch or any file from
   one. The only cross-branch information ever observed was the **list of remote ref
   names** (via `git ls-remote`, names only, no content), and only at push time.

2. **Why this branch is named `claude/plan5-llc-governance-equity-j5kmc7` and not
   `plan-5`.** When pushing, we discovered a `plan-5` branch already exists on the
   remote (alongside `plan-1` and `plan-2`). We could not verify whose work it contains
   without reading it — which the isolation rule forbids — and force-pushing over it
   could have irreversibly destroyed another team's submission. We therefore pushed to
   this session's explicitly designated branch, which carries the plan5 name. Nothing on
   the pre-existing `plan-5` branch was read, modified, or overwritten. The reviewer
   should treat **this branch** as team plan5's submission (or verify ownership of the
   remote `plan-5` and move this content there).

3. **Deliverables on this branch:**
   - `plan-5-one-pager.md` — research summary
   - `plan-5-design.md` — full framework + rationale + worked example
   - `plan-5-operating-agreement.md` — article-by-article business-terms draft
   - `plan-5-references.md` — annotated bibliography with evidence-strength ratings
