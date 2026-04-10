# Create Ubuntu Virtual Machine

## Objective
The objective of this step is to create the virtual machine that will host the Wazuh server in the lab environment.

This virtual machine will be prepared in VMware Workstation and configured with the resources required for a small all-in-one Wazuh lab.

## **Steps**
## 🖥️ Ubuntu Server Installation for Wazuh Lab

The first step is to install the operating system. We will use **Ubuntu Server 22.04 LTS**, as it is a stable and compatible option for our **Wazuh All-in-One** lab (Manager, Indexer, and Dashboard).

---

### 1. Download Ubuntu Server

Go to the following link and download the ISO image:

👉 https://ubuntu.com/download/server

---

### 2. Create a New Virtual Machine

Open **VMware**, then go to:

**File → New Virtual Machine**

---

### 3. Initial Setup

The setup wizard will appear.  
(The interface may vary depending on your VMware version, but the process is the same.)

---

### 4. Configuration Type

Select:

**Typical (recommended)**

Then click **Next**.

---

### 5. Select ISO Image

Choose:

**Installer disc image file (ISO)**

Then select the Ubuntu ISO you downloaded.

---

### 6. Virtual Machine Name

Assign a name to your virtual machine, for example:

```bash
Wazuh_Lab
