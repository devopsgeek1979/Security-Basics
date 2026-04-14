# 08. DevSecOps Basics

## Table of Contents

- [What is DevSecOps?](#what-is-devsecops)
- [Security in CI-CD Pipeline](#security-in-ci-cd-pipeline)
- [Shift-Left + Shift-Right](#shift-left--shift-right)
- [Real-World Controls](#real-world-controls)

## What is DevSecOps?

DevSecOps integrates security into development and operations workflows from day one.

## Security in CI-CD Pipeline

- Pre-commit: secret scanning, linting
- Build: SAST, dependency checks, IaC scanning
- Test: DAST/API security tests
- Release: policy gates and approvals
- Runtime: monitoring, alerting, incident response

## Shift-Left + Shift-Right

- **Shift-Left:** Catch issues earlier in design and coding.
- **Shift-Right:** Observe and defend in production.

## Real-World Controls

- Use signed artifacts and provenance
- Enforce branch protections and code reviews
- Store secrets in vault, not in repository
- Auto-create tickets for critical findings
- Define severity-based deployment blocking
