# XSS with w3af, DVWA
### What is cross-site scripting (XSS)?
> "Cross-site scripting (also known as XSS) is a web security vulnerability that allows an attacker to compromise the interactions that users have with a vulnerable application."
### How does XSS work?
> "Cross-site scripting works by manipulating a vulnerable web site so that it returns malicious JavaScript to users. When the malicious code executes inside a victim's browser,   
the attacker can fully compromise their interaction with the application."
### What are the types of XSS attacks?
**Three main parts of XXS**
* Reflected XSS, where the malicious script comes from the current HTTP request.  
* Stored XSS, where the malicious script comes from the website's database.  
* DOM-based XSS, where the vulnerability exists in client-side code rather than server-side code.  
### Reflected cross-site scripting
simplest variety of cross-site scripting. It arises when an application receives data in an HTTP request and includes that data within the immediate response in an unsafe way.



https://portswigger.net/web-security/cross-site-scripting
