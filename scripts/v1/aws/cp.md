# aws/cp

## Upload files to AWS S3
[`source`](https://github.com/omrilotan/ci-cd.net/blob/master/scripts/v1/aws/cp)

```sh
curl ci-cd.net/v1/aws/cp | bash -s docs/ s3://docs.website.com/ *.log
```

Upload file structure to S3 (recursive). Uses awscli (via pip).

### Arguments

| # | Role | Default | Optionality
| --- | --- | --- | ---
| 1 | source file/directory | none | Mandatory
| 2 | AWS bucket destination | none | Mandatory
| 3 | Exclude pattern | none | Optional

> Your environment **must include** AWS access keys for this operation (`AWS_ACCESS_KEY_ID` `AWS_SECRET_ACCESS_KEY`)
