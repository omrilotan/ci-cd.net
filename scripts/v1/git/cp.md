# git/cp

## Copy a file right from a repository

```sh
curl ci-cd.net/v1/git/cp | sh -s git@github.com:user/repo.git templates/my-template-file.html template.html
```

### Arguments

| # | Role | Default | Optionality
| --- | --- | --- | ---
| 1 | repository | none | Mandatory
| 2 | remote file | none | Mandatory
| 3 | local name | file's base name | Optional
