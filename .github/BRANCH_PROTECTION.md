# Branch protection setup

After pushing this workflow, enable branch protection
on the main branch in GitHub:

Settings → Branches → Add rule → Branch name: main

Required checks:
- [x] Require status checks to pass before merging
- [x] Require branches to be up to date
- Status check name: "Lint, typecheck, and build"
- [x] Require pull request reviews before merging
- [x] Do not allow bypassing the above settings

This ensures no direct commits to main and every PR
must pass CI before merge.
