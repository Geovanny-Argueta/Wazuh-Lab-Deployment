# Lab Overview

## Objective

I built this lab to practice security monitoring in an environment I could control from end to end. The goal is not only to install Wazuh, but also to understand how logs move from an endpoint to the SIEM, how alerts are generated, and how an analyst can investigate the activity.

This first part of the project focuses on building the infrastructure. Later phases will use the same environment to simulate attacks, create detection rules, validate alerts, and document incidents from a SOC perspective.

## Lab Scope

The current environment includes:

- **Wazuh Server:** Ubuntu Server running the Wazuh Manager, Indexer, and Dashboard
- **Windows Server 2022:** Monitored endpoint with the Wazuh Agent
- **Kali Linux:** Testing machine used to generate controlled activity
- **VMware Workstation:** Virtualization platform used to run and isolate the lab

## How the Lab Works

1. VMware Workstation runs the virtual machines.
2. Ubuntu Server hosts the Wazuh platform.
3. Windows Server sends security events to the Wazuh Manager.
4. Kali Linux generates controlled activity for future detection tests.
5. Wazuh analyzes the events and makes the alerts available for investigation in the Dashboard.

## Documentation

Follow the guides in this order:

1. **Lab Overview** — Current section
2. [Install VMware Workstation](02-install-vmware.md)
3. [Create the Ubuntu Virtual Machine](03-Create-Ubuntu-VM.md)
4. [Install Ubuntu Server](04-VM-Ubuntu-Configuration.md)
5. [Configure the VMware Lab Networks](05-Configuration-Ubuntu-Before-Install-Wazuh.md)
6. [Install Wazuh All-in-One](06-Wazuh-Installation.md)
7. [Install Windows Server 2022](07-Windows_Server_2022.md)
8. [Install the Wazuh Agent on Windows Server](08-Installing-the-Wazuh-Agent-on-Windows-Server.md)
9. [Install Kali Linux](09-Install-Kali-Linux.md)

## Expected Result

After completing this deployment phase, the lab should have:

- A working Wazuh All-in-One server
- Access to the Wazuh Dashboard
- An active Windows Server agent
- A Kali Linux machine ready for controlled testing
- An isolated environment that can support future Detection Engineering use cases

## Next Phase

The next phase will add more endpoint telemetry and document the first complete detection use case, from attack simulation to alert investigation and response.
