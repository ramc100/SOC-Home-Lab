# SOC-Home-Lab
This project demonstrates a Security Operations Center (SOC) home lab built using Splunk to monitor and investigate security events.

## Lab Environment

Virtual machines were created using VirtualBox.

Machines used:

- Kali Linux (attacker)
- Windows 10 (target)
- Ubuntu Server running Splunk (SIEM)

## Tools Used

- Splunk Enterprise
- Kali Linux
- Windows Event Logs
- Hydra (brute force testing)

## Simulated Attacks

1. Brute force login attack
Framework: MITRE ATT&CK
Detection Source: Windows Security Logs (Event ID 4625)
Tool Used: Splunk SIEM

2. Malware detection using EICAR test file
Incident Name: Brute Force Login Attack
MITRE ATT&CK Technique:
T1110 – Brute Force

Description:
Multiple failed login attempts were detected targeting a Windows host from a Kali Linux attacker machine.

Detection Method:
Splunk SIEM query monitoring Windows Security Event Logs.

Relevant Logs:
Event ID 4625 – Failed Logon Attempt

Indicators of Compromise:
Repeated authentication failures from a single IP address.

Mitigation:
Account lockout policies recommended after 5 failed login attempts.

## Detection

Logs from Windows were forwarded to Splunk where they were analyzed to detect suspicious activity such as:

- Multiple failed login attempts
- Malware detection alerts
- PowerShell execution events

## Screenshots

Screenshots of the dashboards and alerts are located in the screenshots folder.

## Incident Reports

Incident analysis reports are located in the incident-reports folder.
