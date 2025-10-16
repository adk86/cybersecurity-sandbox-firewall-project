
# Cybersecurity Sandbox, Firewall & Access Control

### Author: Jesse Ebosele  
**Course:** CS4371 – Computer Security Systems, Fall 2025  
**Role:** Cybersecurity Analyst  

---

## 🧠 Project Overview
This project demonstrates practical cybersecurity and network defense skills through the design, implementation, and testing of a **virtual sandbox environment**.  
The goal was to simulate a secure enterprise network, apply **firewall and access control policies**, and validate security configurations through hands-on testing and analysis.

---

## 🎯 Objectives
- Build a **virtualized sandbox environment** using Oracle VirtualBox and pfSense.
- Configure internal (trusted) and external (untrusted) network zones.
- Implement **router and host firewall policies** using pfSense and Linux `iptables`.
- Perform **network discovery and vulnerability testing** with Nmap.
- Analyze traffic and verify enforcement using **Wireshark packet captures**.
- Document the system configuration, results, and lessons learned.

---

## 🧰 Tools & Technologies Used
| Category | Tools |
| Virtualization | Oracle VirtualBox |
| Firewall/Router | pfSense |
| Operating Systems | Ubuntu Linux, Windows XP, Kali Linux, Windows 95 |
| Network Analysis | Wireshark, Nmap |
| Security Configuration | iptables, pfSense Rules |
| Documentation | ReportLab (PDF generation), Markdown |

---

## 🔐 Skills Demonstrated
- Network Hardening & Security Policy Implementation  
- Packet Capture & Traffic Analysis  
- Firewall Configuration (pfSense / iptables)  
- Virtual Machine Deployment & Segmentation  
- Vulnerability Detection and Remediation  
- Technical Documentation & Cybersecurity Reporting  

---

## 🧩 Implementation Summary
- Created isolated virtual subnets to represent **internal and external** networks.
- Configured pfSense rules to:
  - Allow external web (HTTP/HTTPS) access only to the internal web server.
  - Restrict external SSH and ICMP access.
  - Permit internal hosts limited outbound connectivity.
- Tested configurations using **Nmap scans** and verified traffic using **Wireshark captures**.
- Applied Linux host firewalls (`iptables`) to reinforce endpoint-level security.

---

## 📊 Results
- External scans revealed **only ports 80/443 open**, validating restricted exposure.
- Internal users retained SSH and web access to the server.
- ICMP and unauthorized service traffic were correctly filtered.
- Demonstrated measurable improvement in network security posture.

---

## ⚙️ Challenges & Resolutions
| Issue | Solution |
|-------|-----------|
| Misconfigured pfSense rule blocking SSH traffic | Adjusted rule order and direction. |
| Ubuntu `iptables` policy accidentally flushed | Reconstructed rules from saved configuration logs. |
| Nmap port inconsistencies | Verified with multiple scan types and Wireshark captures. |

---

## 📘 Lessons Learned
This project reinforced the importance of **layered security**, precise **firewall rule ordering**, and **continuous verification**.  
It provided hands-on experience relevant to **cybersecurity analyst roles**, emphasizing analytical thinking and defensive configuration in real-world network scenarios.

---
