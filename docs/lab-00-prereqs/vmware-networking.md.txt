# Lab 00 – VMware Networking Baseline

## Purpose of this document
This document defines the virtual networking design used across all home lab projects.
The goal is to simulate a small enterprise-style environment with:
- Controlled internet access
- A fully isolated internal LAN for Active Directory and domain services

This network design is reused across all labs to ensure consistency.

---

## Host environment
- Host OS: Windows 11
- Virtualisation platform: VMware Workstation Pro 17

---

## Virtual network design overview

Two VMware virtual networks are used:

### VMnet10 – NAT (Internet access)
- Purpose:
  - Provide controlled internet access for patching and downloads
  - Prevent direct exposure of lab systems to the host network
- Network type: NAT
- Subnet: 10.10.10.0/24
- DHCP: Enabled (VMware-managed)

### VMnet20 – Host-only (Internal LAN)
- Purpose:
  - Simulate an internal corporate network
  - Host Active Directory, DNS, and all domain-joined systems
- Network type: Host-only
- Subnet: 10.20.20.0/24
- DHCP: Disabled (will be provided by Windows Server later)

---

## Security and isolation considerations
- VMnet20 has no direct internet access
- Domain services are isolated from the host LAN
- This design mirrors common enterprise segmentation:
  - Internal LAN
  - Controlled egress via NAT or firewall

---

## Validation checklist
The following must be true before continuing with any lab:
- VMnet10 exists and provides internet access
- VMnet20 exists and has DHCP disabled
- Host has VMware network adapters for both VMnet10 and VMnet20

---

## Evidence
Screenshots proving the configuration are stored in:
