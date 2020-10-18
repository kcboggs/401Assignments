# Network Packet Analysis with Wireshark
Firstly, stealing is wrong and stealing passwords is unethical - DO NOT DO IT!!!!

## Capturing interesting network packets

1. All the packets on the network that actually arrive at your PCs (or Mac) will be inspected to check if they have a destination that matches the network card  
2. If the destination address is a match, the packets are destined for your PC and will be passed up to the CPU and processed    
3. If the destination address in the packet does not match the address of the network card the packets will simply be ignored and discarded

## The real big question
How can I capture packets to and from someone on another network than my own?

* Physically connected to the network they’re using  
* Physically connected to the Facebook networ  
* Physically connected to any network in between those two  
* Capture plain text wireless packets while sitting close to someone you want to steal credentials from  

## Finding the passwords  
Let’s say we somehow managed to get the packets we wanted, and they do contain the passwords we want. Which means that one of three things is the case

1. The network protocol transporting the packets is unencrypted  
2. The network protocol is encrypted, and we do not have the encryption keys  
3. Tthe network protocol is encrypted, but we have the encryption keys  

https://blog.packet-foo.com/2016/07/how-to-use-wireshark-to-steal-passwords/
