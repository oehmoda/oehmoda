# all-plans — Integration Branch for Independent Plan Teams

This branch collects the deliverables of all independent plan teams in one place
**without collisions and without breaking team isolation**.

## Structure

```
plans/
  plan-1/   ← team plan1's deliverables, exactly as on branch plan-1
  plan-2/
  ...
  plan-10/
```

## Rules for every team/agent

1. **Write only inside your own directory** `plans/plan-{N}/`. Never create,
   edit, or delete anything outside it (except nothing — the README is maintained
   by the repo owner).
2. **Never open, read, or diff** any file under another team's `plans/plan-*/`
   directory, and never checkout or browse another team's branch. Copy your files
   from your own branch using `git show plan-{N}:<file>` only.
3. **Keep your original `plan-{N}` branch intact** — this branch is a copy
   destination, not a replacement.
4. **Push with a rebase-retry loop** (see below). Because every team touches a
   disjoint directory, rebases always apply cleanly; the loop only handles the
   race of two teams pushing at the same moment.
5. **Do not open pull requests** for this branch.

## Standard migration commands

```bash
N=<your number>
git fetch origin all-plans
git checkout -B all-plans origin/all-plans
mkdir -p plans/plan-$N
for f in $(git ls-tree --name-only plan-$N); do git show plan-$N:"$f" > plans/plan-$N/"$f"; done
git add plans/plan-$N
git commit -m "plan-$N: add deliverables under plans/plan-$N/"
for i in 1 2 3 4 5; do
  git push origin all-plans && break
  sleep $((2**i)); git fetch origin all-plans && git rebase origin/all-plans
done
```
