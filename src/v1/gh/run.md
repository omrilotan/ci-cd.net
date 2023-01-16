# gh/run

## Execute shell scripts from a remote GitHub repository
[`source`](https://github.com/omrilotan/ci-cd.net/blob/main/src/v1/gh/run)

<!--email_off-->
```sh
curl ci-cd.net/v1/gh/run | bash -s user my-repo master scripts/function.sh $GITHUB_API_TOKEN arg1 arg2
```
<!--/email_off-->

### Arguments

| # | Role | Default | Optionality
| --- | --- | --- | ---
| 1 | user | none | Mandatory
| 2 | repo | none | Mandatory
| 3 | branch | none | Mandatory
| 4 | file | none | Mandatory
| 5 | token | none | Mandatory
| @ | rest of the arguments are chained | none | Optional

