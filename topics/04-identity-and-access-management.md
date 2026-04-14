# 04. Identity and Access Management (IAM)

## Table of Contents

- [Core Terms](#core-terms)
- [IAM Building Blocks](#iam-building-blocks)
- [Best Practices](#best-practices)
- [Interview Scenario](#interview-scenario)

## Core Terms

- **Authentication (AuthN):** Who are you?
- **Authorization (AuthZ):** What can you do?
- **Accounting/Auditing:** What did you do?

## IAM Building Blocks

- User lifecycle management (joiner/mover/leaver)
- Role-Based Access Control (RBAC)
- Attribute-Based Access Control (ABAC)
- Single Sign-On (SSO)
- Multi-Factor Authentication (MFA)

## Best Practices

- Enforce MFA for privileged and remote access
- Use short-lived credentials where possible
- Review access rights quarterly
- Remove dormant accounts automatically
- Separate admin and normal user accounts

## Interview Scenario

**Question:** A developer left the company. What IAM actions are critical in first 24 hours?

**Good answer:**

1. Disable identity provider account immediately.
2. Revoke cloud/API/SSH keys and active sessions.
3. Rotate shared secrets the user had access to.
4. Transfer ownership of repositories and services.
5. Review logs for suspicious post-notice activity.
