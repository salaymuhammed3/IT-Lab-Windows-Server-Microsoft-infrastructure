Lab 02 - Active Directory Objects and identity management

## Objective: 

 Lab was focused on creating core AD (Active Directory) objects used in a real enterprise environment, including OU's, users, devices (computers/laptops) and security groups.


## Environment
 
 - Domain controller: DC1 
 - Domain: lab.local
 - Tools:
     - Active Directory Users and computers
     - Windows Server (Domain Controller)

## OU Structure

 Below is the exact structure of my OU's which were created to separate users, computers/laptops and security groups:

  - School
    - Staff
       - Users 
       - Computers/laptops
    - Student
       - Users
       - Computers/laptops
  -Groups
    - Security Groups
  - Servers 

# This structure mirrors enterprise and educational directory designs



## created objects:

Within 'school -> staff ' their is a sub-group for Staff and students also within in that I have created a group specifically for computers/laptops

A 'group' OU was created that contains the object 'groups' which has the 'security groups', one for staff and one for students, these are created to make sure that permissions and access control for example we wouldn't want students to be given access to a groups named 'exam papers' for example which is why security groups are created so that correct users are given access to only what they need 


















## Evidence

![image alt](https://github.com/salaymuhammed3/IT-Lab-Windows-Server-Microsoft-infrastructure/blob/74ce325b8f9f771f4d030492a67e28c1a6bd734b/docs/lab-02-ad-objects/evidence/Adding-users-to-designated-security%20group-corresponding-with-name.png)

![image alt](https://github.com/salaymuhammed3/IT-Lab-Windows-Server-Microsoft-infrastructure/blob/26dd99a3d7bbc3be9177d3faa37db4136b1463f2/docs/lab-02-ad-objects/evidence/Creating-student-security-group.png)

![image alt](https://github.com/salaymuhammed3/IT-Lab-Windows-Server-Microsoft-infrastructure/blob/26dd99a3d7bbc3be9177d3faa37db4136b1463f2/docs/lab-02-ad-objects/evidence/Creating-user-within-staff-OU.png)

![image alt](https://github.com/salaymuhammed3/IT-Lab-Windows-Server-Microsoft-infrastructure/blob/26dd99a3d7bbc3be9177d3faa37db4136b1463f2/docs/lab-02-ad-objects/evidence/Setting-up-OU'S.png)

















