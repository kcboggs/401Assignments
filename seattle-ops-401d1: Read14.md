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

# Traffic mirror filters and filter rules
_A traffic mirror filter is a set of inbound and outbound traffic rules that define the traffic that is copied
from the traffic mirror source, and sent to the traffic mirror destination_

### Traffic mirror filter rules
_Traffic mirror filter rules define what traffic gets mirrored_
• Traffic direction: Inbound or outbound  
• Action: The action to take, either to accept or reject the packet  
• Protocol: The L4 protocol  
• Source port range  
• Destination port range  
• Source CIDR block  
• Destination CIDR block  

### Traffic mirror sessions
_A traffic mirror session establishes a relationship between a traffic mirror source and a traffic mirror
target._
• A traffic mirror source  
• A traffic mirror target  
• A traffic mirror filter

### Traffic Mirroring and VPC Flow Logs
• Allowed and denied traffic  
• Source and destination IP addresses  
• Ports  
• Protocol number  
• Packet and byte counts  
• Action taken (accept or reject)  

### Traffic mirror source and target connectivity
options
• The same VPC, or  
• A different VPC connected by using an intra-Region VPC peering connection or a transit gateway  







https://docs.aws.amazon.com/vpc/latest/mirroring/vpc-tm.pdf#traffic-mirroring-how-it-works

