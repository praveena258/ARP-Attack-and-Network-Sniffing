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

From kali linux issue the command :
sudo arpspoof -i eth0 -t <target system> <gateway>
## OUTPUT:


 dsniff:

<img width="353" height="128" alt="Screenshot 2026-05-12 200712" src="https://github.com/user-attachments/assets/feec4610-4a3c-41dd-8ca9-7e62a8daf7b6" />





In Metasploit open the ftp console as below. Also you can try other ftp websites ftp.vim.org
## OUTPUT:
<img width="614" height="435" alt="Screenshot 2026-05-12 203632" src="https://github.com/user-attachments/assets/9de302b4-a68b-436b-9544-2d7d7e840c4c" />




In Kali issue the following commands:
sudo dsnifff
## OUTPUT:
<img width="920" height="1030" alt="VirtualBox_kali_12_05_2026_19_50_51" src="https://github.com/user-attachments/assets/fe6fbb23-e143-4843-b363-6e22f9f22559" />



Invoke the wireshark and examine the various menus  and controls of the tool:
<img width="920" height="1030" alt="image" src="https://github.com/user-attachments/assets/69455035-c734-41a8-bca6-4b74b11a0d6d" />


<img width="866" height="897" alt="Screenshot 2026-05-12 202829" src="https://github.com/user-attachments/assets/b6436163-4ef2-4260-b1e1-5bde70008c15" />


## RESULT:
The kali linux tools for ARP Attack and Network Sniffing were identified successfully
