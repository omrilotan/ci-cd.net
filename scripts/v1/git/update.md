# git/update

## Commit changes if there are any changes to commit
Then commit them upstream.
[`[source]`](https://github.com/omrilotan/ci-cd.net/blob/master/scripts/v1/git/update)

```sh
curl ci-cd.net/v1/git/update | bash -s All your codebase are belong to us
```

<img width="624" alt="image" src="https://user-images.githubusercontent.com/516342/37645734-5cad4f7e-2c30-11e8-99ee-5d4462ee606b.png">

### Arguments
**No arguments** - Use a random commit message from [whatthecommit.com](https://whatthecommit.com/)

| # | Role | Default | Optionality
| --- | --- | --- | ---
| @ | commit message | random commit message | Optional

> This operation requires the environment holds push privileges, and a user has been configured (see [git/user](#gituser))
