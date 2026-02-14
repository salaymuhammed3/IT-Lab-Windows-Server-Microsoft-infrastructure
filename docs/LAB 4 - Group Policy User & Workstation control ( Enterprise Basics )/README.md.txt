## Purpose of lab 
Creating a group policy to restrict access to a specific function or tool with in windows.


## Config & Validation

GPO is linked to staff OU 

- delegation to enable certain users in OU's to have exclusive permissions in this instance it would be the Admin account for the staff OU. (Config)

- Enable newly created GPO which prohibits all users in the staff group but delegated user from having access to control panel. (Config)

- After delegation has been applied run CMD command (gpupdate /r) and then restart the pc. 
  (Validation)

- Pc has now reset so run command (gpresult /r)  to see results of GPO's and if they have been applied and what GPO has been applied (Validation)

- Then an actual test on the delegated account to see if the GPO applied correctly and the (AdminS) account has access to control panel (Validation)




## Why this is beneficial ?

 This prevents a key security vulnerability being that users such as staff don't have access to administrator level tools/controls which prevents them or a malicious third-party from making changes that would leave the domain open to potential vulnerabilities.

Delegation based access allows for strict access to be given to users who have a clear purpose and function for having such accesses such as sys admins. 