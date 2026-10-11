# EVE-NG Creation of Port-Channel on Switch + Fortigate, IP Setup on VPC and Kali Linux to access Fortigate GUI. 
My Setup / Steps (No current VLAN Segmentation but this is subject to be issued)

<img width="640" height="241" alt="image" src="https://github.com/user-attachments/assets/ffcdcfb7-023f-4533-87da-1de5b43b0674" />

<img width="1397" height="542" alt="image" src="https://github.com/user-attachments/assets/146698e3-a869-4040-9e00-0b2f27fbfe69" />



# WinSCP File Transferring Setup

This allows you to upload virtioa.qcow2 files and ISO's to EVE-NG

Install WinSCP via: https://winscp.net/eng/download.php

Setup a New Site 

File Protocol: SFTP
Hostname: "The IP of your EVE-NG VM, If set to NAT this will likely be a 192.168 address

<img width="600" height="400" alt="image" src="https://github.com/user-attachments/assets/e90a3c6a-9426-4070-86a3-dbcdcc888739" />

Username: "The name you setup on startup of the eve-ng vm"

Password: "The password you setup on startup of the eve-ng vm"

Default Username and Password is: 

Username: Root

Password: eve

# Installation of Windows Node

https://www.youtube.com/watch?v=sxrBSTFQynQ&t=93s

Credit to Automation Archive

Fantastic Video on setup of Windows 11 Installation into EVE-NG with correct commands on installation / setup as QEMU in Eve-NG. 

# Installation of Kali-Linux Node

https://www.kali.org/get-kali/#kali-virtual-machines

The QEMU installation is as simple as adding into a file path under: /opt/unetlab/addons/qemu/linux-Kali-2025.c1 and running the node. 

# Installation of FortiOS / Cisco Switch Node

These images require licensing, creation of accounts in Fortigate so please review online the installation, or use Ahmed Ali's Udemy Course Part1 on assistance of Installation like I have. 


# Commands + Setup of Nodes
<img width="1187" height="372" alt="image" src="https://github.com/user-attachments/assets/3d0ba007-6f05-4982-94a8-4ca769837122" />

<img width="1290" height="272" alt="image" src="https://github.com/user-attachments/assets/73432cd3-a04a-4015-9525-16143540ddde" />
