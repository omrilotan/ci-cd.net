# aws/cp
## Upload files to AWS S3
Upload file structure to S3 (recursive). Uses awscli (via pip)
Your environment **must include** AWS access keys for this operation (`AWS_ACCESS_KEY_ID` `AWS_SECRET_ACCESS_KEY`)

### Arguments

| Argument | Role | Default
| --- | --- | ---
| 1 | _mandatory_, source file/directory | none
| 2 | _mandatory_, AWS bucket destination | none
| 3 | _optional_, Exclude pattern | none

#### Example
> `curl ci-cd.net/v1/aws/cp | sh -s docs/ s3://docs.website.com/ *.log`
