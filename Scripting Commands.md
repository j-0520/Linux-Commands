#!/bin/bash 

if [ "$1" == "" ] 
then 
echo "you forgot an IP address"
echo "Syntax: ./ipsweep.sh 10.0.2"

else
for ip in `seq 1 254`; do
ping -c 1 $1.$ip | grep "64 bytes" | cut -d " " -f 4 | tr -d ":" &
done
fi
- this script first checks that the command line entry alongside the ./ipsweep.sh is there (otherwise returns nothing) 
	- if an entry is given then move into executing the code below
- this script goes through each ip address on the subnet  (1 - 254) and grep for successful returns "64 bytes" (checking that the IP address works and returns a ping)
- cut -d " " -f 4 - cut the response by a space and cut off by the 4th space 
- tr -d ":" - remove the : from the response



**for ip in $(cat ips.txt); do nmap $ip; done  **

- basic nmap scan for all the Ip addresses if you have saved it to a file named ips.txt 