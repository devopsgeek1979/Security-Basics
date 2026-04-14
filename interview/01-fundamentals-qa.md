# 01. Fundamentals Interview Q&A

## Q1 What is the CIA triad Give a practical example

**Answer:**

CIA stands for Confidentiality, Integrity, and Availability.

- Confidentiality ensures only authorized users can access data.
- Integrity ensures data is accurate and unaltered.
- Availability ensures services are accessible when needed.

Example: In online banking, account details must be private (C), transaction amounts must not be tampered (I), and app access must remain available during peak traffic (A).

## Q2: Difference between threat, vulnerability, and risk?

**Answer:**

- Threat is a potential attacker/event.
- Vulnerability is weakness.
- Risk is potential impact if threat exploits the weakness.

Formula style explanation: Risk is approximately likelihood multiplied by impact.

## Q3: What is defense in depth?

**Answer:**

Defense in depth means implementing multiple layers of security, so if one control fails, others still protect the system.

Example layers: endpoint protection, network segmentation, IAM controls, logging/SIEM, backup and recovery.

## Q4: What is least privilege and why is it critical?

**Answer:**

Least privilege gives users/services only permissions needed for their job. It reduces blast radius from account compromise and insider misuse.

Operationally, I implement it via role templates, temporary elevation, periodic access reviews, and alerts on privilege escalation.

## Q5: How do you respond to a phishing incident?

**Answer (real-time style):**

1. Contain: isolate affected account/device.
2. Eradicate: reset credentials, revoke sessions/tokens.
3. Investigate: review mail logs, endpoint events, and suspicious lateral movement.
4. Recover: restore trust, monitor for recurrence.
5. Improve: user awareness training and phishing-resistant MFA.
