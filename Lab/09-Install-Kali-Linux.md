## Install Kali Linux Virtual Machine

In this section, we will download the official Kali Linux virtual machine image, import it into VMware Workstation, organize the VM files, and start Kali Linux for the first time. This VM will be used later as part of the Wazuh lab environment for security testing, log generation, and cybersecurity practice.

---

### Step 1: Download the Kali Linux Virtual Machine

First, go to the official Kali Linux download page:

https://www.kali.org/get-kali/#kali-platforms

On the download page, select the **Virtual Machines** option, after that, choose the **VMware** image and click **Download**, this option is useful because Kali Linux already provides a prebuilt virtual machine, so we do not need to install the operating system manually from an ISO file.

![step1](../Docs/Install-Kali-Linux/step-1.png)
![step2](../Docs/Install-Kali-Linux/step-2.png)

---

### Step 2: Extract the Downloaded File

Once the Kali Linux VMware file has been downloaded, locate the compressed file on your computer, right-click the file and extract it, wait until the extraction process finishes completely.

After the file is extracted, you should see the Kali Linux virtual machine files, including the VMware configuration file.

![step2](../Docs/Install-Kali-Linux/step-3.png)

---

### Step 3: Move the Kali Linux VM Folder to the Virtual Machines Directory

After extracting the file, I like to keep my lab organized by moving the Kali Linux VM folder to the same location where I store all my other virtual machines, this helps keep the lab structure clean and easy to manage.

You can also rename the extracted folder to something simple, for example: **Kali Linux**, after organizing the folder, open **VMware Workstation**, go to **Home**, and select:

**Open a Virtual Machine**

![step3](../Docs/Install-Kali-Linux/step-4.png)

---

### Step 4: Open the Kali Linux Virtual Machine in VMware

Now browse to the folder where you extracted and saved the Kali Linux VM, select the VMware virtual machine file and click **Open**, this will import the Kali Linux VM into VMware Workstation.

![step4](../Docs/Install-Kali-Linux/step-5.png)

---

### Step 5: Rename the Virtual Machine in VMware

After opening the Kali Linux VM, it should now appear in VMware Workstation, to keep the lab organized, click on the VM name and rename it to: **Kali Linux**, this makes it easier to identify the machine later, especially when working with multiple virtual machines in the Wazuh lab.

![step5](../Docs/Install-Kali-Linux/step-6.png)

---

### Step 6: Review the Virtual Machine Hardware Settings

Before starting the VM, you can review the hardware settings if needed, for example, you can adjust:
- RAM
- CPU
- Disk settings
- Network adapter
In this lab, I will leave the default hardware settings because the Kali Linux VMware image already works well with the recommended configuration.


---

### Step 7: Power On the Kali Linux Virtual Machine

Now power on the Kali Linux virtual machine, wait until the system finishes booting, do not press **Enter** or click anything during the boot process. Just wait until the login screen appears.

Once the login screen is displayed, use the default Kali Linux credentials:
- **Username:** : **kali**
- **Password:** : **kali**

After logging in, the Kali Linux VM will be ready to use in the lab environment.

---

## Final Result

At this point, the Kali Linux virtual machine has been successfully downloaded, imported into VMware Workstation, renamed, and started for the first time, this VM is now ready to be used for cybersecurity testing, security tools, Wazuh log generation, and future lab exercises.

---

<p align="center">
  <strong>Lab Navigation</strong>
</p>

<p align="center">
  <a href="08-Installing-the-Wazuh-Agent-on-Windows-Server.md">⬅️ Previous Step: Install Wazuh Agent on Windows Server</a>
  &nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="01-Lab_Overview.md">Back to First Step: Lab Overview 🔄</a>
</p>
