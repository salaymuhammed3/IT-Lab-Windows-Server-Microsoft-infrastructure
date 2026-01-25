# Lab 01 – Step 02: Server Baseline Configuration

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
  - IP: 10.20.20.10
  - Subnet: 255.255.255.0
  - DNS: 10.20.20.10
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
