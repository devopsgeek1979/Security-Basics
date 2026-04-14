# DevSecOps Mock Interview Q&A

## Round Snapshot

- Focus: secure pipelines, supply chain, and release governance
- Best answer style: automation-first and risk-based
- What interviewers look for: practical controls that developers will actually use

> Tip: Show how security can move fast without becoming a blocker.

## 1 What is DevSecOps in one minute

DevSecOps integrates security controls into the software lifecycle so security is continuous, automated, and shared across development, operations, and security teams.

## 2 Which security checks belong in CI pipeline

- SAST
- Dependency vulnerability scan
- Secret scan
- IaC scan
- Container image scan
- License checks
- Policy gate on critical findings

## 3 How do you manage vulnerable dependencies

Track SBOM, enforce version pinning, automate dependency updates, block critical vulnerabilities, and prioritize fixes by exploitability and runtime exposure.

## 4 What is shift-left security practically

Design threat modeling, secure coding standards, and automated pre-merge checks so vulnerabilities are prevented earlier and cheaper.

## 5 What is shift-right security practically

Runtime monitoring, anomaly detection, canary analysis, and incident feedback loops to improve preventive controls upstream.

## 6 How do you secure Terraform pipelines

Use IaC scanning, policy-as-code, module allowlists, remote state encryption, state access restrictions, and mandatory reviews for privileged changes.

## 7 What is artifact signing and why needed

It verifies build provenance and integrity so only trusted artifacts are deployed. It protects against supply-chain tampering.

## 8 How do you prevent secret leaks in repositories

Use pre-commit and CI secret scanners, enforce push protection, educate developers, and rotate exposed secrets immediately.

## 9 How do you design security gates without slowing teams

Block only critical exploitable issues, auto-create remediation tickets for lower severities, and provide actionable developer feedback with fix guidance.

## 10 Explain SAST vs DAST quickly

SAST analyzes source code before runtime. DAST tests running application behavior externally. Both are complementary.

## 11 What is policy-as-code

Security and compliance rules are defined in code and automatically enforced during infrastructure and application deployments.

## 12 How do you secure containers

- Use minimal base images
- Run as non-root users
- Enable image signing
- Scan for vulnerabilities
- Apply runtime restrictions
- Patch regularly

## 13 How do you handle a critical finding on release day

Assess exploitability and exposure, apply emergency patch or mitigation, block release if necessary, communicate impact clearly, and document risk decision if exception is granted.

## 14 What metrics prove DevSecOps maturity

Critical vulnerability aging, scan coverage, mean remediation time, escaped defects in production, and policy exception trend.

## 15 How does threat modeling help developers

It gives developers a map of likely attack paths and prioritized controls before coding, reducing rework and security debt.

## 16 How do you secure CI runners

Use ephemeral runners, least privilege identities, strict network egress, signed pipeline definitions, and hardened base images.

## 17 What is secure release evidence

- Code review proof
- Test results
- Scan outputs
- Approval records
- Artifact signature
- Deployment audit records
