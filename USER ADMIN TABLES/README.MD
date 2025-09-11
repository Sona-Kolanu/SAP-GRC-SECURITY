In SAP,all user-related data is stored in the database tables.
These tables are called as User Administration Tables.

User Administration Tables starts with USR* in security.

We have different tables like--

USR01-- Stores users default data(date format,decimal notation,logon language etc...)

USR02-- Stores users logon-related data/Lock status(last login date/time,wrong login attempts,lock status,user type)

USR03-- Stores users address data or details(name,email,phone number,department etc..)

USR04-- Stores users authorization/profile assignment data(modification data reflected here--(who modified,at what time, on which date)
                                                           
USR05-- Stores users specific parameter data(parameter ID and parameter Value)
                                                           
USR40-- Password restriction table.
        Stores forbidden/illegal password patterns to prevent weak and common passwords.                                                   
                                                    
