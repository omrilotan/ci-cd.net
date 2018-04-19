# git/user

## If missing, configure git user

<!--email_off-->
```sh
curl ci-cd.net/v1/git/user | sh -s CI-CD ci-cd@gmail.com
```
<!--/email_off-->

### Arguments
**No arguments** - Use user from last commit

| # | Role | Default | Optionality
| --- | --- | --- | ---
| 1 | name | last commit's user name | Optional
| 2 | email | last commit's user email | Optional

