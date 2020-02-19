# AWS AMI for CSYE6225

## Install Packer

[Packer] (https://github.com/hashicorp/packer)
[Packer Download] (https://packer.io/downloads.html)

## Validate Template

`packer validate ubuntu-ami.json`

## Build AMI

`packer build \
    -var 'aws_access_key=REDACTED' \
    -var 'aws_secret_key=REDACTED' \
    -var 'aws_region=REDACTED' \
    -var 'subnet_id=REDACTED' \
    ubuntu-ami.json`

