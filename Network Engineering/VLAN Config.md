
This is a notetaking for useful commands to make a VLAN setup 

on the switch CLI complete the following commands

-enable 
-configure terminal  
	These two commands above are just to begin configuring the switch
	Once in, complete the following

-vlan 10
-name (insert_name_here)

-vlan 20
-name (insert_name_here)

-vlan 30
-name (insert_name_here)
	this can be done for as many vlans as necessary to make 


once this is complete 

interface fastEthernet0/1
switchport mode access
switchport access vlan (desired ethernet number here)


interface fastEthernet1/1
switchport mode access
switchport access vlan (desired ethernet number here)

interface fastEthernet2/1
switchport mode access
switchport access vlan (desired ethernet number here)

these commands tell the switch hey for the device that's connected on this ethernet port, make it part of this vlan please

