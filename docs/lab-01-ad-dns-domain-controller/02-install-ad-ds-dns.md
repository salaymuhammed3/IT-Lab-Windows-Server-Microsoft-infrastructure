# Lab 01 – Step 03: Install AD DS and DNS

## Purpose
This step installs Active Directory Domain Services and DNS, then promotes the server to a Domain Controller in a new forest.

---

## Roles installed
- Active Directory Domain Services
- DNS Server

---

## Domain configuration
- Forest root domain: lab.local
- NetBIOS name: LAB
- DNS integrated with AD
- Global Catalog enabled

---

## Validation performed
- net share confirmed SYSVOL and NETLOGON
- nslookup verified DNS resolution
- dcdiag used to validate domain health

---

## Result
DC1 successfully promoted to a domain controller for lab.local.


# Evidence

![image alt](https://github.com/salaymuhammed3/IT-Lab-Windows-Server-Microsoft-infrastructure/raw/f99a3e3a2bc8a7902c6bfa6357e1ccaa07f7dc89/docs/lab-01-ad-dns-domain-controller/evidence/screenshots/AD%20DS%20-%20(DC1)%20ADDING%20SREVER%20roles%20(%20vm).png) 
Figure 1: Installation of active directory and domain services (AS DS)

<img width="820" height="404" alt="image" src="https://github.com/user-attachments/assets/3e057978-4637-472b-9acd-f17fed872367" />



Figure 2: Showing that DC1 (Server name) is my domain controller 









<img width="640" height="184" alt="image" src="https://github.com/user-attachments/assets/ea6e1725-3ad4-4359-a54a-1f7ae7366729" />






<img width="640" height="184" alt="image" src="https://github.com/user-attachments/assets/dc0a74ea-d217-4de0-b746-828eccdda828" />




Figure 3: Conforming that SYSVOL and NETLOGON are working meaning that domain contreoller is operational 
