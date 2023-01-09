# gh/add-pr

## Create a Pull Request on GitHub
[`source`](https://github.com/omrilotan/ci-cd.net/blob/master/scripts/v1/gh/add-pr)

*Bundle*: Add, commit and create pull request. (For OR only use `/v1/gh/pr`)

```sh
curl ci-cd.net/v1/gh/add-pr | bash -s ee977806d7286510da8b9a7492ba58e2484c0ecc
```

### Arguments

| # | Role | Default | Optionality
| --- | --- | --- | ---
| 1 | GitHub API token | none | Mandatory
| 2 | Message | Random commit message by WhatTheCommit (where applicable) | Optional
