# gh/pages

## Commit a file or directory to gh-pages branch

```sh
npx jsdoc docs/ -c .jsdocrc.json # Create docs for example
curl ci-cd.net/v1/gh/pages | sh -s docs/.
```

### Arguments

| # | Role | Default | Optionality
| --- | --- | --- | ---
| 1 | source | none | Mandatory
| 2 | commit message | a random commit message from [whatthecommit.com](https://whatthecommit.com/) | Optional

