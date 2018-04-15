# git/user
## If missing, configure git user

### Arguments
**No arguments** - Use user from last commit

| Argument | Role | Default
| --- | --- | ---
| 1 | name | last commit's user name
| 2 | email | last commit's user email

> #### Example
> `curl ci-cd.net/v1/git/user | sh -s CI-CD ci-cd@gmail.com`
