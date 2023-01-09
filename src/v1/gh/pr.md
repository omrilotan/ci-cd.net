# gh/pr

## Create a Pull Request on GitHub
[`source`](https://github.com/omrilotan/ci-cd.net/blob/master/scripts/v1/gh/pr)

Uses last commit message to create pull request title and description

```sh
curl ci-cd.net/v1/gh/pr | bash -s ee977806d7286510da8b9a7492ba58e2484c0ecc
```

### Arguments

| # | Role | Default | Optionality
| --- | --- | --- | ---
| 1 | GitHub API token | none | Mandatory
