# Asset Identification

## Purpose
This section identifies and classifies critical assets within the simulated
ICS/OT environment. Asset identification is a key step in cybersecurity
risk assessment and decision-making for industrial systems.

---

## OT Critical Assets

### PLCs / RTUs / Industrial Controllers
- **Description**: Devices responsible for direct control of physical processes.
- **Security Impact**: Loss of control, unsafe states, equipment damage.
- **Criticality**: Very High (availability and safety).

### SCADA Servers
- **Description**: Centralized supervisory systems for monitoring and control.
- **Security Impact**: Loss of visibility, delayed response, operational disruption.
- **Criticality**: High.

### HMI Stations
- **Description**: Operator interfaces used to monitor and control processes.
- **Security Impact**: Incorrect decisions, unauthorized commands.
- **Criticality**: High.

### Engineering Workstation
- **Description**: Used for configuration and programming of PLC logic.
- **Security Impact**: Unauthorized logic changes, persistent compromise.
- **Criticality**: Very High (integrity).

### Historian / OT Data Systems
- **Description**: Collect and store operational data for reporting and analysis.
- **Security Impact**: Data manipulation, loss of historical visibility.
- **Criticality**: Medium to High.

---

## Supporting IT Assets (Relevant to OT Security)

### Remote Access Infrastructure (VPN / Jump Server)
- **Description**: Enables secure access to OT systems for engineers and vendors.
- **Security Impact**: Common attack vector into OT environments.
- **Criticality**: Very High.

### Identity and Access Management Systems
- **Description**: Authentication and authorization services.
- **Security Impact**: Privilege abuse, unauthorized access.
- **Criticality**: High.

### Monitoring and Logging Systems
- **Description**: Provide visibility into security events.
- **Security Impact**: Delayed detection and response.
- **Criticality**: Medium.

---

## Asset Constraints (ICS Context)
- Long asset lifecycles and legacy systems
- Limited patching windows
- Compatibility constraints with security tools
- High availability and safety requirements
