# 01. Fundamentals Interview Q&A

## Table of Contents

- [What This Round Tests](#what-this-round-tests)
- [Q1 What is the CIA triad Give a practical example](#q1-what-is-the-cia-triad-give-a-practical-example)
- [Q2 Difference between threat, vulnerability, and risk](#q2-difference-between-threat-vulnerability-and-risk)
- [Q3 What is defense in depth](#q3-what-is-defense-in-depth)
- [Q4 What is least privilege and why is it critical](#q4-what-is-least-privilege-and-why-is-it-critical)
- [Q5 How do you respond to a phishing incident](#q5-how-do-you-respond-to-a-phishing-incident)

## What This Round Tests

- Core security concepts
- Real-world explanation ability
- Clear communication under time pressure

> Tip: Keep answers simple, practical, and example-driven.

## Q1 What is the CIA triad Give a practical example

**Answer:**

CIA stands for Confidentiality, Integrity, and Availability.

- Confidentiality ensures only authorized users can access data.
- Integrity ensures data remains accurate and unaltered.
- Availability ensures services are accessible when needed.

Example: In online banking, account details must stay private, transaction amounts must not be tampered with, and the app must remain available during peak traffic.

## Q2 Difference between threat, vulnerability, and risk

**Answer:**

- Threat is a potential attacker or harmful event.
- Vulnerability is a weakness in a system or process.
- Risk is the potential business impact if a threat exploits a vulnerability.

Quick explanation: Risk is approximately likelihood multiplied by impact.

## Q3 What is defense in depth

**Answer:**

Defense in depth means implementing multiple layers of security so that if one control fails, others still provide protection.

Examples include:

- Endpoint protection
- Network segmentation
- IAM controls
- Logging and SIEM
- Backup and recovery

## Q4 What is least privilege and why is it critical

**Answer:**

Least privilege gives users and services only the permissions required for their role. It reduces the blast radius from account compromise and insider misuse.

Operationally, I implement it through:

- Role templates
- Temporary elevation
- Periodic access reviews
- Alerts on privilege escalation

## Q5 How do you respond to a phishing incident

**Answer real-time style:**

1. Contain by isolating the affected account or device.
2. Eradicate by resetting credentials and revoking active sessions or tokens.
3. Investigate mail logs, endpoint events, and suspicious lateral movement.
4. Recover safely and monitor for recurrence.
5. Improve controls with user awareness training and phishing-resistant MFA.
