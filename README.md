# ARP-Attack-and-Network-Sniffing
# Explore Network Sniffing and ARP Attacks

# AIM:

To explore network sniffing and ARP Attacks

## STEPS:

### Step 1:

Install kali linux either in partition or virtual box or in live mode

### Step 2:

Investigate on the various categories of tools as follows:


### Step 3:
Open terminal and try execute some kali linux commands

## ARP Attacks:  
ARP spoofing: A hacker sends fake ARP packets that link an attacker's MAC address with an IP of a computer already on the LAN. 
Boot kali and Windows7 virtual machines.
In windows 7 give the command arp -a
## OUTPUT:

<img width="1205" height="709" alt="image" src="https://github.com/user-attachments/assets/9622f8d7-031c-4893-a79a-1cf0216a6b51" />
Purpose:

Displays the ARP (Address Resolution Protocol) table/cache of your machine.

What ARP table contains:

Mapping between:
IP Address → MAC Address

From kali linux issue the command :
sudo arpspoof -i eth0 -t <target system> <gateway>

Explanation part by part:

sudo
Runs the command with administrator (root) privileges.
Needed because network packet manipulation requires elevated permissions.
arpspoof
A tool used to send fake ARP (Address Resolution Protocol) messages on a local network.
Commonly used in authorized network security labs to demonstrate ARP poisoning / man-in-the-middle concepts.
-i eth0
-i means interface.
eth0 is the network interface (network adapter) being used.
So the attack packets are sent through eth0.
-t <target_ip>
-t means target.
Specifies the victim machine’s IP address.
<gateway_ip>
Usually the router/default gateway IP.
The command tells the victim that the attacker’s MAC address belongs to this gateway IP.
## OUTPUT:


 dsniff:

<img width="353" height="128" alt="Screenshot 2026-05-12 200712" src="https://github.com/user-attachments/assets/feec4610-4a3c-41dd-8ca9-7e62a8daf7b6" />


Meaning:

dsniff is a network packet sniffing tool.

Purpose:

Captures and analyzes network traffic on a local network.
Commonly used in authorized security labs to observe unencrypted traffic.

What it can do:

Monitor packets passing through the network
Extract readable data from insecure protocols such as:
HTTP
FTP
Telnet
POP3
IMAP

Example:
If a machine sends plain-text login credentials over HTTP/FTP, dsniff may display that data because it is unencrypted.


In Metasploit open the ftp console as below. Also you can try other ftp websites ftp.vim.org
## OUTPUT:
<img width="614" height="435" alt="Screenshot 2026-05-12 203632" src="https://github.com/user-attachments/assets/9de302b4-a68b-436b-9544-2d7d7e840c4c" />




In Kali issue the following commands:
sudo dsnifff
## OUTPUT:
<img width="920" height="1030" alt="VirtualBox_kali_12_05_2026_19_50_51" src="https://github.com/user-attachments/assets/fe6fbb23-e143-4843-b363-6e22f9f22559" />


Explanation:

sudo
Runs the command with administrator/root privileges.
Needed because capturing network packets requires elevated permissions.
dsniff
Starts the packet sniffing tool.
Listens to network traffic and tries to extract readable information from unencrypted protocols.

What happens:

The tool begins monitoring packets on the default network interface (or a specified one if you use -i).
It may display information such as:
HTTP data
FTP usernames/passwords
Telnet sessions
Other plain-text network traffic

Invoke the wireshark and examine the various menus  and controls of the tool:
<img width="920" height="1030" alt="image" src="https://github.com/user-attachments/assets/69455035-c734-41a8-bca6-4b74b11a0d6d" />




# ARP SPOOFING

<img width="866" height="897" alt="Screenshot 2026-05-12 202829" src="https://github.com/user-attachments/assets/b6436163-4ef2-4260-b1e1-5bde70008c15" />
<img width="627" height="727" alt="Screenshot 2026-05-13 093824" src="https://github.com/user-attachments/assets/c1f47afc-edd5-4052-959b-d79e24ef7643" />
<img width="924" height="930" alt="Screenshot 2026-05-13 095052" src="https://github.com/user-attachments/assets/c6a0fccc-0b2d-458d-af1b-fcaf5aabda6f" />
<img width="956" height="949" alt="Screenshot 2026-05-13 094749" src="https://github.com/user-attachments/assets/1ac3556b-2a59-4740-aaf4-927f4ae9b6d3" />




## RESULT:
The kali linux tools for ARP Attack and Network Sniffing were identified successfully
