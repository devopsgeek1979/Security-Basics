# 03. Web Security and OWASP Basics

## Table of Contents

- [OWASP Top Risks (Interview Focus)](#owasp-top-risks-interview-focus)
- [High-Value Attacks to Know](#high-value-attacks-to-know)
- [SQL Injection](#sql-injection)
- [Cross-Site Scripting (XSS)](#cross-site-scripting-xss)
- [CSRF](#csrf)
- [Secure SDLC Basics](#secure-sdlc-basics)

## OWASP Top Risks (Interview Focus)

- Broken access control
- Cryptographic failures
- Injection
- Insecure design
- Security misconfiguration
- Vulnerable and outdated components
- Identification and authentication failures
- Software and data integrity failures
- Security logging and monitoring failures
- Server-side request forgery (SSRF)

## High-Value Attacks to Know

### SQL Injection

- **Cause:** Unsanitized user input in SQL query.
- **Impact:** Data exfiltration, auth bypass, data tampering.
- **Prevention:** Parameterized queries, ORM safety, least DB privilege.

### Cross-Site Scripting (XSS)

- **Cause:** Untrusted script rendered in browser.
- **Impact:** Session hijack, phishing overlays, account takeover.
- **Prevention:** Output encoding, CSP, input validation.

### CSRF

- **Cause:** Browser sends authenticated request unintentionally.
- **Prevention:** CSRF tokens, SameSite cookies, re-auth for critical actions.

## Secure SDLC Basics

- Threat modeling in design phase
- SAST/DAST and dependency scans in CI
- Security test cases in QA
- Secrets management and key rotation
- Security sign-off before production release
