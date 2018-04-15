---
title: git/update
description: Commit changes if there are any changes to commit
toc: true
---

<img width="624" alt="image" src="https://user-images.githubusercontent.com/516342/37645734-5cad4f7e-2c30-11e8-99ee-5d4462ee606b.png">

> Commit changes if there are any changes to commit. Then commit them upstream. This requires the environment holds push privileges, and a user has been configured (see [git/user](#gituser))

### Arguments
**No arguments** - Use a random commit message from [whatthecommit.com](https://whatthecommit.com/)

| Argument | Role | Default
| --- | --- | ---
| @ | commit message | random commit message

> #### Example
> `curl ci-cd.net/v1/git/update | sh -s Automated commit from CI`
