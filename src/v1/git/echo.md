# git/echo

## Echos a file's content right from a repository.
[`source`](https://github.com/omrilotan/ci-cd.net/blob/main/src/v1/git/echo)

The script parses through bash so, environment variables or shell snippets will get parsed.

<!--email_off-->
```sh
curl ci-cd.net/v1/git/echo | bash -s git@github.com:user/repo.git templates/my-template-file > template-output.txt
```
<!--/email_off-->

### Arguments

| # | Role | Default | Optionality
| --- | --- | --- | ---
| 1 | repository | none | Mandatory
| 2 | remote file | none | Mandatory

### Example

**Template file**
```sh
[default]
aws_access_key_id = ${AWS_SECRET}
aws_secret_access_key = ${AWS_SECRET}
```

**CI script**
```sh
  - mkdir -p ~/.aws
  - curl ci-cd.net/v1/git/echo | sh -s git@github.com:user/repo.git templates/aws_cred > ~/.aws/credentials
```
