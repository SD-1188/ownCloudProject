# ownCloud Quick Reference Guide

------

This quick reference guide assumes that the reader is well versed with ownCloud pre-requisites and installation in Windows 7. This guide covers the following topics: 

- Install and configure ownCloud on Windows 7
- Add new user account to ownCloud server
- Enabling users to connect to ownCloud server through mobile client

------



## Installing ownCloud on Windows 7

To install ownCloud in your Windows 7 system, perform the following steps: 

1. Naviagate to *Windows Programs and Features* and enable *Internet Information Services (IIS)* 
2. Download and install PHP and MySQL
3. Download ownCloud. Extract it and copy the folders to *C:\Example\wwwroot" folder*
4. Navigate to Config folder in server install files. Rename the configuration file to *configex.php*
5. Use the *configex.php* file to define values for *dbname*, *dbuser*, and *dbpassword*
6. To view the admin panel, open a web browser and type *http://localhost/owncloud*

## Adding a User Account

To add a user account to ownCloud server, perform the following steps: 

1. In your ownCloud server, navigate to *User Management* page.
2. In the *Username* field, enter the login name.
3. In the *Password* field, enter the password.
4. Select the user group from the drop-down list next to *Password* field.
5. Click *Create*.

## Connecting with ownCloud Server through Mobile Client

To connect to ownCloud server though mobile client, perform the following steps: 

1. To enable access from mobile client, install Time-based One Time Password (TOPT). 

```
owncloud recommends that you use one of these TOPT applications: OpenOTP, PrivacyIDEA, and TOPT
```

2. Install second factoring application on your mobile device such as FreeOTP
3. Open your mobile application, navigate to personal security and select *Activate TOPT*.
4. Scan the QR-code and verify the authentication through your mobile's second factoring application.
5. Open the ownCloud application and login to the server through two-factor authentication.
