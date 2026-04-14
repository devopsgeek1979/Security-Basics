# 07. Cloud Security Basics

## Table of Contents

- [Shared Responsibility Model](#shared-responsibility-model)
- [Core Cloud Security Controls](#core-cloud-security-controls)
- [Common Misconfigurations](#common-misconfigurations)
- [Incident Scenario](#incident-scenario)

## Shared Responsibility Model

- **Cloud provider:** Security *of* the cloud.
- **Customer:** Security *in* the cloud.

## Core Cloud Security Controls

- Least-privilege IAM policies
- Private networking and segmentation
- Encryption at rest and in transit
- Centralized logging and monitoring
- Automated compliance checks

## Common Misconfigurations

- Public object storage buckets
- Open security groups (`0.0.0.0/0` on admin ports)
- Excessive IAM permissions (`*:*` style access)
- Hardcoded credentials in code or pipelines

## Incident Scenario

**Question:** A storage bucket became public. What next?

**Answer approach:**

1. Restrict public access immediately.
2. Review access logs for data exposure window.
3. Classify exposed data sensitivity.
4. Rotate keys/tokens possibly exposed.
5. Raise incident, communicate, and document RCA.
6. Add preventive guardrails (policy-as-code).
