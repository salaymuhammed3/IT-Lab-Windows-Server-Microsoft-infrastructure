## Purpose 

- For security purposes to prevent users and groups that aren't meant to see certain folder from seeing them ( e.g. don't want members of HR seeing Finance data )
- Prevent no admin users form deleting company files 
- Also permissions based access so that only required and authorised users have the ability to make changes to files, folder etc.. for example a manager making corrections to work or data 



## Config & Validation 

- Create a shared folder on Domain server which will be shared to staff (Config)
- Give shared only access to staff, shared permissions only give a restricted amount of access and it is in the folder level only ( Config)

- Go to security tab and give privileged users such as (Admin) more exclusive and full control over folder and the files within it as the security tab is NTFS so Admin has folder & file level permissions compared to staff who only got shared folder level permissions and not NTFS. (Config)


- Now network drives will be mapped so that they work on client pc, but this is not an ideal way of setting up shared folders as after the client device is restarted the shared folder will disappear  and have to be added back again, hence the reason it is 'mapped' (Config)

- Now for a more Permanente solution to the above issue that 'mapped' has is to use network sharing which will be done by configuring a GPO to automatically map drives for users (config)

- GPO created and users that should be in the group added in, run GPUPDATE /force on client pc forcing GPO then restart client pc and then check to see if the user has access to the new shared folder (Validation)


## Why this is beneficial ?

Having shared file GPO's allows for users to have access to shared folders and files without the need to manually added a shared folder via file explorer every time they needed access reducing the incidents of technical issues and also save time for both technicians and the end users.
