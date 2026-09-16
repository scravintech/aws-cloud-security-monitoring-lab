# aws-cloud-security-monitoring-lab
Hands-on cloud security lab deploying EC2, centralized auditing via CloudTrail/CloudWatch, automated threat detection with GuardDuty, and security aggregation in Security Hub.

# Cloud Security Monitoring & Threat Detection Lab (AWS)

## Overview
A foundational cloud security and monitoring lab built to simulate enterprise-grade threat detection, auditing, and posture management in AWS. 

## Architecture & Tech Stack
* **Compute Target:** Amazon EC2 (Linux Server)
* **Auditing & Logging:** AWS CloudTrail & Amazon CloudWatch (Account-wide API call tracking & system logs)
* **Threat Detection:** Amazon GuardDuty (Automated threat detection and anomaly analysis)
* **Centralized Dashboard:** AWS Security Hub (Single pane of glass for security posture and findings)

## Implementation Steps
1. **Provisioned Compute:** Deployed an Amazon EC2 instance to serve as the baseline cloud resource.
2. **Configured Auditing:** Set up a multi-region CloudTrail management events trail linked to an S3 log archive and CloudWatch log groups.
3. **Enabled Threat Intelligence:** Activated Amazon GuardDuty to continuously monitor AWS API activity and network traffic patterns.
4. **Centralized Security Posture:** Configured AWS Security Hub to aggregate findings, compliance checks, and alerts.

## Key Findings & Triage
During validation, GuardDuty successfully identified and flagged simulated security telemetry:
* **Root Credential Usage Alerts:** Detected API calls (`GetPolicy`, `ListOrganizationAdminAccounts`) invoked using root-level credentials during setup, proving the efficacy of continuous behavioral monitoring.

## Resume Impact
Demonstrates practical competency in CompTIA Security+ Domain 4 (Security Operations / Monitoring) and foundational AWS Cloud Security engineering.
