# Local Vulnerability Assessment Report (Nessus)

# Task Objective

To perform a  vulnerability assessment on the local Kali Linux system (localhost) using Nessus Essentials to identify, document, and plan remediation for critical security weaknesses.

---

# Steps Executed

1.  Service Initialization: Ensured the `nessusd` service was running.
2.  Scan Configuration: Created and configured a Basic Network Scan in the Nessus web interface.
3.  Target Setting: Set the scan target to the local loopback address: `127.0.0.1`.


#Key Findings Summary

The scan identified *65 vulnerabilities* across the system:

Critical- 0 - (None Found) 
High- 1 Denial of Service (DoS) Risk 
 Medium- 1  Denial of Service (DoS) Risk 
 Low  0  (None Found) 
 Info -63  Service Detection & Configuration Notes 

# Top Vulnerabilities Identified:

1.  HIGH (7.5 CVSSv3): Python Library Brook -- 1.1.0 DoS
2.  MEDIUM (5.3 CVSSv3): Ruby REXML 3.3.3 - 3.4.2 DoS vulnerability


# II. Critical Vulnerabilities & Remediation Plan (Documentation)



1)Python Library Brook -- 1.1.0 DoS - HIGH 
Research and Upgrade: upgrade it to a version greater than 1.1.0 (or remove the package if unused).

2)Ruby REXML 3.3.3 - 3.4.2 DoS vulnerability - MEDIUM 
System Update: The best fix is usually to perform a full system update to pull the latest Ruby/REXML patches: `sudo apt update && sudo apt upgrade`. 


