# Create the Ubuntu Virtual Machine

## Objective

This virtual machine will host the complete Wazuh platform: Manager, Indexer, and Dashboard. I assigned enough resources for a small all-in-one deployment while leaving room for logs and future testing.

This lab was originally built with **Ubuntu Server 22.04 LTS**. If you reproduce it with a newer release, check the current Wazuh compatibility list before installing.

## Create the VM

### 1. Download Ubuntu Server

Download the Ubuntu Server ISO from the [official Ubuntu website](https://ubuntu.com/download/server).

![Ubuntu Server download](../Docs/Linux-1.png)

### 2. Start the VMware Wizard

Open VMware Workstation and select:

**File > New Virtual Machine**

Choose **Typical (recommended)** and continue.

![VMware configuration type](../Docs/Linux-2.png)

### 3. Select the ISO

Choose **Installer disc image file (ISO)** and select the Ubuntu Server ISO.

![Ubuntu ISO selection](../Docs/Linux-3.png)

### 4. Name the Virtual Machine

Use a clear lab name, for example:

`Wazuh-Server`

![Virtual machine name](../Docs/Linux-4.png)

### 5. Configure the Disk

Assign an **80 GB** virtual disk and select **Store virtual disk as a single file**.

Fifty gigabytes can work for a basic deployment, but additional space is useful once Wazuh starts storing alerts and endpoint data.

![Virtual disk configuration](../Docs/Linux-8.png)

### 6. Configure the Hardware

Before finishing, review the hardware settings.

| Resource | Recommended | Minimum for this lab |
|---|---:|---:|
| CPU | 4 vCPU | 4 vCPU |
| RAM | 10–12 GB | 8 GB |
| Disk | 80 GB | 50 GB |

I used **4 vCPU, 10 GB of RAM, and an 80 GB disk**.

![Virtual machine memory](../Docs/Linux-5.png)
![Virtual machine hardware](../Docs/Linux-6.png)

### 7. Finish the Setup

Review the settings and select **Finish**. VMware will create the virtual machine and start the Ubuntu installation.

## Expected Result

The VM should boot from the Ubuntu Server ISO and display the installation menu.

---

<p align="center">
  <strong>Lab Navigation</strong>
</p>

<p align="center">
  <a href="02-install-vmware.md">⬅️ Previous: Install VMware Workstation</a>
  &nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="04-VM-Ubuntu-Configuration.md">Next: Install Ubuntu Server ➡️</a>
</p>
