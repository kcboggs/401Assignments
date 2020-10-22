# Cloud Network Traffic Analysis
### How Traffic Mirroring works

> "Traffic Mirroring copies inbound and outbound traffic from the network interfaces that are attached to
your Amazon EC2 instances. You can send the mirrored traffic to the network interface of another EC2
instance, or a Network Load Balancer that has a UDP listener."

**Required procedures** 

• Identify the traffic mirror source (Source A)  
• Identify the traffic mirror source (Source B)  
• Configure the traffic mirror target (Target D)  
• Configure the traffic mirror filter (Filter A)  
• Configure the traffic mirror session for Source A, Filter A, and Target D  
• Configure the traffic mirror session for Source B, Filter A, and Target D  

_After you create the traffic mirror session, any traffic that matches the filter rules is encapsulated in a
VXLAN header. It is then sent to the target._    

**Traffic mirror targets**
_the destination for mirrored traffic_

• A network interface  
• A Network Load Balancer  

**Network Load Balancer considerations**    
• There must be UDP listeners on port 4789.  
• If all of the Network Load Balancer traffic mirror targets in an Availability Zone become unhealthy, the  
mirrored traffic can still be sent to traffic mirror targets in other zones

https://docs.aws.amazon.com/vpc/latest/mirroring/vpc-tm.pdf#traffic-mirroring-how-it-works

