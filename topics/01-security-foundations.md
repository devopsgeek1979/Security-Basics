# 01. Security Foundations

## Table of Contents

- [Why Security Matters](#why-security-matters)
- [CIA Triad](#cia-triad)
- [Threat, Vulnerability, Risk](#threat-vulnerability-risk)
- [Security Principles](#security-principles)
- [Common Attack Types](#common-attack-types)
- [Practical Interview Tip](#practical-interview-tip)

## Why Security Matters

Security protects **confidentiality, integrity, and availability** of systems and data.

In business terms, security protects:

- customer trust,
- compliance posture,
- revenue continuity,
- brand reputation.

## CIA Triad

- **Confidentiality:** Only authorized users access data.
  - Controls: encryption, access controls, data classification.
- **Integrity:** Data stays accurate and unmodified.
  - Controls: hashing, checksums, digital signatures, audit logs.
- **Availability:** Systems/data are accessible when required.
  - Controls: redundancy, failover, backups, DDoS protections.

## Threat, Vulnerability, Risk

- **Threat:** Potential cause of harm (attacker, malware, insider).
- **Vulnerability:** Weakness that can be exploited.
- **Risk:** Likelihood × impact of a threat exploiting a vulnerability.

### Example

- Threat: attacker scans internet-facing port.
- Vulnerability: outdated web server with known CVE.
- Risk: remote code execution and data breach.

## Security Principles

- **Least Privilege:** Give minimum permissions needed.
- **Defense in Depth:** Use layered controls.
- **Zero Trust:** Never trust by default; always verify.
- **Need to Know:** Restrict access by role and purpose.
- **Fail Securely:** On failure, deny by default.

## Common Attack Types

- Phishing/social engineering
- Malware/ransomware
- Credential stuffing and brute force
- Web exploits (SQL injection, XSS)
- Misconfiguration abuse (open storage buckets, weak ACLs)

## Practical Interview Tip

When answering, connect concept to operations:

- "I enforce least privilege using role-based access, quarterly access reviews, and break-glass monitoring."
