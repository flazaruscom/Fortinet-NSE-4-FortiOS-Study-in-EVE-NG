# Fortinet-NSE-4-FortiOS-Study-in-EVE-NG
  Documentation on EVE-NG setup in VMware Workstation for Cisco CLl Switch/FortiGate/FortiManager/FortiAnalyzer/Windows-11/Kali-Linux Nodes

# Reasoning for Repo
  Creation of adding virtioa.qcow2 QEMU images into directories for accessing images as nodes in EVE-NG
  
  Documentation of commands to setup PC Nodes, Cisco CLI Switches and FortiOS.
  
  Providing context of my study, showcasing how I have set this up, what commands I have used to access Fortigate nodes on Kali-Linux nodes inside EVE-NG.

# Inspiration 
<img width="856" height="419" alt="Screenshot 2026-09-30 212856" src="https://github.com/user-attachments/assets/164860ae-ecbe-4ff2-a1b3-c4de2dd74685" />
  
  Lab setup via Ahmed Ali (Udemy)

# EVE-NG Creation of Port-Channel on Switch + Fortigate, IP Setup on VPC and Kali Linux to access Fortigate GUI. 
My Setup / Steps (No current VLAN Segmentation but this is subject to be issued)

<img width="1812" height="535" alt="image" src="https://github.com/user-attachments/assets/0d86f355-a019-4995-9c25-c1a644fabb48" />


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
