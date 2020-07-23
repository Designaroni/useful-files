# AWS CLI goodies 

### Flags

  - `--dryrun`: 
    - ex: `$ aws s3 sync s3://bucket-name.aws-bucket-url.com/theme_assets/siteId12345 ./siteId12345/ --dryrun`

### Credentials

---

### Profiles

A [default] profile is used when you run a CLI command with no profile. A secondary or specific profile can be used when you run a CLI command with the `--profile user1` parameter.

  - `--profile`:
    - ex: `$ aws s3 sync --profile ian.roberts --dryrun`

