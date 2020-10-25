# Threat Analysis, Cyber Kill-Chain, and Stuxnet
### BREAKING THE KILL CHAIN: A DEFENSIVE APPROACH
> " First developed by Lockheed Martin, the Cybersecurity Kill Chain is a model for describing the steps an attacker must 
complete to carry a successful attack."

This model is made up of 7 sequential steps, including:  
1. Reconnaissance  
2. Weaponization  
3. Delivery  
4. Exploitation  
5. Installation  
6. Command and Control  
7. Actions on Objectives  

_To disrupt the attack, one or more of these steps must be broken for the entire chain to fail. And in order for us to do that, we need to understand their playbook_

### Reconnaissance
Firstly gather information about the victim
The two different stages of reconnaissance are passive and active

During **Passive** reconnaissance, an attacker will use indirect methods to gather information from publicly available sources like WHOIS, ARIN registrations, Google, Shodan, Job Listings and  company websites.
Once an attacker has collected as much public information as possible, the attacker will move on to **Active** reconnaissance, which involves some level of interaction with your organizations. 
_The entire goal of the reconnaissance phase is to find a weakness that can be exploited. Once the attacker has found that weakness, they can move on to the next step._


### Weaponization
Once an attacker has found a weakness, their next step is find or create the attack that will exploit the vulnerability  
* Metasploit or exploit-db for publicly available exploits  
* The Veil framework is commonly used to generate evasion code for malware  
* Social Engineering Toolkit, if they’ve decided they will deliver the malware through a Social Engineering campaign.   

### Delivery
By this point, the attacker has selected the weapon based on their earlier reconnaissance.   

Examples of delivery channels are:   
* Websites (malicious or clean): An attacker can infect a legitimate website they know your users frequent.  
* Social media: Cat phishing via social networks is a very effective way to gain trust  
* User input: The attacker has some level of interaction with a server (like a web server or a DB)  
* Email: Attackers love phishing email because it works. Phishing is usually a numbers game. If only .    
  1% of a 20k enterprise corporation click on a link, I’ve successfully infected 20 people.  
* USB: Common attack to leave infected USB’s in public areas and around employee’s car hoping the temptation is too much.   

_DKIM and SPF are email authentication method to detect spoofed emails. SPF makes sure that emails are coming from the authorized IP of the domain while DKIM uses digital signatures. Both techniques help to make sure emails are coming from legitimate, authorized channels._ 

Some other effective measures include: 
* Webfiltering can prevent a user from accessing questionable or known bad sites  
* Disabling USB and not giving any user “admin” rights also prevents a big portion of delivery mechnism that malware can use  
* DNS Filtering: While web filtering blocks web request destined to malicious sites, using a DNS security solution can block any DNS lookup attempt to prevent connections over any protocol. I always use this is combination with web filtering. 

### Exploitation
Protective measures are limited once an attacker has been able to execute the exploit but they do exist:   
* DEP (Data Execution Prevention) is a software and hardware feature which attempts to prevent the execution of code in memory where it doesn’t belong.      
* Anti-Exploit is a feature on some AV solutions that monitor known applications for unusual calls to memory.  
Both of these techniques act as the last line of defense against common exploit attempts

### Installation
Some common payloads and techniques during this stage involve:  
* DLL hijacking  
* Injecting Meterpreter or other similar payloads  
* Installing Remote Access Tools (or RAT)  
* Registry changes to make my program automatically start up  
* Executing Powershell in fileless attacks  

### Command and Control
_At this stage, the system has been completely compromised and in control of the attacker. If they completed the previous stage correctly, their access is persistent – even if you reboot or patch the vulnerability._

https://thecisoperspective.com/index.php/2020/03/27/breaking-the-kill-chain-a-defensive-approach/
