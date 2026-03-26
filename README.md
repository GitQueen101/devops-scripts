# devops-scripts

Python and Bash automation scripts for cloud and DevOps tasks.

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![Bash](https://img.shields.io/badge/Bash-4EAA25?style=flat&logo=gnu-bash&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat&logo=amazon-aws&logoColor=white)

## Overview

A collection of production-quality Python and Bash scripts for automating common DevOps and cloud tasks. Each script is documented, handles errors gracefully, and includes a --help flag.

## Scripts

### AWS Automation
- `aws/ec2_start_stop.py` -- Start or stop EC2 instances by tag
- `aws/s3_cleanup.py` -- Delete S3 objects older than N days
- `aws/iam_audit.py` -- List IAM users and their last activity

### System Automation
- `system/log_rotate.sh` -- Compress and archive old log files
- `system/disk_alert.sh` -- Alert when disk usage exceeds threshold
- `system/service_check.sh` -- Check status of critical services and restart if down

### CI/CD Helpers
- `cicd/tag_release.sh` -- Create and push a semantic version git tag
- `cicd/notify_slack.py` -- Send deployment notifications to Slack

## Tech Stack

- Python 3.11
- Bash
- AWS CLI / boto3
- argparse (CLI argument parsing)

## Usage

Each script supports --help:

```bash
python3 aws/ec2_start_stop.py --help
bash system/disk_alert.sh --help
```

## Code Quality

GitHub Actions runs flake8 on all Python scripts on every push.

---

Part of the [GitQueen101 DevOps portfolio](https://github.com/GitQueen101).
