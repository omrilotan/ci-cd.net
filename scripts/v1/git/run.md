# git/run

## Run shell scripts right from a repository

<!--email_off-->
```sh
curl ci-cd.net/v1/git/run | sh -s git@github.com:user/repo.git scripts/function.sh arg1 arg2
```
<!--/email_off-->

### Arguments

| # | Role | Default | Optionality
| --- | --- | --- | ---
| 1 | repository | none | Mandatory
| 2 | script | none | Mandatory
| @ | rest of the arguments are chained | none | Optional

