# 💬 04. HR and Behavioral Security Q&A

## Table of Contents

- [What This Round Tests](#what-this-round-tests)
- [Q1 Tell me about a security issue you handled](#q1-tell-me-about-a-security-issue-you-handled)
- [Q2 How do you balance security and delivery speed](#q2-how-do-you-balance-security-and-delivery-speed)
- [Q3 How do you stay updated in security](#q3-how-do-you-stay-updated-in-security)
- [Q4 If team resists security controls what do you do](#q4-if-team-resists-security-controls-what-do-you-do)

## What This Round Tests

- Communication clarity
- Ownership and judgment
- Team collaboration mindset

> Tip: Use short STAR-based answers with a clear result.

## Q1 Tell me about a security issue you handled

**Strong structure:** Situation, Task, Action, Result.

**Sample answer:**

In a release cycle, I found a hardcoded API key in a test configuration. I blocked the deployment, rotated the key, moved secrets to a vault, and added pre-commit secret scanning. The result was zero repeat incidents in later releases.

## Q2 How do you balance security and delivery speed

**Sample answer:**

I avoid manual gatekeeping where possible and automate security checks in CI/CD. Critical findings block releases, medium findings create tracked remediation tasks, and low findings are accepted only after review.

## Q3 How do you stay updated in security

**Sample answer:**

I follow OWASP, CISA advisories, cloud provider bulletins, and security engineering channels. I also practice in labs weekly and summarize key learnings for my team.

## Q4 If team resists security controls what do you do

**Sample answer:**

I align controls with business impact, share practical incident examples, and propose developer-friendly automation. My goal is to reduce friction while improving the baseline security posture.
