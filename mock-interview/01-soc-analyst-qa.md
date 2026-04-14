# 🧭 SOC Analyst Mock Interview Q&A

## Table of Contents

- [Round Snapshot](#round-snapshot)
- [1 How do you triage a high-severity alert](#1-how-do-you-triage-a-high-severity-alert)
- [2 What are false positives and how do you reduce them](#2-what-are-false-positives-and-how-do-you-reduce-them)
- [3 Explain SIEM normalization in simple terms](#3-explain-siem-normalization-in-simple-terms)
- [4 What logs are most important during investigation](#4-what-logs-are-most-important-during-investigation)
- [5 How do you investigate suspicious PowerShell usage](#5-how-do-you-investigate-suspicious-powershell-usage)
- [6 What is MITRE ATT&CK and why does SOC use it](#6-what-is-mitre-attck-and-why-does-soc-use-it)
- [7 Difference between IOC and IOA](#7-difference-between-ioc-and-ioa)
- [8 How do you respond to brute-force login attempts](#8-how-do-you-respond-to-brute-force-login-attempts)
- [9 What should an incident timeline include](#9-what-should-an-incident-timeline-include)
- [10 How do you prioritize multiple simultaneous alerts](#10-how-do-you-prioritize-multiple-simultaneous-alerts)
- [11 What is lateral movement and how detect it](#11-what-is-lateral-movement-and-how-detect-it)
- [12 How would you handle ransomware early signs](#12-how-would-you-handle-ransomware-early-signs)
- [13 What does containment mean in incident response](#13-what-does-containment-mean-in-incident-response)
- [14 What KPIs should a SOC report weekly](#14-what-kpis-should-a-soc-report-weekly)
- [15 How do you validate an endpoint compromise](#15-how-do-you-validate-an-endpoint-compromise)
- [16 What is threat hunting vs alert response](#16-what-is-threat-hunting-vs-alert-response)
- [17 Explain a good escalation note](#17-explain-a-good-escalation-note)
- [18 How do you reduce dwell time](#18-how-do-you-reduce-dwell-time)

## Round Snapshot

- Focus: detection, triage, containment, and escalation
- Best answer style: concise, evidence-based, and time-aware
- What interviewers look for: prioritization and incident judgment

> Tip: Speak like an analyst on shift. Mention evidence, impact, and next action.

## 1 How do you triage a high-severity alert

Start with asset criticality, alert confidence, and blast radius. Validate signal quality from log source, check related indicators, and map to MITRE ATT&CK. If business-critical assets are involved, escalate immediately and begin containment.

## 2 What are false positives and how do you reduce them

False positives are benign events flagged as malicious. Reduce them with tuned detection rules, baseline behavior profiling, allowlists for known-good activities, and feedback loops between SOC and engineering.

## 3 Explain SIEM normalization in simple terms

Normalization converts logs from different sources into a consistent schema so analysts can query, correlate, and alert reliably across products.

## 4 What logs are most important during investigation

- Authentication logs
- Endpoint telemetry
- DNS logs
- Proxy and firewall logs
- Cloud audit trails
- Application logs with identity context

## 5 How do you investigate suspicious PowerShell usage

Identify parent-child process chain, encoded commands, outbound network calls, privilege level, and persistence changes. Correlate with user activity and threat intel indicators before deciding containment scope.

## 6 What is MITRE ATT&CK and why does SOC use it

It is a behavior-based framework of adversary tactics and techniques. SOC uses it to classify detections, find visibility gaps, and communicate attack progression.

## 7 Difference between IOC and IOA

IOC is evidence of compromise like hash or IP. IOA is behavior indicating malicious intent like credential dumping pattern. IOA is generally more resilient than static IOC.

## 8 How do you respond to brute-force login attempts

Enable temporary lockouts, enforce MFA, apply rate limiting, block abusive IP ranges, and review successful logins after failures for possible compromise.

## 9 What should an incident timeline include

- Detection time
- Alert source
- Analyst actions
- Containment milestones
- Communication events
- Business impact
- Recovery confirmation

## 10 How do you prioritize multiple simultaneous alerts

Prioritize by potential impact, confidence, exposed critical assets, and active exploitation signs. Use a severity matrix and assign owners immediately.

## 11 What is lateral movement and how detect it

Lateral movement is attacker spread across systems after initial access. Detect through unusual remote admin activity, credential reuse, abnormal east-west traffic, and privilege escalation patterns.

## 12 How would you handle ransomware early signs

Isolate affected endpoints, disable compromised identities, block command-and-control indicators, protect backups from modification, and activate IR playbook with executive communication.

## 13 What does containment mean in incident response

Containment limits attacker ability to expand damage. It can be short-term like host isolation and long-term like segmentation changes or credential rotation.

## 14 What KPIs should a SOC report weekly

- MTTD
- MTTR
- True-positive rate
- Alert volume by severity
- Incidents by tactic
- Unresolved backlog
- Control improvement actions

## 15 How do you validate an endpoint compromise

Correlate EDR detections, suspicious process tree, persistence artifacts, unusual network destinations, and memory or disk evidence where needed.

## 16 What is threat hunting vs alert response

Alert response is reactive to known detections. Threat hunting is proactive hypothesis-driven search for hidden threats without explicit alert triggers.

## 17 Explain a good escalation note

A strong note includes what happened, affected assets, confidence level, containment actions taken, evidence links, and clear asks from next responder team.

## 18 How do you reduce dwell time

Improve log coverage, tune high-fidelity detections, automate enrichment, shorten triage runbooks, and perform continuous purple-team validation.
