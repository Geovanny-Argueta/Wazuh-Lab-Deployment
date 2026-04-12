## Ubuntu Server Installation in VMWare

Follow these steps to install Ubuntu Server inside your virtual machine:

---

### 1. Start Installation

The VM will boot automatically.  
Press **Enter** on **"Try or Install Ubuntu Server"** and wait.

![step1](..//Docs/Ubuntu-1.png)
---

### 2. Select Language

Choose your preferred language.  
For this lab, we will use:

- **English**

![step2](..//Docs/Ubuntu-2.png)
---

### 3. Installer Update

Since the VM has internet access, you will see an option to update the installer.

- Select: **Update to the new installer** (recommended)  
- You can also skip this step without issues

![step3](..//Docs/Ubuntu-3.png)
---

### 4. Keyboard Configuration

Select your keyboard layout.

- Recommended: **English (US)**

![step4](..//Docs/Ubuntu-4.png)
---

### 5. Installation Type

Leave the default settings and select:

- **Done**

![step5](..//Docs/Ubuntu-5.png)
---

### 6. Network Configuration

Leave the default network configuration.

- We will modify this later for lab purposes

Select **Done**.

![step6](..//Docs/Ubuntu-6.png)
---

### 7. Proxy Configuration

Do not configure any proxy.

- Leave it empty
- Select **Done**

![step7](..//Docs/Ubuntu-7.png)
---

### 8. Mirror Configuration

Wait for the mirror test to complete.

- Once finished, select **Done**

![step8](..//Docs/Ubuntu-8.png)
---

### 9. Storage Configuration (Step 1)

Leave the default configuration:

- **Use entire disk**
- **LVM enabled**
- **No encryption**

Select **Done**.

![setp9](..//Docs/Ubuntu-9.png)
---

### 10. Storage Configuration (Step 2)

No changes are required.

- Select **Done**

![step10](..//Docs/Ubuntu-10.png)
---

### 11. Confirm Changes

You will be asked to confirm disk changes.

- Select **Continue**

![step11](..//Docs/Ubuntu-11.png)
---

### 12. User Setup

Configure the following:

- Server name  
- Username  
- Password  

Then select **Done**.

![step12](..//Docs/Ubuntu-12.png)
---

### 13. Ubuntu Pro

Skip this step.

- Leave it as default
- Select **Continue**

![step13](..//Docs/Ubuntu-13.png)
---

### 14. OpenSSH Setup

Enable SSH access:

- Press **Enter** to select **Install OpenSSH server**
- Then select **Done**

This is important for remote access to your lab.

![step14](..//Docs/Ubuntu-14.png)
---

### 15. Featured Server Snaps

Leave this section as default.

- Select **Done**

![step15](..//Docs/Ubuntu-15.png)
---

### 16. Installation Process

Wait for the installation to complete.  
This may take several minutes.

Once finished:

- Select **Reboot Now**
- Press **Enter** if prompted

![step16](..//Docs/Ubuntu-16.png)
---

### 17. Login

After reboot:

- Enter your **username**
- Enter your **password**

![step17](..//Docs/Ubuntu-17.png)
---

✅ Ubuntu Server is now successfully installed and ready for the next steps.
