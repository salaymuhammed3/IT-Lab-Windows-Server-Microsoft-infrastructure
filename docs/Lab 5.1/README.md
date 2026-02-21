
## Lab 5.1 - Implementing quotas and file screening using (FSRM), File Server Resource Manager


## Purpose

- Used by system administrators to keep track and maintain the storage of their servers.
- Helps to manage and classify data that is stored on file servers

## Config & Validation

- Get FSRM installed on the domain via server manager (config)
- Once on FSRM go to quota management and set a storage limit (quota) for folders so that users do not fill up the storage of the server. (config)
- Setup custom file screening properties to prevent users from installing or sharing files/folders in the shared folder that could lead to the storage filling up fast (config)
- On client PC the folder size restriction should be visible showing max capacity of 10GB (validation)
- When user tries to save a restricted file type to shared folder they should receive a restriction message (validation)

## Why this is beneficial ?

FSRM is beneficial from a financial standpoint as having the folder size limitations in place prevents users from using all the available storage that a server may have, which would require a business to purchase more physical storage for their server that can become expensive. 

Having file screening in place also can act as a layer of security as we can have restrictions in place to prevent certain file types such as executables from being saved to shared folders, which prevents any malicious software from being saved let alone ran on a users device. 
