# Lab 01 – Step 01: Server Baseline Configuration

## Purpose
This step prepares the Windows Server for Active Directory by applying baseline configuration:
- Proper server naming
- Network adapter hygiene
- Static IP configuration
- Snapshot creation for rollback

These steps are mandatory best practice before promoting a domain controller.

---

## Server rename
- Computer name set to: DC1
- Restart performed to apply change

---

## Network configuration
- Network adapter renamed to: LAN-VMnet20
- Static IPv4 configuration applied:
  - IP: 192.168.232.129
  - Subnet: 255.255.255.0
  - DNS: 127.0.0.1
  - Gateway: Not required for internal LAN

---

## Validation
- ipconfig /all used to confirm correct addressing
- Output saved as evidence

---

## Snapshot
A VMware snapshot was taken prior to Active Directory installation to allow rapid rollback if required.

Snapshot name:
- Pre-AD Baseline




#### Evidence

<img width="199" height="226" alt="image" src="https://github.com/user-attachments/assets/3d66164b-1483-4f49-b0f7-835c7be1d33d" />



