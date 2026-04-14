# 02. Network and Web Interview Q&A

## Q1 Explain SQL injection and one mitigation strategy

**Answer:**

SQL injection happens when user input is directly concatenated into SQL queries, allowing attackers to execute unintended database commands.

Primary mitigation is parameterized queries (prepared statements). Additional controls include least DB privilege and WAF signatures.

## Q2 Explain XSS and how CSP helps

**Answer:**

XSS injects malicious script into browser-rendered pages. CSP (Content Security Policy) reduces risk by restricting allowed script sources and blocking inline script execution patterns.

## Q3 Difference between IDS and IPS

**Answer:**

- IDS detects suspicious traffic and alerts.
- IPS sits inline and can block suspicious traffic in real time.

In mature environments, both are used with SIEM correlation.

## Q4 What is SSRF and why is it dangerous

**Answer:**

SSRF tricks a server into making requests to internal/private resources. It can expose metadata services, internal APIs, and secrets.

Mitigation: strict outbound allowlists, URL validation, metadata access hardening.

## Q5 Web app under attack with high 500 errors What first

**Answer:**

1. Check observability dashboards (error rate, latency, saturation).
2. Correlate with WAF/reverse proxy logs.
3. Enable emergency rate limiting and block abusive patterns.
4. Roll back latest risky deployment if needed.
5. Start incident bridge and track timeline.
