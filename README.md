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
# 🛡 Cybersecurity Lab – Phishing Email Analysis (Task 2)

This repository contains the analysis and report for *Task 2: Analyze a Phishing Email Sample* as part of the *Cybersecurity Internship* at *Elevate Labs*.

## 📌 Objective

To analyze a suspicious phishing email and identify key indicators of a phishing attack using various open-source tools.

---

## 🧪 Tools Used

- [PhishTank](https://www.phishtank.com/)
- [MXToolbox](https://mxtoolbox.com/)
- [VirusTotal](https://www.virustotal.com/)
- [WHOIS Lookup](https://whois.domaintools.com/)

---

## 🔍 Analysis Summary

The phishing email analyzed was crafted to impersonate the *SMBC Bank* and used tactics such as:
- *Spoofed email address* (noreply@smbc-cardnb.club)
- *Suspicious link* redirecting to a phishing domain
- *Urgent language* prompting the user to verify their account
- *Mismatched URL* that does not belong to the legitimate SMBC domain

---

## 📥 Sample Email Content

```text
Subject: [Important] Your SMBC Card Account Needs Immediate Attention

From: noreply@smbc-cardnb.club

Dear Customer,

We have detected suspicious activity in your account and have temporarily suspended access for your protection.

👉 Verify My Account: https://smbc-cardnb.club

Failure to act within 24 hours may result in permanent account suspension.

Thank you for your cooperation,  
SMBC Card Security Team


