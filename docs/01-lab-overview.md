# Lab Overview

## Objective
The objective of this lab is to deploy a functional Wazuh environment in a virtualized setup and document the full installation process step by step.

This lab is designed to demonstrate practical skills in virtualization, Linux server preparation, Wazuh deployment, agent onboarding, and validation.

## Lab Scope
This repository covers the initial deployment phase of the lab, including:
- VMware Workstation installation
- Ubuntu virtual machine creation
- Wazuh installation
- Initial dashboard access
- Agent installation
- Basic validation steps

## Lab Environment
The lab will be built using the following components:

- **Host system:** Windows
- **Virtualization platform:** VMware Workstation
- **Wazuh server:** Ubuntu Linux virtual machine
- **Monitored systems:** Windows and Linux endpoints with Wazuh agents

## High-Level Architecture
The environment follows a simple architecture:

1. A Windows host runs VMware Workstation.
2. An Ubuntu virtual machine is created inside VMware.
3. Wazuh is installed on the Ubuntu VM.
4. Additional endpoints are connected to Wazuh as agents.
5. Logs and events are sent from the agents to the Wazuh server for monitoring.

## Why This Lab Matters
This lab helps demonstrate hands-on experience in:
- Building a cybersecurity lab
- Deploying a SIEM solution
- Preparing systems for monitoring
- Connecting endpoints to a central platform
- Validating that monitoring works correctly

## Expected Outcome
At the end of this lab, the environment should:
- Have a working Wazuh installation
- Allow access to the Wazuh dashboard
- Show connected agents
- Receive basic logs and security events

## Next Steps
The next phase of this project is the installation of VMware Workstation and preparation of the virtual environment.
