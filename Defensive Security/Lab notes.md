## Trace Route
```
tracert <destination network name or end device address>
```

(Microsoft Windows systems)

or
```
traceroute<destination network name or end device address>
```
Ex: 
```traceroute www.cisco.com```
(Unix and similar systems)
## Ping Command 
EX: ping -c 4 www.cisco.com
- Here -c means for 4 pings
---

## Mininet
- Mininet is an **open-source network emulator** that creates a virtual network of hosts, switches, and links on a single machine.
### Starting Host in Mininet (start host 1)
```
xterm h1 
```

## Checking IP Address of a host / Check ip in linux
```
[root@secOps analyst]# ifconfig
```
- You get the Result
![[Pasted image 20250220144825.png]]
- after **inet there is IP for H1-eth1** 
- after **ether there is MAC for H1-eth1** 

### **`mn -c` Command in Mininet**

- The `mn -c` command is used to **clean up** Mininet by removing leftover network configurations from a previous session.
___
## Reading wireshark frame
![[1-slide11.jpg]]
- IP (0x0800) means IPV4