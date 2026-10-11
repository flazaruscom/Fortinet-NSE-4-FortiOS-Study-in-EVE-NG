# Initial Setup: Port-Channel, VPC and Kali Access to the FortiGate GUI

How I built the base lab in EVE-NG: a port-channel between the Cisco switch and the FortiGate, IP addressing on the VPC, and Kali Linux reaching the FortiGate GUI.

> No VLAN segmentation yet; this is planned next (see Next steps in the README).

## Lab setup steps
<img width="640" height="241" alt="Lab setup in EVE-NG, step 1" src="https://github.com/user-attachments/assets/ffcdcfb7-023f-4533-87da-1de5b43b0674" />

<img width="1397" height="542" alt="Lab setup in EVE-NG, step 2" src="https://github.com/user-attachments/assets/146698e3-a869-4040-9e00-0b2f27fbfe69" />

## Uploading images with WinSCP
WinSCP lets you upload virtioa.qcow2 images and ISOs to EVE-NG.

1. Install WinSCP from https://winscp.net/eng/download.php
2. Create a new site with these settings:
   - **File protocol:** SFTP
   - **Hostname:** the IP address of your EVE-NG VM (if it uses NAT, this is likely a 192.168.x.x address)
   - **Username:** the username you set when first starting the EVE-NG VM
   - **Password:** the password you set when first starting the EVE-NG VM

<img width="600" height="400" alt="WinSCP new site settings" src="https://github.com/user-attachments/assets/e90a3c6a-9426-4070-86a3-dbcdcc888739" />

> EVE-NG's default login is `root` / `eve`. Change it after your first login.

## Installing the Windows 11 node
This video from Automation Archive covers the correct commands for setting up Windows 11 as a QEMU node in EVE-NG: https://www.youtube.com/watch?v=sxrBSTFQynQ&t=93s

## Installing the Kali Linux node
1. Download the Kali QEMU image from https://www.kali.org/get-kali/#kali-virtual-machines
2. Copy it into a folder under `/opt/unetlab/addons/qemu/` with the `linux-` prefix (I used `linux-Kali-2025.c1`).
3. Fix permissions so EVE-NG can use the image:
```
   /opt/unetlab/wrappers/unl_wrapper -a fixpermissions
```
4. Add the node to your lab and start it.

## Installing the FortiOS and Cisco switch nodes
These images need licences and a Fortinet account, so check the vendor documentation for installation. I followed Part 1 of Ahmed Ali's Udemy course.

## Commands and node setup
<img width="1187" height="372" alt="Node setup commands, part 1" src="https://github.com/user-attachments/assets/3d0ba007-6f05-4982-94a8-4ca769837122" />

<img width="1290" height="272" alt="Node setup commands, part 2" src="https://github.com/user-attachments/assets/73432cd3-a04a-4015-9525-16143540ddde" />
