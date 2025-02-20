
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

## Opening wireshark in ARCH Linux

```
wireshark-gtk &
```

---
## Reading wireshark frame
![[1-slide11.jpg]]
- IP (0x0800) means IPV4

## Ethernet Frame
![[Pasted image 20250220150516.png]]
![[Pasted image 20250220150415.png]]

## Check ARP Cache
```
arp -n
```
## How to clear ARP Cache 
```
arp -d IP-Address
```
## How to check Default Gateway info
```
netstat -f
```
---
NMAP Scanning 
### **Nmap Aggressive Scan Timing **

| Option | Timing Template  | Speed     | Stealth                               |
| ------ | ---------------- | --------- | ------------------------------------- |
| `-T0`  | Paranoid         | Slow      | Very stealthy                         |
| `-T1`  | Sneaky           | Slow      | Stealthy                              |
| `-T2`  | Polite           | Medium    | Reduces impact on target              |
| `-T3`  | Normal (Default) | Moderate  | Balanced                              |
| `-T4`  | Aggressive       | Fast      | Easily detectable                     |
| `-T5`  | Insane           | Very fast | Very loud & likely to miss open ports |
*Use:*
```
nmap -T4  192.168.1.1
```

### What `nmap -A` Does?
**Example:** 
```
nmap -A -T4 192.168.1.1
```
- `-A` → **Enables OS detection**, version detection, script scanning, and traceroute.
- `-T4` → Uses **aggressive timing** for faster scanning.
### **When to Use `-A`?**
✅ When you need **detailed information** about the target.  
✅ Useful for **penetration testing** and **reconnaissance**.  
⚠️ Not stealthy—**can trigger firewalls and IDS**.

### Specifying Subnet Mask in nmap
```
nmap -A -T4 192.168.1.0/24
```
- /24 means 255.255.0.0 subnet mask
