# This folder contains SU01 practice screenshots.

In SAP users can be created and maintained by using Tcode SU01.

# SU01--USER MAINTENANCE

In SU01,we can perform different activities such as:

Create user

Change user

Display

Delete user

Copy user

Lock/Unlock user

Reset password/Change password

# USER MASTER RECORD

Combination of different tabs such as (documentation tab, address tab, logon data tab, SNC, default, Parameters, Roles, Profiles, Groups, Personalization, License tab)called as User Master Record.

**1.DOCUMENTATION** ---> We need to maintain document,It is used to store comments,notes or reason for user account action by using tickets,these tickets are raised by HR,Manager or end user themselves depending on the situation.

**2.ADDRESS** ---> Stores personal information like firstname,lastname, mail id, function, department.

**3.LOGON DATA** ---> Stores the usertype, password field.

**4.SNC/SSO (Secure Network Communication/Single Sign-On)** ---> Provides encryption,integrity and secure authorization between SAP system and Front-end(SAP GUI).

   SSO allows users to login once and access multiple SAP systems without re-entering password.

**5.DEFAULT** ---> This can be as per user recommendations like timezone,dateformat.

**6.PARAMETER** ---> Parameters tab is used to set default values for a user so that when they run transactions, the system automatically uses those values.(parameter Id and value)

**7.ROLES** ---> It is used to assign the roles to the users.

**8.PROFILES** ---> Technical representation of the authorizations.If we assign roles to the users than those automatically assign to hthe profile also.If not role authorizations will not work for that user.

**9.PERSONALIZATION** ---> It is used to store user-specific default data,common for all.

**10.LICENSE** ---> Type of SAP usage rights assigned to a user,used for billing and compliance.


# Types of users in SAP

**1.DIALOG (A)** --> Named persons/ All humans can called as a dialog type users.

**Properties :**
                 1. Login is possible through SAP GUI

                 2. Password is expired for every 2 months 60 days or 90 days.

                 3. Users can change their own password.

                 4. Used for day-to-day interactive work in SAP.

**2. SYSTEM (B)** --> Used for communication between SAP systems — mainly internal RFC (Remote Function Call) connections, background jobs, or interfaces.These users are not real people, but technical users used for system-to-system communication.
**Properties :** 
                 1. Login is not possible through SAP GUI

                 2. Password is never expired(until manually changed).

                 3. Used in internal system-to-system communication.

**3. COMMUNICATION (C)** --> Used for external RFC connections

**Properties :** 
                 1. Login is not possible through SAP GUI,Possible through RFC or external interface 

                 2. Password is never expired(until manually changed).

                 3. Suitable for external communications or integrations


**Example**

Suppose you have a Python application that reads user data from SAP using RFC → you’ll use a **COMMUNICATION user**.

But if SAP GRC system wants to fetch data from SAP ECC → you’ll use a **SYSTEM user**.


**4. SERVICE (S)** --> Emergency access purpose.It is a common user ID used by many people (shared login).
**Properties :** 
                 1.Login is possible through SAP GUI.

                 2. Password is never expired(until manually changed).

                 3. Suitable for external communications or integrations

                 4. Used for Emergency access (when someone can’t log in with their own ID)

**4. REFERENCE (L)** --> A Reference User is a user in SAP whose roles and authorizations are copied to other users. Instead of manually 
assigning roles to each new user, you can assign a reference user, and the system automatically inherits all the roles of that reference 
user.
