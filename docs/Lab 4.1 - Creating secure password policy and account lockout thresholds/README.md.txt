## Purpose:

To ensure that all users are using best practice, being a secure password that is unique and account lockout to prevent to many incorrect passwords from being entered and to also force users to create memorable passwords that are secured by the password policy.


## Config & Validation:

- Create a GPO that ensures that passwords are unique and meet a password criteria so that they are forced to make a strong password (Config)

- GPO criteria will be the password has to be a minimum of 8 characters, include both capitalised and lowercase letters and at least 1 special character ( i.e. !"£$%), (Config)

- All users on next login will have to create a password to that criteria. (Validation)

- The users that input a password that is not to the criteria will get a pop-up showing that their password is not compatible and what the criteria is that they need to meet. (Validation)



## Why this is beneficial ?

This will ensure that all users on the domain are following best security practices by creating a password that is unique and not easily guessable keeping their accounts safe and secure from being compromised 

Account lockout is in place to prevent attempts of brute force attacks to be mitigated and also as a measure to ensure that users have a memorable but secure password.