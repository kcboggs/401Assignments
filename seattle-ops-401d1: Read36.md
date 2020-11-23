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
simplest variety of cross-site scripting. It arises when an application receives data in an HTTP request and includes that data within the   immediate response in an unsafe way.  
### What can XSS be used for?
**An attacker who exploits a cross-site scripting vulnerability is typically able to:**
* Impersonate or masquerade as the victim user.  
* Carry out any action that the user is able to perform.  
* Read any data that the user is able to access.  
* Capture the user's login credentials.  
* Perform virtual defacement of the web site.  
* Inject trojan functionality into the web site.  
### Impact of XSS vulnerabilities
**he actual impact of an XSS attack generally depends on the nature of the application, its functionality and data, and the status of the compromised user. For example:**  
* In a brochureware application, where all users are anonymous and all information is public, the impact will often be minimal.  
* In an application holding sensitive data, such as banking transactions, emails, or healthcare records, the impact will usually be serious.  
* If the compromised user has elevated privileges within the application, then the impact will generally be critical, allowing the attacker to take full control of the vulnerable application and compromise all users and their data.  
### How to prevent XSS attacks
* Filter input on arrival. At the point where user input is received, filter as strictly as possible based on what is expected or valid input.  
* Encode data on output. At the point where user-controllable data is output in HTTP responses, encode the output to prevent it from being interpreted as active content. Depending on the output context, this might require applying combinations of HTML, URL, JavaScript, and CSS encoding.  
* Use appropriate response headers. To prevent XSS in HTTP responses that aren't intended to contain any HTML or JavaScript, you can use the Content-Type and X-Content-Type-Options headers to ensure that browsers interpret the responses in the way you intend.  
* Content Security Policy. As a last line of defense, you can use Content Security Policy (CSP) to reduce the severity of any XSS vulnerabilities that still occur.  



https://portswigger.net/web-security/cross-site-scripting
