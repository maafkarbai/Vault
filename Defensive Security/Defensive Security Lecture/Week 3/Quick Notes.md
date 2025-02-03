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

## Media Independent:
- Means No matter if it's lan, Wan etc
- No matter if fiber optic or ethernet

Hop Count in Time to live?
## Traceroute
- To check the nodes / route of the packet from src to destination
- How it works?

## ARP
- Used to resolve IP AND MAC Address

- ### **1. Device Needs to Send a Packet**

A device wants to send a packet to another device but only has its IP address.

### **2. ARP Request (Broadcast)**

The sender checks its ARP cache. If the MAC address is unknown, it sends an ARP Request to all devices in the subnet. Example ARP Request:

> "Who has 192.168.1.10? Tell me your MAC address."

### **3. ARP Reply (Unicast)**

The device with the requested IP responds with its MAC address:

> "192.168.1.10 is at AA:BB:CC:DD:EE:FF"

### **4. ARP Cache Update**

The sender stores the MAC address in its ARP table to avoid sending another request soon.

### **5. Packet Transmission**

Now that the sender has the MAC address, it forwards the data packet using Ethernet frames.

# MAC Adressing
- They change with each hop
- IP Addresses don't change