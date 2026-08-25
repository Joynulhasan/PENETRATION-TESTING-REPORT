# 🛡️ Penetration Testing Report – Footprinting & Network Scanning

## 📌 Project Overview

This repository contains my **Week 2 Cybersecurity Penetration Testing Report** completed as part of the **B082-Networkwalks** program.

The project covers two major phases of security assessment:

* 🔎 **Phase 1 – Reconnaissance & Footprinting**
* 🌐 **Phase 2 – Network Scanning & Network Discovery**

The objective of this project was to understand how security professionals can gather publicly available information about a target and perform authorized network discovery to identify live hosts and network infrastructure.

---

## 🎯 Objectives

* Perform domain footprinting and reconnaissance.
* Identify publicly available domain and DNS information.
* Fingerprint web technologies.
* Inspect HTTP response headers.
* Identify Web Application Firewall technology.
* Enumerate DNS records.
* Discover live hosts on a local network.
* Identify IP and MAC addresses.
* Perform email/domain footprinting using Maltego.
* Document security observations and potential risks.

---

## 🛠️ Tools Used

| Tool            | Purpose                                         |
| --------------- | ----------------------------------------------- |
| **Kali Linux**  | Reconnaissance and footprinting activities      |
| **Windows**     | Local network identification and scanning       |
| **WHOIS**       | Domain registration and name-server information |
| **WhatWeb**     | Web technology fingerprinting                   |
| **Nslookup**    | Domain-to-IP and DNS resolution                 |
| **Curl**        | HTTP response-header inspection                 |
| **Wafw00f**     | Web Application Firewall detection              |
| **DNSRecon**    | DNS record enumeration                          |
| **Zenmap**      | Network discovery and host scanning             |
| **Windows CMD** | Local IP, subnet and MAC-address identification |
| **Maltego**     | Email/domain relationship analysis              |

---

# 🔎 Activities Performed

## 1. Footprinting & Reconnaissance

I performed reconnaissance against the **networkwalks.com** domain using multiple Kali Linux tools.

### WHOIS

Used to obtain publicly available domain registration information and identify name servers.

### WhatWeb

Used to identify technologies used by the website, including web technologies and CMS-related information.

### Nslookup

Used to resolve the domain name and identify its associated IP address.

### Curl

Used with the `-I` option to inspect HTTP response headers and identify information exposed by the web server/application.

### Wafw00f

Used to determine whether a **Web Application Firewall (WAF)** was protecting the website.

### DNSRecon

---

# 🌐 2. Network Scanning with Zenmap

Zenmap was used to perform network discovery on my **own local network**.

The activities included:

* Identifying the local IP address.
* Identifying the LAN subnet.
* Discovering live hosts.
* Identifying IP addresses.
* Identifying MAC addresses.
* Creating a network topology.

Windows `ipconfig` was used to identify the local network configuration before performing the Zenmap scan.

---

# 🕵️ 3. Maltego – Email Footprinting

**Maltego** was used during the reconnaissance phase to perform **email footprinting** and identify publicly available information associated with the target domain/email infrastructure.

Maltego helps correlate publicly available information such as:

* Email addresses
* Domains
* Websites
* Usernames
* Social profiles
* Related entities

The discovered information can be represented as a **visual relationship graph**, making it easier to understand connections between different publicly available entities.

---

# 📊 Risk Analysis

The assessment identified several security observations:

| # | Finding                                      | Risk Level |
| - | -------------------------------------------- | ---------- |
| 1 | Web technology information exposed           | 🟠 Medium  |
| 2 | Server IP address identifiable               | 🟢 Low     |
| 3 | HTTP technical information exposed           | 🟢 Low     |
| 4 | WAF technology identifiable                  | 🟢 Low     |
| 5 | DNS infrastructure information exposed       | 🟠 Medium  |
| 6 | Multiple live hosts visible on local network | 🟠 Medium  |

> **Note:** These findings represent observations from reconnaissance and network discovery activities. They should not automatically be considered confirmed vulnerabilities. Further authorized security testing would be required for validation.

---

# 🛡️ Recommendations

1. Review publicly exposed web technology information.
2. Keep CMS, plugins, and other software updated.
3. Review HTTP response headers for unnecessary information exposure.
4. Regularly review publicly exposed DNS records.
5. Properly configure and monitor the Web Application Firewall.
6. Perform regular internal network discovery.
7. Investigate unknown or unexpected devices.
8. Maintain accurate network documentation.
9. Perform all reconnaissance and scanning activities only with proper authorization.

---

# 📁 Repository Structure

```text
Penetration-Testing-Network-Scanning-Report/
│
├── README.md
│
├── report/
│   └── penetration-testing-report.md
│
└── evidence/
    ├── README.md
    ├── 01-whois.png
    ├── 02-whatweb.png
    ├── 03-nslookup.png
    ├── 04-curl.png
    ├── 05-dnsrecon.png
    ├── 06-wafw00f.png
    ├── 07-zenmap-scan.png
    ├── 08-zenmap-topology.png
    └── 09-maltego.png
```

---

# 📸 Evidence


* WHOIS
* WhatWeb
* Nslookup
* Curl
* DNSRecon
* Wafw00f
* Zenmap Scan
* Zenmap Topology
* Maltego

---

# ⚖️ Liability & Legal Disclaimer

This project is intended strictly for **authorized security testing, educational, and research purposes**. All activities were performed only on systems owned by the tester or with explicit written permission from the authorized owner.

Unauthorized access, scanning, exploitation, modification, or disruption of systems may violate applicable laws and may result in criminal, financial, or civil penalties.

**Use this information responsibly, legally, and only within an authorized scope.**

---

# 👤 Author

**Joynul Hasan**

🎓 Cybersecurity
🏫 **B082-Networkwalks Program**

🔗 LinkedIn:
https://www.linkedin.com/in/joynul-hasan-12b3ab307/

---

## 📌 Project Information

**Program:** B082-Networkwalks
**Project:** Penetration Testing – Footprinting & Network Scanning
**Focus:** Reconnaissance, OSINT, DNS Enumeration & Network Discovery

---

⭐ **If you find this project useful for learning cybersecurity, consider giving the repository a star.**
