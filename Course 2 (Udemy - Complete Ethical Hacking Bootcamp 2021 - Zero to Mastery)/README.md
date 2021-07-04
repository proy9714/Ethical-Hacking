# Reconnaissance and Information gathering:
---------------------------------------------

nslookup - Lookup ip address

whois - ip/domain details

whatweb - web scanner to scan hosts

theHarvester - email gathering

hunter.io - website for email gathering

redhawk - website information gathering

sherlock - find accounts across social media using username

arp - manipulate the system arp cache


# SCANNING: 
-----------------------

netdiscover - For discovering available networks/ips. 

netstat - (Obsolete) Use ss

nmap - Scanning for ports
	-sS : Syn Scan, half open scanning...detecting replies from syn tcp packets
	-sF : Fyn scan (?)
	-sV : Version number
	--version-intensity : 0 to 9, default:7
	-A : Aggressive
	-sn : No port can, like netdiscover
	-p : port range/ single port scan
	>> filename : to save output to file
	-oN : Output scan in normal file
	-f : Small fragmented tcp packets
	-D : decoys, Make it appear to the target as if multiple ips have scanned target (for hiding attacker ip)
	-S : spoof your ip address, but results of scan sent to spoofed ip
	-Pn : Doesn't perform ping scan, assumes all hosts are online (HAVE to use the -S)
	-e : A network interface (eg: eth0)
	-g : Source port (Maybe to bypass firewall)
	-T : Timing template
	-F: Fast mode - Scan fewer ports than the default scan
	
	nmap scripts - For finding vulnerabilities, explore documentation of nmap on internet
	nmap scripts are in directory: usr/share/nmap/scripts
	nmap --script scriptgroup
	Script help: nmap --script-help scriptname 

man {{command}} - manual of command

Connect using fpt: ftp target-ip

searchsploit - exploiting vulnerabilities

locate filename - Outputs the path of concerned filename

Nessus - Software for vulnerability analysis