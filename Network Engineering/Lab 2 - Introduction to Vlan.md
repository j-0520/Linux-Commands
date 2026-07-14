
Tasks Accomplished 

Setup a network of just pc's and a switch 

Seperated it into a finance, HR and IT set of computers 

Confirmed that they can ping each other on the same subnet - for example 192.168.10.x can speak to 192.168.10.x without a router 

However changing the IP address to 192.168.20.x causes the connection to fail between the laptops and they cannot ping each other 

**VLAN SETUP**

Made all laptops 192.168.10.x 
went into the switch and based on the fast ethernet ports, setup VLan 10 for Finance, VLan 20 for HR and VLan 30 for IT

Confirmed that while these devices had the same IP address as before, they can no longer communicate with each other 

eg: all had 10.x but could not ping one another 
this is important for real world - cant have HR people access IT or Finance and vice versa