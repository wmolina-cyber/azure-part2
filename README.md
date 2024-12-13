# Azure Computing and Networking Lab - Part 2

## Overview
In Part 2 of this lab, I observed ICMP traffic between my Azure Virtual Machines using Wireshark. I also analyzed ping requests and replies within the virtual network.

## Objectives
- Connect to my Windows 10 Virtual Machine using Remote Desktop.
- Install and use Wireshark to capture network traffic.
- Observe and filter ICMP traffic.
- Ping the Ubuntu VM from the Windows 10 VM.

---

## Steps

### 1. Connected to the Windows 10 Virtual Machine
1. Retrieved the **Public IP Address** of the Windows 10 VM from the Azure Portal.
2. Used Remote Desktop to connect to the Windows 10 VM using the credentials created in Part 1.

![2](https://github.com/user-attachments/assets/9225ba2e-eab9-43a2-b9b6-125f5838b518)

---

### 2. Installed Wireshark on the Windows 10 VM
1. Within the Windows 10 VM, downloaded and installed [Wireshark](https://www.wireshark.org/).
2. Launched Wireshark and started a new packet capture.

![26](https://github.com/user-attachments/assets/5554240c-ccac-4cba-9492-7df24aa2a0a1)

---

### 3. Filtered for ICMP Traffic
1. In Wireshark, set the filter to `icmp` to capture only ICMP traffic.
2. Applied the filter and observed the packet capture.

![28](https://github.com/user-attachments/assets/1ff58038-a3d9-430e-8e85-bdb753f5ba87)

---

### 4. Pinged the Ubuntu VM from the Windows 10 VM
1. Retrieved the **Private IP Address** of the Ubuntu VM from the Azure Portal.
2. Opened PowerShell on the Windows 10 VM.
3. Ran the command:
   ```bash
   ping 10.0.0.5
   ```
4. Observed the ping requests and replies in Wireshark.

![32](https://github.com/user-attachments/assets/bd33487a-39ad-44d8-be00-151a9c0948c1)
![33](https://github.com/user-attachments/assets/01f643fb-4655-4a99-8faa-8dfd93343ff1)

---
## Conclusion
This concludes Part 2 of the Azure Computing and Networking Lab. In this segment, I successfully connected to my virtual machine, utilized Wireshark to analyze ICMP traffic, and gained insights into network behavior within Azure's virtual network environment.
