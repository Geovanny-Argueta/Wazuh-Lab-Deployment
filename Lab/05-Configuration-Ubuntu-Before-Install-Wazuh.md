# Configure the VMware Lab Networks

## Objective

I use two virtual networks in this lab:

- A **NAT network** for software updates and package downloads
- A **Host-Only network** for communication between the lab machines

This setup keeps the testing traffic separate from the physical network while still allowing the Wazuh server to reach the internet when needed.

## Network Plan

| VMware Network | Type | Subnet | Purpose |
|---|---|---|---|
| VMnet1 | NAT | `192.168.10.0/24` | Internet access |
| VMnet2 | Host-Only | `10.10.10.0/24` | Internal lab traffic |

Your VMnet numbers may be different if VMware already uses VMnet1 or VMnet2. The important part is to keep one NAT network and one Host-Only network.

## Configuration Steps

### 1. Open Virtual Network Editor

In VMware Workstation, select:

**Edit > Virtual Network Editor**

![Virtual Network Editor](../Docs/Configuration-before-install-wazuh/step-1.png)

### 2. Enable Administrative Changes

Select **Change Settings** and approve the prompt.

![Change network settings](../Docs/Configuration-before-install-wazuh/step-2.png)

### 3. Create the NAT Network

Select **Add Network**, choose an available VMnet other than VMnet0, and create the network.

VMnet0 is normally reserved for Bridged networking, so I left it unchanged.

![Add a virtual network](../Docs/Configuration-before-install-wazuh/step-3.png)
![Confirm the VMnet](../Docs/Configuration-before-install-wazuh/step-5.png)

Set the network type to **NAT** and use `192.168.10.0/24`, or another private subnet that does not conflict with your home network.

![NAT network configuration](../Docs/Configuration-before-install-wazuh/step-6.png)

### 4. Create the Host-Only Network

Create a second VMnet and select **Host-Only**. I used:

- Subnet: `10.10.10.0`
- Mask: `255.255.255.0`

![Host-Only network configuration](../Docs/Configuration-before-install-wazuh/step-7.png)

I did not remove VMware's existing default networks because other virtual machines may depend on them.

### 5. Add the NAT Adapter to the Wazuh VM

Power off the Wazuh VM and open **Edit virtual machine settings**.

![Wazuh VM settings](../Docs/Configuration-before-install-wazuh/step-8.png)

Set the first adapter to **Custom: Specific virtual network** and select the NAT VMnet.

![NAT adapter assignment](../Docs/Configuration-before-install-wazuh/step-9.png)

### 6. Add the Internal Adapter

Add a second **Network Adapter** and assign it to the Host-Only VMnet.

![Host-Only adapter assignment](../Docs/Configuration-before-install-wazuh/step-11.png)

### 7. Update Ubuntu

Start the VM and run the following command on the **Wazuh Ubuntu Server**:

```bash
sudo apt update && sudo apt upgrade -y
```

### 8. Verify the Interfaces

On the **Wazuh Ubuntu Server**, check the assigned addresses and routes:

```bash
ip addr
ip route
```

The server should have one interface connected to the NAT network and another connected to the internal lab network.

## Expected Result

The Wazuh server should reach the internet through NAT and communicate with the other lab machines through the Host-Only network.

---

<p align="center">
  <strong>Lab Navigation</strong>
</p>

<p align="center">
  <a href="04-VM-Ubuntu-Configuration.md">⬅️ Previous: Install Ubuntu Server</a>
  &nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="06-Wazuh-Installation.md">Next: Install Wazuh All-in-One ➡️</a>
</p>
