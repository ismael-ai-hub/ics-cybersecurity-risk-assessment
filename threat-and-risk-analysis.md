# Threat and Risk Analysis

## Purpose
This section identifies realistic cybersecurity threats and risk scenarios
affecting the simulated ICS/OT environment. The analysis follows a risk-based
approach aligned with industrial cybersecurity practices.

---

## Threat Sources
Common threat sources relevant to industrial environments include:

- External attackers targeting critical infrastructure
- Ransomware groups pivoting from IT to OT
- Insider threats (intentional or accidental)
- Third-party vendors and contractors
- Supply chain compromises

---

## Common Attack Paths (Examples)

### 1. IT Network Compromise → OT Environment
- Initial compromise of IT systems (phishing, malware)
- Lateral movement toward the Industrial DMZ
- Unauthorized access to OT systems

### 2. Remote Access Abuse
- Compromised VPN or jump server credentials
- Excessive vendor privileges
- Lack of monitoring of remote sessions

### 3. Engineering Workstation Compromise
- Malware infection or credential theft
- Unauthorized PLC logic modification
- Persistent access to OT environment

### 4. Weak Network Segmentation
- Flat OT network architecture
- Lack of strict access controls between zones
- Rapid propagation of malware or unauthorized access

---

## Risk Scenarios

### Risk 1 — Unauthorized Remote Access to OT Systems
- **Description**: Attacker gains access through compromised remote access.
- **Impact**: Loss of control, operational disruption, safety risks.
- **Likelihood**: Medium
- **Severity**: High
- **Overall Risk**: High

### Risk 2 — PLC Logic Manipulation
- **Description**: Unauthorized modification of control logic.
- **Impact**: Unsafe process behavior, equipment damage.
- **Likelihood**: Low to Medium
- **Severity**: Very High
- **Overall Risk**: High

### Risk 3 — Ransomware Propagation from IT to OT
- **Description**: Ransomware spreads due to insufficient segmentation.
- **Impact**: Loss of visibility, downtime, recovery challenges.
- **Likelihood**: Medium
- **Severity**: High
- **Overall Risk**: High

### Risk 4 — Lack of OT Monitoring and Detection
- **Description**: Security incidents go undetected for extended periods.
- **Impact**: Increased dwell time and damage.
- **Likelihood**: High
- **Severity**: Medium
- **Overall Risk**: Medium to High

---

## High-Level Mapping to ATT&CK (Conceptual)
- Initial Access: Valid Accounts, Phishing
- Lateral Movement: Remote Services
- Persistence: Scheduled Tasks, Services
- Impact: Loss of Control, Denial of Service
