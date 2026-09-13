# Wazuh Lab Deployment

A documented security monitoring lab built in VMware Workstation. The project shows how I prepared an isolated environment, installed Wazuh on Ubuntu Server, enrolled a Windows Server 2022 endpoint, and prepared Kali Linux for controlled testing.

## What is documented

| Component | Role | Evidence |
|---|---|---|
| Ubuntu Server | Wazuh Manager, Indexer, and Dashboard | Installation steps and service checks |
| Windows Server 2022 | Monitored endpoint | Agent installation and active status check |
| Kali Linux | Controlled test machine | VM import and network setup |
| VMware Workstation | Virtual lab platform | VM and network configuration |

This repository covers **deployment and connectivity**. Detection rules, attack simulations, and incident investigations are future work; they are not presented here as completed results.

## Read the lab

Follow the guides in order:

1. [Lab overview](Lab/01-Lab_Overview.md)
2. [Install VMware Workstation](Lab/02-install-vmware.md)
3. [Create the Ubuntu VM](Lab/03-Create-Ubuntu-VM.md)
4. [Install Ubuntu Server](Lab/04-VM-Ubuntu-Configuration.md)
5. [Configure the lab networks](Lab/05-Configuration-Ubuntu-Before-Install-Wazuh.md)
6. [Install Wazuh All-in-One](Lab/06-Wazuh-Installation.md)
7. [Install Windows Server 2022](Lab/07-Windows_Server_2022.md)
8. [Install the Wazuh Agent](Lab/08-Installing-the-Wazuh-Agent-on-Windows-Server.md)
9. [Install Kali Linux](Lab/09-Install-Kali-Linux.md)

## Validation points

The guides show how to check that the three Wazuh services are running, that the Dashboard is reachable, and that the Windows agent appears as **Active**. Kali Linux is prepared for subsequent controlled tests on the isolated lab network. Screenshots support the deployment steps; they are not a substitute for reproducing the checks in a new environment.

## Next phase

I plan to add endpoint telemetry, a first detection with test events, alert evidence, investigation notes, and a concise incident report. Each future case study will distinguish the test procedure from the observed result.

## Security note

The IP addresses and commands in the guides are lab examples. Generate your own credentials, keep installer password archives private, and never commit passwords or screenshots containing them. Restrict testing to systems you own or are authorized to assess.

## Author

**Geovanny Argueta** — SOC Analyst Level 2
