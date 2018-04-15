---
title: gh/pages
description: Commit a file or directory to gh-pages branch
toc: true
---

> commit a file or directory to gh-pages branch

### Arguments

| Argument | Role | Default
| --- | --- | ---
| 1 | _mandatory_, source | none
| 2 | _optional_, commit message | a random commit message from [whatthecommit.com](https://whatthecommit.com/)

#### Example
Create documentation, push to gh-pages
> ```sh
> npx jsdoc docs/ -c .jsdocrc.json
> curl ci-cd.net/v1/gh/pages | sh -s docs/.
> ```

