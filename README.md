# operator-ci-sandbox

Test repository for CI automation experiments.

## Mergify Backport Flow

The `.mergify.yml` rule automatically cherry-picks merged PRs to release branches
when the appropriate label is applied.

### How to backport a PR

1. Create a PR targeting `main`.
2. Add the label `backport/<release-branch>` (e.g., `backport/release-v1`).
3. Merge the PR into `main`.
4. Mergify automatically creates a new PR cherry-picking the changes onto the
   target release branch.

### Available release branches

- `release-v1`
