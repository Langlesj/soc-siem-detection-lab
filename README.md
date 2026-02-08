SOC SIEM Detection Lab
Overview

This project simulates a real Security Operations Center (SOC) monitoring workflow using log ingestion, alert detection, and incident triage techniques.

The objective is to demonstrate hands-on defensive cybersecurity skills aligned with:

MITRE ATT&CK

NIST Cybersecurity Framework

Enterprise SOC investigation procedures

Lab Objectives

Ingest and analyze security and system logs

Detect suspicious or malicious behavior

Triage alerts using SOC investigation methodology

Document containment and remediation actions

Build repeatable detection logic for continuous monitoring

Environment

SIEM Platform: Wazuh / Splunk / Elastic (lab environment)
Endpoints: Windows and Linux virtual machines

Primary Log Sources:

Windows Event Logs

Sysmon telemetry

Authentication activity

Network connection logs

Tools Utilized:
Python · PowerShell · Sysmon · SIEM dashboards

Simulated Threat Scenarios

This lab investigates common real-world attack behaviors, including:

Brute-force authentication attempts

Suspicious PowerShell execution

Malware or ransomware indicators

Unauthorized privilege escalation

Lateral movement between hosts

Each scenario follows a true SOC lifecycle from detection through containment.

Detection & Analysis Workflow

Log Collection
Security telemetry is forwarded into the SIEM.

Alert Generation
Detection rules trigger on suspicious behavioral patterns.

Alert Validation
Determine whether activity is a true positive or benign.

Investigation
Analyze:

Source IP address

Impacted host system

User account behavior

Event timeline

Threat Mapping
Map activity to relevant MITRE ATT&CK techniques.

Containment Actions
Example responses:

Disable compromised account

Isolate affected endpoint

Block malicious IP or file hash

Lessons Learned
Improve detection rules and SOC response playbooks.

Example Detection Case

Scenario: Multiple failed login attempts followed by a successful authentication
Risk: Potential brute-force account compromise

SOC Investigation Steps:

Review authentication event logs

Identify attacking IP address

Check for lateral movement or persistence

Reset credentials and enforce MFA

Document incident timeline and remediation

Mapped MITRE Technique:
T1110 – Brute Force

Skills Demonstrated

SIEM monitoring and log analysis

Security alert triage methodology

Incident investigation workflow

Threat detection aligned with MITRE ATT&CK

Defensive containment planning

Security documentation and reporting

Planned Enhancements

Custom SIEM detection rule creation

Automated alert enrichment using Python

Expanded ransomware behavior simulation

Threat-hunting queries across historical logs

SOC dashboard visualization and reporting

Author

Stephen Langley
SOC Analyst | Cybersecurity Detection & Incident Response

LinkedIn:
https://www.linkedin.com/in/stephenlangley1
