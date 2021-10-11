# GitHub Actions Tests
In this repository we test how different workflows are triggered.

## Test 1: Branch `master`, on push
* [Workflow](https://github.com/mikaelkundert/github-actions-tests/runs/3856205216) was performed after pushing directly to `master`

## Test 2: Branch `feature/first`, on push
* [Workflow](https://github.com/mikaelkundert/github-actions-tests/actions/runs/1327924510) was performed after pushing `feature/first` to `origin`

## Test 3: Branch `feature/second`, on push
* [Workflow](https://github.com/mikaelkundert/github-actions-tests/actions/runs/1327937478) was performed after pushing `feature/second` to `origin`
* No other workflows were performed

## Test 4: Branch `master`, on pull request
* Pushing to `feature/master-pull-request` did not trigger workflow
* Creating pull request to `feature/first` did not trigger workflow
* Creating pull request against `master` [did trigger workflow](https://github.com/mikaelkundert/github-actions-tests/actions/runs/1327955979)
  * Note: After this workflow was executed, green checkmark appeared to commits in both pull requests
## Test 5: Branch `feature/**`, on push
