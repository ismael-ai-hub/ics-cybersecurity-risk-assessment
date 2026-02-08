# System Overview (Simulated ICS Environment)

## Scenario
This project simulates a medium-size critical infrastructure operator (e.g., energy utility or industrial facility)
with an Industrial Control System (ICS) environment used to monitor and control physical processes.

The goal is to document a realistic cybersecurity risk assessment approach for ICS/OT environments.

## High-Level Architecture (IT / OT)

### IT Zone (Business Network)
- Corporate users (email, office applications)
- Identity services (e.g., directory services)
- Business applications (e.g., ERP)
- Remote access services (VPN / jump services)

### Industrial DMZ (IDMZ)
- Historians / data brokers (OT-to-IT data transfer)
- Patch staging services (controlled)
- Jump server / bastion host
- Limited monitoring and log forwarding

### OT Zone (Industrial Network)
- SCADA servers
- HMI stations (operator interfaces)
- Engineering workstation (configuration/programming)
- PLCs / RTUs / controllers
- Industrial switches and segmented VLANs

## Assumptions
- OT network is segmented from IT (with necessary data flows through IDMZ)
- Remote access exists for maintenance and vendors
- OT systems have limited patch windows and legacy constraints

## Security Objectives (ICS Priorities)
1. **Availability**: prevent downtime and disruption of operations
2. **Safety**: avoid unsafe states impacting people or equipment
3. **Integrity**: ensure trusted commands, configurations, and process values
4. **Confidentiality**: important but secondary in most OT environments
