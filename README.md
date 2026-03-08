# SOC-Home-Lab
This project demonstrates a Security Operations Center (SOC) home lab built using Splunk to monitor and investigate security events.

## Lab Environment

Virtual machines were created using VirtualBox.

Kali Linux (Attacker)
        |
        |
Windows 10 (Target)
        |
        |
Ubuntu Server + Splunk (SIEM)

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
2. Malware detection using EICAR test file

## Detection

Logs from Windows were forwarded to Splunk where they were analyzed to detect suspicious activity such as:

- Multiple failed login attempts
- Malware detection alerts
- PowerShell execution events

## Screenshots

Screenshots of the dashboards and alerts are located in the screenshots folder.

## Incident Reports

Incident analysis reports are located in the incident-reports folder.
