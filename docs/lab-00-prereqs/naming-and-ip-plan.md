# Lab 00 – Naming Standard and IP Addressing Plan

## Purpose
This document defines consistent naming conventions and IP addressing used across all lab environments.
Using a fixed standard reduces errors and reflects real-world IT practices.

---

## Active Directory design
- AD domain name: lab.local
- NetBIOS name: LAB

---

## Server naming conventions
| System | Role |
|------|------|
| DC1  | Domain Controller + DNS |
| SRV1 | File Server / DHCP (future lab) |

---

## Client naming conventions
| System | Role |
|------|------|
| W11-CL1 | Windows 11 domain client |
| W11-CL2 | Windows 11 domain client |

---

## Internal LAN IP plan (VMnet20)
- Subnet: 10.20.20.0/24

### Static IP assignments
| System | IP Address |
|------|-----------|
| DC1  | 10.20.20.10 |
| SRV1 | 10.20.20.20 |

### DHCP scope (future lab)
- 10.20.20.100 – 10.20.20.200

---

## DNS configuration
- Primary DNS server for all domain-joined systems:
  - 10.20.20.10 (DC1)

---

## Change management
Any changes to naming or IP allocation must be documented and committed to GitHub.
