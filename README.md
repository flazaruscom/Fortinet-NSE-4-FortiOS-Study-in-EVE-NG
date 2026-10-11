# Fortinet NSE 4 / FortiOS Study Lab in EVE-NG

A virtual lab I built in EVE-NG (running on VMware Workstation) to study for Fortinet's FortiGate Administrator certification (formerly NSE 4) and to practise the FortiGate skills I use as a Junior Network Engineer.

> **Status:** Work in progress. I'm adding to this lab as I study.

## What's in the lab
- **FortiGate** firewall running FortiOS
- **Cisco switch** (CLI) connected to the FortiGate over a port-channel
- **FortiManager** and **FortiAnalyzer** nodes
- **Windows 11** and **Kali Linux** nodes, plus a VPC for basic connectivity testing

## What I've practised so far
  Adding FortiGate, FortiManager, FortiAnalyzer, Cisco and other QEMU images to EVE-NG
  Building a switch-to-FortiGate port-channel
  IP addressing and connectivity testing between nodes
  Accessing and managing the FortiGate from Kali Linux
  Configuring NTP on the FortiGate (see `FortiGate-Configure-NTP`)

# Reasoning for Repo
  Creation of adding virtioa.qcow2 QEMU images into directories for accessing images as nodes in EVE-NG
  
Documentation of commands to setup PC Nodes, Cisco CLI Switches and FortiOS.
  
Providing context of my study, showcasing how I have set this up, what commands I have used to access Fortigate nodes on Kali-Linux nodes inside EVE-NG.

# Inspiration 
<img width="856" height="419" alt="Screenshot 2026-09-30 212856" src="https://github.com/user-attachments/assets/164860ae-ecbe-4ff2-a1b3-c4de2dd74685" />
  
  Lab setup via Ahmed Ali (Udemy)

  ## Next steps
- [x] Core lab built: FortiGate, Cisco switch, Kali, Windows 11 and VPC nodes
- [x] NTP configured on the FortiGate
- [ ] VLAN segmentation on the switch and FortiGate
- [ ] Firewall policies between VLANs
- [ ] Register the FortiGate to FortiManager and push policy centrally
- [ ] Send FortiGate logs to FortiAnalyzer
- [ ] Remote-access VPN with FortiClient from the Windows 11 node
- [ ] Labelled topology diagram with the lab IP plan
