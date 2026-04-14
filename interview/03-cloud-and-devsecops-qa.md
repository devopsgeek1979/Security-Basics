# 03. Cloud and DevSecOps Interview Q&A

## Q1 Explain cloud shared responsibility model

**Answer:**

Cloud provider secures infrastructure, while customer secures workloads, data, identities, configurations, and access controls.

Interview tip: mention this varies by SaaS/PaaS/IaaS depth.

## Q2 How do you secure secrets in CI/CD

**Answer:**

- Store secrets in vault or managed secret manager.
- Inject secrets at runtime, never hardcode.
- Rotate secrets automatically.
- Audit access and usage events.

## Q3 What checks would you add to pipeline before deploy

**Answer:**

I add SAST, dependency scan (SCA), IaC scan, container image scan, and policy gates for critical findings. I also verify artifact signing and provenance.

## Q4 Public cloud key leaked in repository What now

**Answer (real-time):**

1. Revoke compromised key immediately.
2. Rotate dependent credentials and tokens.
3. Investigate logs for suspicious usage window.
4. Contain affected resources/accounts.
5. Raise incident and communicate stakeholders.
6. Add pre-commit and CI secret scanning controls.

## Q5 How would you prioritize vulnerabilities in production

**Answer:**

I combine CVSS with exploit maturity, internet exposure, business criticality, and compensating controls, then map to remediation SLAs and owner accountability.
