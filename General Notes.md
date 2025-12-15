
**Networking Notes**

 **NAT** = Network address translation 

if the IP address is 192.xxxx or 10.xxx or 172.xxx/ these are private IP addresses
	this is to resolve the issue of too many IPv4 addresses
	all of these IP addresses goes out to the internet through one IP address (solving the IPv4 range shortage)

**MAC address**
 - MAC address is the unique address of the device. It is not used in IP addresses its just for identifying which device is which on the network
 - MAC addresses are used for layer 2 (switching) so the packets know which specific device to go to once on the correct network


**Subnetting**

- /24 subnet = 254 possible devices 
- it is 265 hosts however (first and last address are reserved for broadcast IP and network ID)
- 


**TCP vs UDP**

**TCP**
- TCP is the transmission control protocol
- TCP is connection orientated protocol
- used for reliability 
- think website (HTTPS)
- used in a three way handshake
- **SYN > SYN ACK > ACK**
- basically initial SYN (waving at someone) SYN ACK (them waving back) ACK (you understand and acknowledge its now good to approach and chat to them)
- if i want to connect to a host on port 443 (HTTPS) I send a SYN pack. If port 443 is open then host will send SYN ACK (basically saying yea im open) and then when I want to chat I send and ACK packet back (cool I now know your open to chat)

**UDP**
- UDP is user datagram protocol 
- connectionless protocol
- used for streaming services 


**Ports**
**TCP****
-  HTPP - 80 
-  HTTPS - 443
-  FTP - 21
- SSH - 22
- Telnet - 23
- SMTP - 25
- DNS - 53
- POP3 - 110
- SMB - 139 + 445
- IMAP 143
**UDP**
- DNS - 53
- DHCP - 67.68
- TFTP - 69
- SNMP - 161

**example**
if we search google.com - google.com resolves to an IP address by way of DNS (domain name system) 
the computer does not know what google.com is it has to search for the IP address


**OSI Model**

numonic 
 - please do not throw sausage pizza away

1 Physical - data cables eg: Cat6
2 Data - switching, MAC addresses
3 Networking - IP Addresses, routing
4 Transport - TCP, UDP 
5 Session - Session management
6 Presentation - WMV, JPEG, MOV
7 Application - HTTP, SMTP




**The 5 Stages of Ethical Hacking**

 1 **reconnaissance** 
	- Active / passive
	**Passive reconnaissance**
		- Things like looking at the company website, looking at a LinkedIn account 
		- looking at an employees Instagram account 
		- **not directly interacting with the target system**
	**Active reconnaissance**
		- NMAP scanning 
		- Nessus scanning 
		- enumeration (digging and searching for items of interest)
		- **directly interacting with the system**
(please note here that active reconnaissance kind of falls into step 2)

3 **gaining access (exploitation)**
	- this is running an exploit against the vulnerabilities found in section 1 to get a foothold into the system 
	- for example, brute force passwords, known exploits for enumerated information such as APACHE 

4 **Maintain access**
	- this is key for a prolonged attack 
	- need to be sure that if the user turns off their computer (you lose access) but if they turn it back on again you then have access again 
	- **OR**
	- deeper rooted access into server etc that never turns off 

5 **covering tracks**
	- deleting logs / malware pushed in 
	- delete any accounts or logs 
	- clean up 



**WGET**
 - Wget allows us to download files from the web via HTTP. 
	 - only thing is you must know the entire web address


**SCP (secure copy)**
 - a way of securely copying files using the SSH protocol for authentication and encryption 
	 - note: this is of course used for transferring between two computers




**Passive Reconnaissance**

**Location information**
- satellite images 
- drone recon 
- building layout

**Job information**
- Employees (name, job title, phone number, manager)
- pictures (badge photos, desk photos, computer photos)


**Web / host assessment**
	 **Target validation** 
		- WHOIS, nslookup, dnsrecon
	**Finding Subdomains**
		- Google FU, dig, nmap
	**fingerprinting**
		- NMAP, WhatWeb, netcat
	**Data breaches**
		-  HaveIBeenPwned, breachparse



