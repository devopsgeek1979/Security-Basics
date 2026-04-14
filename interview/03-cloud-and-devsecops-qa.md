# 03. Cloud and DevSecOps Interview Q&A

## What This Round Tests

- Cloud security fundamentals
- Secure delivery thinking
- Response to secret and key exposure

> Tip: Tie every answer to risk reduction, automation, and accountability.

## Q1 Explain cloud shared responsibility model

**Answer:**

The cloud provider secures the underlying infrastructure, while the customer secures workloads, data, identities, configurations, and access controls.

Interview tip: mention that this varies by SaaS, PaaS, and IaaS service depth.

## Q2 How do you secure secrets in CI/CD

**Answer:**

- Store secrets in a vault or managed secret manager.
- Inject secrets at runtime and never hardcode them.
- Rotate secrets automatically.
- Audit access and usage events.

## Q3 What checks would you add to a pipeline before deployment

**Answer:**

I would add:

- SAST
- Dependency scanning or SCA
- IaC scanning
- Container image scanning
- Policy gates for critical findings
- Artifact signing and provenance validation

## Q4 Public cloud key leaked in repository What now

**Answer real-time:**

1. Revoke the compromised key immediately.
2. Rotate dependent credentials and tokens.
3. Investigate logs for suspicious usage during the exposure window.
4. Contain affected resources and accounts.
5. Raise the incident and communicate with stakeholders.
6. Add pre-commit and CI secret scanning controls.

## Q5 How would you prioritize vulnerabilities in production

**Answer:**

I combine CVSS with exploit maturity, internet exposure, business criticality, and compensating controls, then map the result to remediation SLAs and clear owner accountability.
