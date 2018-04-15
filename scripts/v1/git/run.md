---
title: git/run
description: Run shell scripts right from a repository
toc: true
---

> Run shell scripts from a git repository

### Arguments

| Argument | Role | Default
| --- | --- | ---
| 1 | repository | none
| 2 | script | none
| @ | rest of the arguments are chained | none

> #### Example
> `curl ci-cd.net/v1/git/run | sh git@github.com:user/repo.git scripts/function.sh arg1 arg2`
