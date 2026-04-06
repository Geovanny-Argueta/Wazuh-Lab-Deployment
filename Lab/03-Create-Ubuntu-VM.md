# Create Ubuntu Virtual Machine

## Objective
The objective of this step is to create the virtual machine that will host the Wazuh server in the lab environment.

This virtual machine will be prepared in VMware Workstation and configured with the resources required for a small all-in-one Wazuh lab.

## Virtual Machine Configuration
The virtual machine will be created with Ubuntu Server as the operating system.

Recommended lab settings:
- **Guest operating system:** Linux
- **Version:** Ubuntu 64-bit
- **vCPU:** 4
- **RAM:** 8 GB
- **Disk:** 50 GB
- **Network adapter:** NAT or Bridged

## Creation Steps
1. Open VMware Workstation.
2. Click **Create a New Virtual Machine**.
3. Select **Typical (recommended)** and click **Next**.
4. Choose **Installer disc image file (iso)**.
5. Browse and select the Ubuntu Server ISO file.
6. Click **Next**.
7. Select **Linux** as the guest operating system.
8. Select **Ubuntu 64-bit** as the version.
9. Click **Next**.
10. Enter a name for the virtual machine, such as **Wazuh-Server**.
11. Choose the location where the virtual machine will be stored.
12. Click **Next**.
13. Set the disk size to **50 GB**.
14. Select **Store virtual disk as a single file**.
15. Click **Next**.
16. Click **Customize Hardware**.
17. Set the memory to **8 GB**.
18. Set the processors to **4 vCPU**.
19. Verify that the network adapter is configured as **NAT** or **Bridged**.
20. Confirm that the Ubuntu ISO is attached to the virtual CD/DVD drive.
21. Click **Close**.
22. Click **Finish** to create the virtual machine.

## Expected Result
At the end of this step, the Ubuntu virtual machine should be created in VMware Workstation and ready for the operating system installation.

## Evidence
Take screenshots of:
- the new virtual machine wizard
- the hardware configuration
- the final virtual machine summary
