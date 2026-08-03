# Install VMware Workstation

## Objective

VMware Workstation is the virtualization platform I use to run the Wazuh server, Windows endpoint, and Kali Linux on the same computer. This step prepares the host before creating any of the lab machines.

## Installation Steps

1. Go to the [Broadcom Support Portal](https://support.broadcom.com/) and sign in. A Broadcom account may be required before the installer becomes available.

2. Open **My Downloads** and select **Free Software Downloads Available Here**.

   ![Broadcom downloads page](../Docs/VMWare-1.png)

3. Search for **VMware Workstation Pro** and choose the installer for your host operating system.

   ![VMware Workstation product page](../Docs/VMWare-2.png)
   ![VMware Workstation version selection](../Docs/VMWare-3.png)

4. Complete the download form if Broadcom displays one, then download the installer.

   ![VMware Workstation download](../Docs/VMWare-4.png)

5. Locate the installer, right-click it, and select **Run as administrator**.

6. Accept the license agreement and continue through the setup wizard.

7. When the optional features appear, enable:

   **Add VMware Workstation console tools into the system PATH**

   ![VMware installation options](../Docs/VMWare-5.png)

8. Keep the remaining settings at their defaults unless your computer requires something different.

9. Select **Install**, wait for the process to finish, and restart the host if prompted.

10. Open VMware Workstation and confirm that the application starts normally.

## Expected Result

VMware Workstation should open without errors and be ready to create the first virtual machine.

---

<p align="center">
  <strong>Lab Navigation</strong>
</p>

<p align="center">
  <a href="01-Lab_Overview.md">⬅️ Previous: Lab Overview</a>
  &nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="03-Create-Ubuntu-VM.md">Next: Create Ubuntu Virtual Machine ➡️</a>
</p>
