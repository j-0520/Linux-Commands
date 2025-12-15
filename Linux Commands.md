																											
**Basic commands**

- sudo 
	- elevates privileges 

- su {} 
	- replace {} with the user you want to switch to 
	- useful to switch between users

- sudo su - 
	- this sets you as **Root**
	- use **ONLY** as required

- ls 
	- lists the files in the specific directory 

- ls -la 
	- lists **ALL** files within the specific directory including hidden files


**Networking commands**

- IP a 
	- identifies the ip information in colors - use it instead of ifconfig

- Route
	- shows the routing table useful for understanding the gateway etc.

- ping
	- pings a specific IP address

- apache2 
	- usually done by sudo service apache2 start
	- Spins up a webserver on your ipaddress
	- this can host information and files on it

- python3 -m http.server ()
	- () = your desired port number
	- this can be used to again host information and grab files 

ifconfig



**File Commands**

- echo {} > ().txt
	- this is to type something into a file 
		- replace {} with the text 
		- replace () with the filename.txt

- echo {} >> ().txt 
	- this is to add something to an already written file 
	- if you were to just have singular > it would overwrite the file 
	- >> adds it to the next line of the file 

- touch (filename.txt)
	- this is to create a new file without having to input any text 

- cat (filename.txt)
	- this is to open and read the contents of the file
		- note: not all files can be open by all users you may need to **Sudo**. If you don't have **Sudo** privileges then you may not be able to open file

- nano (filename.txt) 
	- this is to open the file up and be able to type out all info required

- mousepad 
	- this is the best way to edit files 
		- legitimate linux version of notepad on windows
		- easiest to use and graphical 

- grep
	- grep grabs a line from a file based on what you specify to search for 
	- eg: cat ip.txt | grep "64 bytes"


**System commands**

- sudo apt update && apt upgrade 
	- this updates the operating system
	- also goes out to known repositories and upgrading to latest version for tools

**SSH**
- SSH (username)@(ipaddress)

**Scripting in bash**

**always start programs with #!/bin/bash**

