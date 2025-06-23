# 🔐 Elevate Labs Cybersecurity Internship – Task 1: Network Scanning

Welcome to the first task of my Cybersecurity Internship at **Elevate Labs**. This task focused on performing a comprehensive **network scan** to identify active hosts, open ports, and analyze associated security risks using tools like **Nmap** and **Wireshark**.

---

## 🎯 Objective

To scan the local network for open TCP ports, identify the services running on those ports, and assess the potential security implications of exposed services.

---

## 🛠️ Tools & Environment

- **OS:** Linux (Ubuntu)
- **Tools Used:**
  - [Nmap](https://nmap.org/) – Port scanning
  - [Wireshark](https://www.wireshark.org/) – Packet analysis
- **IP Range Scanned:** `192.168.15.0/24`

---

## 🔧 Task Workflow

1. Installed Nmap via package manager.
2. Identified local IP address and subnet using `ifconfig`.
3. Performed a **TCP SYN scan** using:

4. Collected open port and service information from active hosts.
5. Captured packets using Wireshark during the scan for deeper insight.
6. Analyzed services running on open ports.
7. Documented security risks and provided recommendations.

---

## 📊 Key Results

| Port | Protocol | Service       | Risk Summary                             |
|------|----------|----------------|------------------------------------------|
| 135  | TCP      | msrpc          | Vulnerable to DCOM/RPC-based attacks     |
| 139  | TCP      | netbios-ssn    | Used for Windows file sharing; risky     |
| 445  | TCP      | microsoft-ds   | Target for SMB exploits & ransomware     |
| 53   | TCP      | DNS            | Risk of amplification or data leakage    |

---

## 📁 Repository Contents

- 📄 `Network_Scanning_Task_with_Cover.docx` – Full documentation with professional formatting and analysis.

---

## ✅ Takeaways

This task reinforced the importance of:
- Regular internal port audits
- Minimizing exposed services
- Understanding how attackers view network surface areas
- Using tools like Nmap and Wireshark for hands-on insight

---

## 🙋‍♀️ About Me

**👩 Name:** Voonna Venkatesh 
**🎓 Role:** Cybersecurity Intern @ Elevate Labs  
**🔗 LinkedIn:** [linkedin.com/in/voonna-venkatesh/]((https://www.linkedin.com/in/voonna-venkatesh/))  


---

> ⚠️ **Disclaimer:** This scanning task was performed in a safe, authorized lab environment. Unauthorized scanning of networks without permission is prohibited and unethical.
