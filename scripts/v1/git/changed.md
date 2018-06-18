# git/changed

## Check if a file was changed in the last commit, returns "yes" or "no"
[`source`](https://github.com/omrilotan/ci-cd.net/blob/master/scripts/v1/git/changed)

```sh
[ $(curl ci-cd.net/v1/git/changed | bash -s .version) == "yes" ] && echo "Version was changed"
```

### Arguments

| # | Role | Default | Optionality
| --- | --- | --- | ---
| 1 | file name | none | Mandatory

> Git compares the complete file names, so, for example the file "pkg/program.go" will only match the string `"pkg/program.go"` (`"./pkg/program.go"` and `"program.go"` will not match)
