# git/run

## Run shell scripts right from a repository

```sh
curl ci-cd.net/v1/git/run | sh git@github.com:user/repo.git scripts/function.sh arg1 arg2
```

### Arguments

| # | Role | Default | Optionality
| --- | --- | --- | ---
| 1 | repository | none | Mandatory
| 2 | script | none | Mandatory
| @ | rest of the arguments are chained | none | Optional