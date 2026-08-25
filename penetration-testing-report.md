# Penetration Testing Report

## Footprinting & Network Scanning Phases

**Cybersecurity | Networkwalks**

### Tester Information

- **Penetration Tester:** Joynul Hasan
- **Program:** B082-Networkwalks
- **Target:** Networkwalks + My Own LAN
- **Permission:** Yes
- **Phases:** Reconnaissance & Footprinting; Scanning & Network Discovery
- **Modules:** Multiple Kali Tools; Zenmap Scanning; Maltego Domain Reconnaissance

## 1. Liability & Legal Disclaimer

This penetration testing report is intended strictly for authorized security testing, educational, and research purposes. All activities described in this report were conducted only on systems owned by the tester or with explicit written permission from the authorized owner.

The tools, techniques, findings, and proof-of-concept demonstrations included in this report are provided solely to identify security weaknesses and improve defensive security practices. Nothing in this report grants permission to access, scan, exploit, modify, or disrupt any system without authorization.

The tester, instructor, authors, and associated organizations assume no responsibility for misuse of the information contained in this report. Unauthorized access or exploitation may violate applicable laws and can result in criminal, financial, or civil penalties.

## 2. Introduction

This report covers two key phases of network security assessment: footprinting and network scanning. The first module focuses on footprinting the networkwalks.com domain using multiple Kali Linux tools, while the second module covers scanning my own local network using Zenmap.

Together, these activities demonstrate how an attacker can move from gathering publicly available information about a target to identifying live hosts, open ports, and potential services within a network.

## 3. Tools Used

| Tool | Purpose |
|---|---|
| Kali Linux & Windows | Operating systems used for reconnaissance activities |
| WHOIS | Find domain registration details |
| WhatWeb | Fingerprint web technologies |
| nslookup | Resolve domain name to IP address |
| curl -I | Read HTTP response headers |
| Wafw00f | Detect Web Application Firewall |
| DNSRecon | Enumerate DNS records |
| Zenmap | Discover live hosts, IPs and MAC addresses |
| Windows CMD | Identify local IP and MAC address |
| Maltego | Email/domain relationship analysis |

## 4. Activities Performed

### 4.1 Footprinting & Reconnaissance

Reconnaissance was performed using WHOIS, WhatWeb, Nslookup, Curl, Wafw00f and DNSRecon. Each tool was used to collect a different type of publicly available information.

The assessment identified domain registration information, web technologies, DNS/IP information, HTTP response headers, WAF information and DNS records.

### 4.2 Network Scanning with Zenmap

Zenmap was used to perform network discovery on my local network. The local IP address and subnet were identified using Windows `ipconfig`, followed by a Ping Scan in Zenmap to identify active hosts.

The Topology section was then used to visualize the discovered network.

### 4.3 Maltego

Maltego was used during the reconnaissance phase for email footprinting and to identify publicly available information associated with the target domain/email infrastructure. The information was represented through a visual relationship graph.

## 5. Risk Analysis

The identified observations included exposed web technology information, identifiable server IP information, HTTP technical information, identifiable WAF technology, DNS infrastructure information and multiple live hosts on the local network.

These are observations from information gathering and host discovery, not confirmed vulnerabilities. Further authorized security testing would be required to validate vulnerabilities.

## 6. Recommendations

- Review publicly exposed technology information.
- Keep software and plugins updated.
- Review HTTP response headers.
- Review DNS records regularly.
- Properly configure and monitor the WAF.
- Perform regular internal network discovery.
- Investigate unknown devices.
- Maintain network documentation.
- Perform security testing only with authorization.

## 7. Conclusion

The exercises demonstrated the importance of reconnaissance and network discovery in cybersecurity. Multiple Kali Linux tools were used to collect domain and infrastructure information, while Zenmap was used to discover active hosts on a local network.

The project also demonstrated the importance of documenting security observations, explaining their potential impact, and recommending appropriate defensive improvements.

## 8. Evidence

Screenshots and supporting evidence can be placed in the `evidence/` directory.

Recommended evidence:

1. WHOIS
2. WhatWeb
3. Nslookup
4. Curl -I
5. DNSRecon
6. Wafw00f
7. Zenmap Ping Scan
8. Zenmap Topology
9. Maltego domain/email footprinting
