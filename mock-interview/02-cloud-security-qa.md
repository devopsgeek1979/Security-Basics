# Cloud Security Mock Interview Q&A

## 1 Explain cloud shared responsibility with example

Provider secures physical infrastructure and managed service foundations, while customer secures identities, data, configurations, and workload permissions. Example: provider secures hypervisor, customer secures object storage bucket policies.

## 2 What is cloud posture management

Cloud posture management continuously evaluates cloud resources against security best practices and compliance rules to detect and remediate misconfigurations.

## 3 How do you secure object storage

Block public access by default, use least-privilege bucket policies, enable encryption, enforce versioning, enable access logs, and monitor anomalous data egress.

## 4 What is identity federation and why useful

Federation allows enterprise identity providers to grant cloud access without separate long-term cloud users. It improves lifecycle control and central auditability.

## 5 How do you protect cloud secrets

Use managed secret stores, automatic rotation, short-lived credentials, strict access policies, and usage audit alerts.

## 6 What is a dangerous IAM anti-pattern

Over-broad wildcard permissions granted for convenience such as full admin access to service roles. This increases privilege abuse risk and blast radius.

## 7 How do you detect crypto-mining in cloud

Look for sudden compute spikes, unusual outbound traffic, unexpected process execution on instances, and anomalous billing trends. Confirm with runtime telemetry.

## 8 Explain network segmentation in cloud

Use VPC/VNet segmentation, private subnets, restrictive security groups, network ACLs, and service endpoints to limit lateral movement.

## 9 How do you secure Kubernetes in cloud

Use least-privilege service accounts, restrict API server access, enforce admission policies, scan images, limit pod privileges, and monitor runtime behavior.

## 10 What should cloud incident response start with

Contain exposure quickly, snapshot evidence safely, preserve audit logs, rotate keys, isolate compromised resources, and open a structured incident timeline.

## 11 How do you enforce compliance continuously

Apply policy-as-code, scheduled and event-driven scans, deployment gates, drift detection, and auto-remediation where safe.

## 12 What is data exfiltration risk in cloud

Unauthorized transfer of sensitive data outside trusted boundaries. Mitigate with DLP controls, egress restrictions, encryption, anomaly detection, and strict key controls.

## 13 How do you secure serverless workloads

Minimize function permissions, validate inputs, protect secrets, apply dependency scanning, enforce network controls, and monitor invocation anomalies.

## 14 Explain cloud key management basics

Use managed KMS, separate key admin and data admin roles, rotate keys by policy, and log every key usage event.

## 15 What do you do after accidental public database exposure

Remove public access, assess data exposure window, rotate credentials, review query logs for unauthorized access, notify stakeholders, and implement preventive policy controls.

## 16 How would you secure multi-account architecture

Separate workloads by environment and business unit, use centralized identity, enforce guardrails via org policies, and centralize logging/security monitoring.

## 17 What is cloud threat modeling

It identifies assets, trust boundaries, attack paths, and mitigations for cloud architecture before deployment.
