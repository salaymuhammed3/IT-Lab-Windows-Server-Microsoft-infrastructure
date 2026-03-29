# Purpose of lab 

- A new client pc was created in VMWare, which will join to ( DC1.lab.local) domain, as this will be a domain based client
- GPO's will be created which will control the users ability to have specific functions and access levels to certain apps and permission on their accounts and devices
- Creation of these GPO's replicates how sysadmins and technicians on enterprise and general server environments delegate and manage user access to applications and 



## Config & Validation 

- On client pc go to system properties and change the device name to (Client-1), also make (Client-1) member of domain (lab.local). (Config)
- Add/create (Client-1) on active directory (Config)
- Modified Security ACL of lab.local DNS zone to grant domain controller group full control (Config)
- During configuration and adding (Client-1) to domain I ran into an issue where (Client-1) was not connecting to domain (lab.local), so I had to create a reverse lookup zone for (192.168.232). (Config)
- Used CMD to run (nslookup lab.local) and confirmed that (Client-1) was connecting to (lab.local). (Validation)
- Created a GPO, this GPO was created so that the domain admin accounts can work on the staff computers/laptops, as if the admin account was to login without the GPO the admin account would login as a default user without any admin rights. (Config)
- GPO created and (gpupdate /force) is ran on client pc with CMD to force new GPO to apply (config)
- Went on computer management and checked admin accounts and the admin account that was added via the GPO now appears under the administrator accounts (Validation) 


## Why this is beneficial ?

- Device (client-1) needs to be added to domain so that it goes from a stand alone workstation to active directory managed device, establishing secure trust relationships with (DC1)-Domain Controller via DNS. This enables centralised authentication and allows for GPO's to be applied for better control/security and automated software deployment
- GPO created as a measure of best security practice, principle of least privilege. This GPO uses group policy preferences to add IT admins to the local admin group, allowing for support staff to have admin rights necessary to manage devices without exposing highly privileged domain admin credentials 