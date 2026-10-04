# Home SOC Lab: Security Monitoring, Threat Detection & Incident Investigation

## Project Goal

The goal of this project is to design, build, and document a practical home Security Operations Center (SOC) lab to develop hands-on skills in security monitoring, threat detection, log analysis, and incident investigation.

The lab will simulate controlled security events in an isolated virtual environment. Security logs and alerts will be collected and analyzed using a Security Information and Event Management (SIEM) platform. The project will focus on understanding how attacks generate observable activity, how security tools detect suspicious behavior, and how an analyst investigates and documents potential incidents.

### Key Objectives

- Build a virtual cybersecurity lab using VirtualBox.
- Deploy Wazuh as the central SIEM and security monitoring platform.
- Configure endpoint monitoring and collect relevant security logs.
- Generate safe, controlled security events for testing.
- Create and validate detection use cases for suspicious activity.
- Investigate alerts and map relevant techniques to the MITRE ATT&CK framework.
- Document incident investigations, detection logic, findings, and recommendations.
- Publish the lab architecture, configuration, and investigation reports on GitHub.


### Data Flow

1. **Generate activity:** Perform controlled security tests from Kali Linux against designated lab systems.
2. **Collect telemetry:** Monitored endpoints record relevant system and security events.
3. **Forward logs:** Wazuh agents send endpoint telemetry to the Wazuh server.
4. **Detect suspicious behavior:** Wazuh analyzes incoming events and generates alerts based on configured detection rules.
5. **Investigate:** Review alerts, examine event details, and identify the likely cause and impact.
6. **Document:** Record investigation steps, evidence, detection results, and recommended remediation.

### Planned Detection Use Cases

- Repeated failed login attempts.
- Suspicious process execution.
- Unusual network scanning activity.
- Changes to important system files.
- Potentially suspicious PowerShell activity.

Each use case will be tested in the lab, and its detection results and limitations will be documented.

## Security and Isolation

- Keep testing activity within the lab's authorized virtual environment.
- Use isolated virtual networking for security testing.
- Avoid exposing vulnerable lab systems or services to the public internet.
- Take VM snapshots before significant configuration changes.
- Do not store passwords, API keys, private logs, or sensitive personal information in the public repository.

## Project Deliverables

- Documented lab architecture and setup instructions.
- Working Wazuh SIEM deployment.
- Endpoint log collection and monitoring configuration.
- Tested detection use cases and supporting evidence.
- Incident investigation reports.
- Screenshots of relevant dashboards and alerts.
- Lessons learned, limitations, and future improvements.

## Project Status

**Current phase:** Initial setup

**Completed:**
- Kali Linux virtual machine downloaded.

**In progress:**
- VirtualBox VM configuration.
- Lab network design.
- Wazuh deployment.

**Planned next steps:**
- Configure the lab network.
- Deploy Wazuh.
- Connect and monitor a test endpoint.
- Generate and investigate the first security events.
