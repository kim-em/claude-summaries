---
source_path: /Users/kim/.ec2
generated: 2025-12-01T18:50:00Z
git_sha: 629fb3cc99de1db687a986ca5547ddff189dce8a
git_branch: master
status: complete
files_count: 13
subdirs_count: 0
---

# .ec2

## Overview

AWS EC2 credentials and SSL certificates directory containing access keys, private keys (.pem), and PuTTY keys (.ppk) for various EC2 instances. The files date from September 2023 and include keys for instances named "counterexample", "fusionatlas", "mathoverflow", and various "default" instances across different AWS regions (Ireland, Oregon). The `access` file stores AWS access key IDs and secret access keys in CSV format.

## Key Files

| File | Purpose |
|------|---------|
| `access` | CSV file containing AWS access key IDs and secret access keys for default and fusionatlas accounts |
| `counterexample.pem` | SSH private key for EC2 instance named "counterexample" |
| `counterexample.ppk` | PuTTY private key format for counterexample instance |
| `default.pem` | Default SSH private key for EC2 instances |
| `default.ppk` | Default PuTTY private key |
| `default-ireland.pem` | SSH private key for EC2 instance in Ireland region |
| `default-oregen.pem` | SSH private key for EC2 instance in Oregon region (note: filename typo "oregen" instead of "oregon") |
| `fusionatlas.pem` | SSH private key for EC2 instance named "fusionatlas" |
| `mathoverflow.pem` | SSH private key for EC2 instance named "mathoverflow" |
| `cert-QSLWRHBHDNEPRZ7XX4GYPVNDEIQVAFSF.pem` | SSL certificate with identifier QSLWRHBHDNEPRZ7XX4GYPVNDEIQVAFSF |
| `pk-QSLWRHBHDNEPRZ7XX4GYPVNDEIQVAFSF.pem` | Private key corresponding to the above SSL certificate |

## Subdirectories

None.

## Search Tags

aws ec2 credentials ssh-keys private-keys pem ppk certificates ssl access-keys fusionatlas counterexample mathoverflow cloud-infrastructure security
