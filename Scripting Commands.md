
**#!/bin/bash** 
**for ip in `seq 1 254`; do**
**ping -c 1 (ip range) | grep "64 bytes" | cut -d " " -f 4 | tr -d ":"**
**done**
- this script goes through each ip address on the subnet and grep for successful returns "64 bytes" 
- cut -d " " -f 4 - cut the response by a space and cut off by the 4th space 
- tr -d ":" - remove the : from the response



**for ip in $(cat ips.txt); do nmap $ip; done  **

- basic nmap scan for all the Ip addresses if you have saved it to a file named ips.txt 