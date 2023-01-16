# git/cp

## Copy a file right from a repository
[`source`](https://github.com/omrilotan/ci-cd.net/blob/main/src/v1/git/cp)

<!--email_off-->
```sh
curl ci-cd.net/v1/git/cp | bash -s git@github.com:user/repo.git templates/my-template-file.html template.html
```
<!--/email_off-->

### Arguments

| # | Role | Default | Optionality
| --- | --- | --- | ---
| 1 | repository | none | Mandatory
| 2 | remote file | none | Mandatory
| 3 | local name | file's base name | Optional
