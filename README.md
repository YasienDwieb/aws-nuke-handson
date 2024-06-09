## AWS Nuke Handson
AWS Nuke is a tool that can do AWS services discovery and mass deletion of them, which is useful for cleanup and cost leakages fixing.

#### Objectives/Use cases:
- Detect what's already provisioned in your account
- Delete resources in specific regions
- Cleanup after a testing/handson setup


### Usage
> :white_check_mark: Ensure AWS-cli is installed and a profile is configured with admin credentials
1. Install AWS-nuke by downloading proper release file from here: https://github.com/rebuy-de/aws-nuke/releases

2. extract and move binary to PATH detected location
```bash
$ tar -xf aws-nuke-v2.25.0-linux-amd64.tar.gz
$ sudo mv aws-nuke-v2.25.0-linux-amd64 /usr/local/bin/aws-nuke
```

1. Run command in dry-run mode
```bash
$ aws-nuke -c config.yml
```

1. When ready, run in non-dry-run mode :rocket: :rocket: :rocket:
```bash
$ aws-nuke -c config.yml --no-dry-run
```

### Docs
Refer repo for further examples and customizations: [AWS-Nuke repo](https://github.com/rebuy-de/aws-nuke)
