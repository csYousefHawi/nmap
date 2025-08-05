 **## nmap (network mapper)



**Nmap** is a tool used to discover devices connected to a network and gather sensitive information without raising suspicion. It is commonly used by network administrators and ethical hackers for scanning and security assessment purposes.


 Features of Nmap: 
 - Discover IP addresses of connected devices 
 - Detect operating systems 
 - Scan open ports (Open Ports) 
 - Identify used protocols 
 - Detect MAC addresses 
 - Collect various types of network information


Common Nmap Commands:

  1- Basic Network Scan: Displays information about all devices connected to the network:
 ```bash 
 nmap (ip router)/24
 ```
 

 2- Finds connected devices without scanning ports:
 ```bash 
 sudo nmap -sn (ip router)/24
 
```
 3- Shows open ports without checking if the host is up:
 ```bash
 sudo nmap -Pn (ip router)/24
 
```
 Same as the above but more stealthy to bypass firewalls and detection systems:
```bash
sudo nmap -sS -Pn (ip router)/24
```
# or
```bash
sudo nmap -sS -sn (ip router)/24
```
-Notes: 
 Use sudo because some commands require administrative privileges.
 Use /24 to scan the full subnet range of the network.
 



