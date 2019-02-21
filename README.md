# AWS AMI for CSYE 6225

## Team Information

| Name | NEU ID | Email Address |
| --- | --- | --- |
| Sonia Mahankali| 001476237|mahankali.s@husky.neu.edu|
| Shardul Singh Negi|001898181|negi.s@husky.neu.edu|
| Zhe Liu |001475826|liu.zhe3@husky.neu.edu|
| Xuewen Xu|001434974|xu.xue@husky.neu.edu|

## Validate Template

```
packer validate ubuntu-ami.json
```

## Build AMI

```
packer build \
    -var 'aws_access_key=REDACTED' \
    -var 'aws_secret_key=REDACTED' \
    -var 'aws_region=us-east-1' \
    -var 'subnet_id=REDACTED' \
    ubuntu-ami.json
```
