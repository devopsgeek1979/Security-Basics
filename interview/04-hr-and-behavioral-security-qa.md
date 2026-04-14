# 04. HR and Behavioral Security Q&A

## Q1 Tell me about a security issue you handled

**Strong structure:** Situation, Task, Action, Result.

**Sample answer:**

In a release cycle, I found a hardcoded API key in a test config. I blocked deployment, rotated the key, moved secrets to a vault, and added pre-commit secret scanning. Result was zero repeat incidents in later releases.

## Q2 How do you balance security and delivery speed

**Sample answer:**

I avoid manual gatekeeping where possible and automate security checks in CI/CD. Critical findings block releases, medium findings create tracked remediation tasks, and low findings are risk-accepted with review.

## Q3 How do you stay updated in security

**Sample answer:**

I follow OWASP, CISA advisories, cloud provider bulletins, and security engineering channels. I also do weekly lab practice and summarize learnings for my team.

## Q4 If team resists security controls what do you do

**Sample answer:**

I align controls with business impact, show practical incidents, and propose developer-friendly automation. My goal is to reduce friction while improving baseline security posture.
