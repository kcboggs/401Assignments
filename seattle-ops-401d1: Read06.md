# Applying The CIA Triad To Your Enterprise File Transfer

> The CIA Triad refers to three basic principles/objectives in information security, namely: confidentiality, integrity, and availability.
It's been proven that, in order to establish a secure system, you need to achieve these three objectives. Let me explain each one first and
why they are crucial to business file transfers."

## Confidentiality
 _Confidentiality refers to the principle of restricting access to or knowledge of certain pieces of information to certain individuals._
 
 
## Integrity
_Pertains to the principle of preventing data from being tampered._

## Availability
_Ensures that information and resources are available to those who need them._

## CIA-Triad-in-One
> "Normally, in order to apply all three elements of the CIA Triad, you would need to employ disparate solutions and integrate them. The problem
with this approach is that it can be quite complex and would therefore require considerable time and expertise before you can come up with a complete
solution. A better option would be to find a single solution that already incorporates all three elements (and possibly more)._

An example of JSCAPE MFT Server, a managed file transfer server that already includes:

* Data-in-motion encryption through secure file transfer protocols like FTPS, SFTP, HTTPS, WebDAVs, AS2 over HTTPS, and OFTP (secured by SSL)  
* Data-at-rest encryption through OpenPGP   
* End-to-end encryption, which can be achieved through automation-enabling features known as triggers.   
* 2-factor authentication  
* Data integrity checking mechanisms that employ hash functions and digital signatures.  
* Built-in support for High Availability configurations, active-active and active-passive  
* Data Loss Prevention (DLP), which automatically detects the presence of sensitive data and take appropriate action (e.g. cancel the download or apply encryption)  

https://www.jscape.com/blog/implementing-the-cia-triad-when-transferring-files-through-the-internet

# What Are MD5, SHA-1, and SHA-256 Hashes

> "These seemingly random strings of text allow you to verify files you download aren’t corrupted or tampered with. You can do this with the commands built into Windows, macOS, and Linux."

## How Hashes Work, and How They’re Used for Data Verification

Hashes are the products of cryptographic algorithms designed to produce a string of characters.

![Hash](Hash Verification.png)

