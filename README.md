# Penetration Testing Report – Footprinting & Network Scanning

## 📌 Project Overview

This repository contains my **Week 2 cybersecurity penetration testing report** completed as part of the **B082-Networkwalks** program.

The project covers two main phases:

- **Phase 1 – Reconnaissance & Footprinting**
- **Phase 2 – Scanning & Network Discovery**

The assessment demonstrates how publicly available information can be collected from a domain and how an authorized local network can be mapped to identify live hosts.

> ⚠️ **Authorization:** All activities were performed only on systems owned by me or within an explicitly authorized scope. This project is intended for educational and security research purposes only.

## 🛠️ Tools Used

| Tool | Purpose |
|---|---|
| Kali Linux | Reconnaissance and footprinting |
| Windows | Local network identification and scanning |
| WHOIS | Domain registration and name-server information |
| WhatWeb | Web technology fingerprinting |
| nslookup | DNS/domain-to-IP resolution |
| curl -I | HTTP response-header inspection |
| Wafw00f | Web Application Firewall detection |
| DNSRecon | DNS record enumeration |
| Zenmap (Nmap GUI) | Local network host discovery and topology |
| Windows CMD | Local IP, subnet and MAC-address identification |
| Maltego | Email/domain relationship analysis |

## 🔎 Activities Performed

### 1. Footprinting & Reconnaissance

The target domain was assessed using:

- WHOIS
- WhatWeb
- Nslookup
- Curl
- Wafw00f
- DNSRecon

The assessment collected information related to domain registration, web technologies, IP addressing, HTTP headers, WAF technology, DNS records, mail servers and other publicly exposed infrastructure information.

### 2. Network Scanning with Zenmap

Zenmap was used on my own local network to:

- Identify the local IP address and subnet
- Discover live hosts
- Identify IP and MAC addresses
- Generate a network topology

### 3. Maltego – Email Footprinting

Maltego was used during the reconnaissance phase to perform email footprinting and identify publicly available information associated with the target domain/email infrastructure.

The discovered information was represented as a visual relationship graph to help understand connections between domains, emails and other publicly available entities.

## 📊 Risk Analysis

The assessment identified observations including:

| Finding | Risk |
|---|---|
| Web technology information exposed | Medium |
| Server IP address identifiable | Low |
| HTTP technical information exposed | Low |
| WAF technology identifiable | Low |
| DNS infrastructure information exposed | Medium |
| Multiple live hosts visible on local network | Medium |

These observations are **not confirmed vulnerabilities**. Further authorized vulnerability validation would be required.

## 🛡️ Recommendations

1. Review publicly exposed technology information.
2. Keep CMS, plugins and other software updated.
3. Review HTTP response headers.
4. Regularly review publicly exposed DNS records.
5. Properly configure and monitor the WAF.
6. Perform regular internal network discovery.
7. Investigate unknown devices.
8. Maintain updated network documentation.
9. Perform reconnaissance and scanning only with proper authorization.

## 📁 Repository Structure

```text
Penetration-Testing-Network-Scanning-Report/
├── README.md
├── report/
│   └── penetration-testing-report.md
└── evidence/
    └── README.md
```

## ⚖️ Liability & Legal Disclaimer

This penetration testing project is intended strictly for authorized security testing, educational, and research purposes. All activities were conducted only on systems owned by the tester or with explicit written permission from the authorized owner.

Unauthorized access, scanning, exploitation, modification or disruption of systems may violate applicable laws and may result in criminal, financial or civil penalties.

**Use this information responsibly, legally, and only within an authorized scope.**

## 👤 Author

**Joynul Hasan**  
Cybersecurity  
Program: **B082-Networkwalks**

LinkedIn: [Joynul Hasan](https://www.linkedin.com/in/joynul-hasan-12b3ab307/)

---

⭐ If this repository is useful for learning, feel free to star it.
