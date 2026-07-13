These are some notes on how to install / setup a router on packet tracer 

- put a router down (connect to a switch)
- enter the CLI 
- spam no on the setup (not necessary at this stage) 
- enter these commands 
-Enable
	 - this should get you to have router# instead of router>
-configure terminal 
	 - should change to Router(config)
-interface gigabitEthernet0/0
	- this should change it to be Router(config-if)
-no shutdown
	- this changes the ethernet to up state 
Routers come stock disabled, they must be enabled manually 

Once this has been done go onto the physical on the router and go GigabitEthernet 0/0 and set ip address as xxx.xxx.x.1 (this could be 192.168.0.1 or 192.168.1.1)
To determine which one it needs to be look at the network side its routing through. If its routing information from that switch which is apart of the .0 group then make it .0.1. if its from the .1 group then make it .1.1 

Another option is in CLI 
once in the interface gigabitEthernet0/x 
- type ip address (xxx.xxx.x.x and subnet mask xxx.xxx.xxx.x)


