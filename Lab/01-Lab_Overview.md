# Lab Overview

## Objective

The objective of this lab is to build a practical Wazuh SIEM environment for cybersecurity monitoring, detection, and analysis, this lab is not only focused on installing Wazuh. The main purpose is to create a portfolio-ready environment where I can document SIEM use cases, simulate security events, validate detections, and analyze alerts from a SOC perspective.

## Lab Scope

This lab includes the deployment and preparation of the following systems:

- **Wazuh Server** running on Ubuntu Server
- **Windows Server** monitored with the Wazuh Agent
- **Kali Linux** used for testing, traffic generation, and future pentesting scenarios
- **VMware Workstation** as the virtualization platform

## High-Level Architecture

1. VMware Workstation runs the virtual lab.
2. Ubuntu Server hosts the Wazuh platform.
3. Windows Server is connected as a monitored endpoint.
4. Kali Linux is used to generate activity for future SIEM use cases.
5. Wazuh collects logs, detects events, and provides alerts for analysis.

## Lab Documentation Steps

Follow the lab documentation in order:

1. **Lab Overview**  
   Current section.

2. [Install VMware Workstation](02-install-vmware.md)

3. [Create Ubuntu Virtual Machine](03-Create-Ubuntu-VM.md)

4. [Ubuntu VM Configuration](04-VM-Ubuntu-Configuration.md)

5. [Configure Ubuntu Before Installing Wazuh](05-Configuration-Ubuntu-Before-Install-Wazuh.md)

6. [Install Wazuh All-in-One](06-Wazuh-Installation.md)

7. [Install Windows Server 2022](07-Windows_Server_2022.md)

8. [Install Wazuh Agent on Windows Server](08-Installing-the-Wazuh-Agent-on-Windows-Server.md)

9. [Install Kali Linux](09-Install-Kali-Linux.md)

## Expected Outcome

At the end of this deployment phase, the lab should have:

- A working Wazuh server
- Access to the Wazuh Dashboard
- A Windows Server endpoint connected to Wazuh
- A Kali Linux machine ready for testing
- A base environment prepared for future SIEM use cases

## Next Phase

The next phase of this project will focus on documenting SIEM use cases, detection logic, alert analysis, and practical SOC investigation workflows.
