
**Networking Notes**

 **NAT** = Network address translation 

if the IP address is 192.xxxx or 10.xxx or 172.xxx/ these are private IP addresses
	this is to resolve the issue of too many IPv4 addresses
	all of these IP addresses goes out to the internet through one IP address (solving the IPv4 range shortage)

**MAC address**
 - MAC address is the unique address of the device. It is not used in IP addresses its just for identifying which device is which on the network
 - MAC addresses are used for layer 2 (switching) so the packets know which specific device to go to once on the correct network


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