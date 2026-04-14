# 02. Network Security Basics

## Table of Contents

- [Key Concepts](#key-concepts)
- [Network Layers and Threats](#network-layers-and-threats)
- [Common Controls](#common-controls)
- [Incident Scenario](#incident-scenario)

## Key Concepts

- **Firewall:** Filters traffic based on rules.
- **IDS/IPS:** Detects/prevents malicious activity.
- **Segmentation:** Splits networks to limit blast radius.
- **VPN:** Secure tunnel over untrusted network.
- **WAF:** Protects web applications at HTTP layer.

## Network Layers and Threats

- **L3/L4 threats:** port scans, SYN flood, spoofing.
- **L7 threats:** HTTP floods, bot abuse, API misuse.

## Common Controls

- Deny-by-default ingress rules
- Restrict outbound traffic (egress filtering)
- Disable unused ports/services
- Use bastion hosts for admin access
- Enable centralized logging and flow analysis

## Incident Scenario

**Question:** Sudden spike in traffic on port 443. What do you do?

**Answer framework:**

1. Validate if legitimate (release event, campaign, known crawler).
2. Check WAF/CDN/Load balancer telemetry.
3. Identify source patterns (ASN, geo, user-agent anomalies).
4. Apply mitigation (rate limit, bot challenge, block rules).
5. Confirm service health and error rates.
6. Document timeline and preventive actions.
