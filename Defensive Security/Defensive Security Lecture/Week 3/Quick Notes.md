# Protocols
- Each protocol has it's own Header
- They have fields 
- Message formats?
- Message Encapsulation (Adding data to header)
- Message Decapsulation (Removing the headers like opening an envelope)
- Each protocol much have a size limit (must be divided)
- Receiver must rearrange the message parts using sequence no.
- what is retransmitting?
	- When data is corrupted data is retransmitted
-What are reliable protocols?
 - Used to knowledge the message has been sent
 
- What is collision?
- What is unicast, multicast, broadcast?
	- Uni for single only
	- Multi for multiple 
	- Broad for all

- Application layer:
	- Apps like netflix,Outlok
	- User interacts
	- Interface
	- Manages the format of data 
	- Manages sessions of apps
	- DNS for resolving urls to an ip
	- DHCP for assigning ips
- Transport layer
	- Delivers the data 
	- TCP
		- Guarantees delivery
		- Resends if not sent 
	- UDP
- Network Layer
	- Manages multiple networks 
	- Like connecting one network to another 
	- IPV4, IPV6 
	- For Routing

Media Independent:
	- Means No matter if it's lan, Wan etc
	- No matter if fiber optic or ethernet

Hop Count in Time to live?