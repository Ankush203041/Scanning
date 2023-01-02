# scanning


//nmap //
it is the most important tool used for scanning to get info about your target
Scanning types
-TCP Connect [nmap -sT]
-stealth scan [nmap -sS]
-Inverse TCP flag scanning
-Xmas Scan [nmap -sX -v]
-Ack Flag Probe Scan [nmap -SF]
-IDLE/PID Header Scan [nmap -sN]
UDP Scan [nmap -sU]


//analyzing TTl value and window size//
operating system       |   TTL        |    Window size
   Linux               |   64         |      5840
   Windows             |   128        |      8192
   CISCO Router        |   255        |      4128
  
//nmap scripts//
commands
ls -l /usr/share/nmap/scripts/     [to list all the scripts]
ls -l /usr/share/nmap/scripts/  | grep ssh     [to get only ssh scripts]
nmap --scripts=ssh-brute.nse 192.168.230.136   [to bruteforce ssh .....]


//wireshark//
//solarwinds//[download the software]

#Enumeration
enumeration is defined as the process of extracting user names machines names , network resources , shares and services from a system

enumeration techniques 
-enumeration using email-id
-enumeration using default password(cirt.net is a website to get defaults passwords of some devices)
-enumeration using SNMP 
Simple Network Management Protocol is an internet standard protocol for collecting and organizing information about managed devices on IP networks and for modifying that information to change device behavior

The SNMP system is conststing of three elements 
1- SNMP manager
2- SNMP agents
3- Management Information Base
......to be continued

-DNS enumeration 
DNS zone transfer is the process where a DNS server passes a copy of part of its database (which is called a "Zone") to another DNS server
commands
dnsenum website.com
host website.com
dig
nslookup

-NetBIOS enumeration
NetBIOS stands for network basic input output system. it allows computer communication over a LAN and allow them to share files and printers.
NetBIOS names are used to identifynetwor devices over TCP/IP (windows).
IT must be unique on a network , limited to 16 characters where 15 characters are used for the device name and the 16th character is reserved for identifying the type of service running or name recird type.
atteckers use the NetBIOS enumeration to obtain:
-list of computers that belong to a domain 
-list of shares on the individual host on network
-policies and posswards
commands 
nbtstst - 192.168.230.135


