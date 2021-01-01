# AWS CLI goodies 

# `$ aws`

## `$ aws s3`

### `$ aws s3 sync`

#### Flags

  - `--dryrun`: 
    - ex: `$ aws s3 sync s3://bucket-name.s3.amazonaws.com/theme_assets/siteId12345 ./siteId12345/ --dryrun`

### `$ aws s3 rm`

#### Flags

  - `--recursive`
    - ex: `aws s3 rm s3://bucket-name.com.s3.amazonaws.com/theme_assets/siteId12345 --recursive --dryrun`

### Credentials

---

### Profiles

A [default] profile is used when you run a CLI command with no profile. A secondary or specific profile can be used when you run a CLI command with the `--profile user1` parameter.

  - `--profile`:
    - ex: `$ aws s3 sync --profile ian.roberts --dryrun`

