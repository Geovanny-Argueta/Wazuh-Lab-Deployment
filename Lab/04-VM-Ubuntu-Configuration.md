# Install Ubuntu Server

This section covers the Ubuntu Server installation inside the virtual machine created in the previous step.

## Installation Steps

### 1. Start the Installer

Boot the VM and select **Try or Install Ubuntu Server**.

![Ubuntu boot menu](../Docs/Ubuntu-1.png)

### 2. Select the Language

I used **English** for the operating system and documentation.

![Language selection](../Docs/Ubuntu-2.png)

### 3. Installer Update

If Ubuntu offers a newer installer, you can update it before continuing. Skipping this update will not normally prevent the operating system installation.

![Installer update](../Docs/Ubuntu-3.png)

### 4. Configure the Keyboard

Select the keyboard layout that matches your physical keyboard. This lab uses **English (US)**.

![Keyboard configuration](../Docs/Ubuntu-4.png)

### 5. Choose the Installation Type

Keep the standard Ubuntu Server installation and select **Done**.

![Installation type](../Docs/Ubuntu-5.png)

### 6. Initial Network Configuration

Leave the automatic network settings in place for now. The VMware lab networks will be configured in the next guide.

![Initial network configuration](../Docs/Ubuntu-6.png)

### 7. Proxy and Mirror

Leave the proxy field empty unless your network requires one. Wait for the Ubuntu mirror test to complete, then continue.

![Proxy configuration](../Docs/Ubuntu-7.png)
![Mirror configuration](../Docs/Ubuntu-8.png)

### 8. Configure Storage

For this lab, I used:

- **Use entire disk**
- **LVM enabled**
- **No disk encryption**

Review the storage layout, select **Done**, and confirm the changes.

![Storage configuration](../Docs/Ubuntu-9.png)
![Storage layout](../Docs/Ubuntu-10.png)
![Storage confirmation](../Docs/Ubuntu-11.png)

### 9. Create the Local Account

Create a server name, administrator username, and strong password. Use lab-specific values and do not publish the password in screenshots or documentation.

![Local account setup](../Docs/Ubuntu-12.png)

### 10. Ubuntu Pro

Ubuntu Pro is not required for this lab, so I skipped this step.

![Ubuntu Pro](../Docs/Ubuntu-13.png)

### 11. Enable OpenSSH

Select **Install OpenSSH server**. SSH will make it easier to administer the Wazuh server from the host machine.

![OpenSSH configuration](../Docs/Ubuntu-14.png)

### 12. Optional Packages

No featured server snaps are required. Leave the list unchanged and continue.

![Featured server snaps](../Docs/Ubuntu-15.png)

### 13. Complete the Installation

Wait for the installation to finish, select **Reboot Now**, and press **Enter** if Ubuntu asks you to remove the installation media.

![Installation complete](../Docs/Ubuntu-16.png)

### 14. Sign In

After the reboot, sign in with the local account created earlier.

![Ubuntu login](../Docs/Ubuntu-17.png)

## Expected Result

Ubuntu Server should start normally and display a terminal login prompt. The VM is now ready for the network configuration.

---

<p align="center">
  <strong>Lab Navigation</strong>
</p>

<p align="center">
  <a href="03-Create-Ubuntu-VM.md">⬅️ Previous: Create Ubuntu Virtual Machine</a>
  &nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="05-Configuration-Ubuntu-Before-Install-Wazuh.md">Next: Configure VMware Networks ➡️</a>
</p>
