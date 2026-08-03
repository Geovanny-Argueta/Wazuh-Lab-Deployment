# Wazuh Lab Deployment

## Overview

This repository documents the Wazuh lab I built in VMware Workstation. I started this project to move beyond theory and create a small SOC environment where I can collect logs, generate security events, test detections, and investigate alerts.

The lab is still growing. This repository covers the infrastructure and deployment process, while the next phase will focus on Detection Engineering and practical SIEM use cases.

## Lab Environment

| System | Purpose |
|---|---|
| **Ubuntu Server** | Hosts the Wazuh Manager, Indexer, and Dashboard |
| **Windows Server 2022** | First monitored endpoint with the Wazuh Agent |
| **Kali Linux** | Generates controlled activity for detection testing |
| **VMware Workstation** | Runs and isolates the virtual machines |

## What This Project Covers

- Building an isolated virtual lab
- Deploying Wazuh All-in-One
- Connecting a Windows endpoint to Wazuh
- Preparing Kali Linux for controlled security testing
- Verifying that agents and Wazuh services are working
- Creating a foundation for future detection and investigation use cases

## Lab Documentation

The deployment is documented step by step, including screenshots and validation checks.

[Start the Lab Documentation](Lab/01-Lab_Overview.md)

## Next Phase

The next phase will add Windows and Linux telemetry, custom Wazuh rules, MITRE ATT&CK mapping, Active Response, dashboards, and incident reports. Each detection will be tested in the lab before it is documented.

## Author

**Geovanny Argueta**  
Cybersecurity Portfolio Project
