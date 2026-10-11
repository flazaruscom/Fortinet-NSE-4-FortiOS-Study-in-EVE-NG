# Fortinet NSE 4 / FortiOS Study Lab in EVE-NG

A virtual lab I built in EVE-NG (running on VMware Workstation) to study for Fortinet's FortiGate Administrator certification (formerly NSE 4) and to practise the FortiGate skills I use as a Junior Network Engineer.

> **Status:** Work in progress. I'm adding to this lab as I study.

## What's in the lab
- **FortiGate** firewall running FortiOS
- **Cisco switch** (CLI) connected to the FortiGate over a port-channel
- **FortiManager** and **FortiAnalyzer** nodes
- **Windows 11** and **Kali Linux** nodes, plus a VPC for basic connectivity testing

## What I've practised so far
- Adding FortiGate, FortiManager, FortiAnalyzer, Cisco and other QEMU images to EVE-NG
- Building a switch-to-FortiGate port-channel
- IP addressing and connectivity testing between nodes
- Accessing and managing the FortiGate from Kali Linux
- Configuring NTP on the FortiGate

## Documentation
- [Initial Setup](Initial%20Setup.md): lab topology, port-channel build, uploading images with WinSCP, and node installs
- [FortiGate NTP configuration](FortiGate-Configure-NTP.md): CLI steps for FortiOS 7.0.5

## Why this repo
- Documents how I added QEMU images (virtioa.qcow2) to EVE-NG so they run as nodes
- Records the commands I used to set up PC nodes, Cisco switches and FortiOS
- Shows how I access and manage FortiGate nodes from Kali Linux inside EVE-NG

## Next steps
- [x] Core lab built: FortiGate, Cisco switch, Kali, Windows 11 and VPC nodes
- [x] NTP configured on the FortiGate
- [ ] VLAN segmentation on the switch and FortiGate
- [ ] Firewall policies between VLANs
- [ ] Register the FortiGate to FortiManager and push policy centrally
- [ ] Send FortiGate logs to FortiAnalyzer
- [ ] Remote-access VPN with FortiClient from the Windows 11 node
- [ ] Labelled topology diagram with the lab IP plan

## Credits
Lab design based on Ahmed Ali's FortiGate course on Udemy.

<img width="856" height="419" alt="Reference lab setup from Ahmed Ali's Udemy course" src="https://github.com/user-attachments/assets/164860ae-ecbe-4ff2-a1b3-c4de2dd74685" />
