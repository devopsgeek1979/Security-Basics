# 02. Network and Web Interview Q&A

## Table of Contents

- [What This Round Tests](#what-this-round-tests)
- [Q1 Explain SQL injection and one mitigation strategy](#q1-explain-sql-injection-and-one-mitigation-strategy)
- [Q2 Explain XSS and how CSP helps](#q2-explain-xss-and-how-csp-helps)
- [Q3 Difference between IDS and IPS](#q3-difference-between-ids-and-ips)
- [Q4 What is SSRF and why is it dangerous](#q4-what-is-ssrf-and-why-is-it-dangerous)
- [Q5 Web app under attack with high 500 errors What first](#q5-web-app-under-attack-with-high-500-errors-what-first)

## What This Round Tests

- Network security basics
- Application-layer attack understanding
- Incident response prioritization

> Tip: Mention both the attack and at least one prevention control.

## Q1 Explain SQL injection and one mitigation strategy

**Answer:**

SQL injection happens when user input is directly concatenated into SQL queries, allowing attackers to execute unintended database commands.

Primary mitigation is parameterized queries or prepared statements.

Additional controls include:

- Least database privilege
- Input validation
- WAF signatures

## Q2 Explain XSS and how CSP helps

**Answer:**

XSS injects malicious script into browser-rendered pages. CSP reduces risk by restricting allowed script sources and blocking risky inline script execution patterns.

## Q3 Difference between IDS and IPS

**Answer:**

- IDS detects suspicious traffic and raises alerts.
- IPS sits inline and can block suspicious traffic in real time.

In mature environments, both are often used with SIEM correlation.

## Q4 What is SSRF and why is it dangerous

**Answer:**

SSRF tricks a server into making requests to internal or private resources. It can expose metadata services, internal APIs, and secrets.

Good mitigations include:

- Strict outbound allowlists
- Strong URL validation
- Metadata access hardening

## Q5 Web app under attack with high 500 errors What first

**Answer:**

1. Check observability dashboards for error rate, latency, and saturation.
2. Correlate findings with WAF and reverse proxy logs.
3. Enable emergency rate limiting and block abusive patterns.
4. Roll back the latest risky deployment if needed.
5. Start an incident bridge and track the timeline.
