# **Week 04 — Networks & Network Security**

**Date Range:** Nov 17 – Nov 23, 2025
**Total Hours:** ~8–9 hrs
**Phase:** Google Cybersecurity Certificate (Course 3: Networks & Network Security)

---

## **Topics Covered**

### **Module 1: Introduction to Networks**

**Key Concepts:**

* Definition of networks and how devices communicate
* LAN vs WAN vs PAN
* How data travels across network media
* OSI Model (7 layers) and why abstraction helps security
* TCP/IP Model (4 layers) and how it maps to OSI
* Packet structure (headers, payload, protocols)

**Important Terms:**

* Router: Directs traffic between networks
* Switch: Connects devices within a network
* IP Address: Logical addressing
* MAC Address: Physical addressing

---

### **Module 2: TCP/IP, Routing, and Switching**

**Key Concepts:**

* IPv4 vs IPv6
* Subnetting basics
* NAT and PAT
* DHCP for automated addressing
* ARP for mapping MAC ↔ IP
* Routing tables & default gateway
* How switching creates isolated collision domains

**Important Terms:**

* TCP vs UDP
* Ports (HTTPS: 443, SSH: 22, DNS: 53)
* MTU (Maximum Transmission Unit)

---

### **Module 3: Network Security Controls**

**Key Concepts:**

* Firewalls (packet-filtering, stateful, proxy, NGFW)
* IDS vs IPS and how they detect/block threats
* VPNs and encrypted network tunnels
* ACLs for traffic filtering
* Zero Trust model basics
* Network hardening techniques

**Important Terms:**

* Signature-based detection
* Anomaly-based detection
* Honeypots / honeynets
* TLS, SSL, IPsec

---

### **Module 4: WiFi Security & Monitoring**

**Key Concepts:**

* WPA2 vs WPA3
* Wireless vulnerabilities (Evil Twin, Deauth, MITM)
* Network logs (firewall logs, DHCP logs, access logs)
* Logging best practices for incident response
* WIDS/WIPS (Wireless IDS/IPS)
* Network monitoring dashboards and baselines

**Screenshots:**

* `2025-12-3_Course3_Completion.png`

---

## **Key Takeaways**

1. Networks are built from predictable layers (OSI & TCP/IP), which helps security teams pinpoint vulnerabilities.
2. Firewalls + IDS/IPS are foundational defense tools for controlling and observing traffic.
3. WiFi security is often a weak point — modern orgs must use WPA3 and monitoring systems.
4. Logs and baselines are crucial for detecting anomalies (DDoS, MITM, port scans).
5. Secure configurations (ACLs, NAT, segmentation) drastically reduce attack surfaces.
6. Network security = visibility + control + segmentation + encryption.

---

## **Questions/Confusion**

* How deep does Coursera expect us to go with segmentation? (Basic VLAN vs full micro-segmentation)
* IDS placement: Is it better at the perimeter or inside the LAN?
* IPS false positives—how do companies reduce accidental block events?

---

## **Next Week Goals**

* [ ] Start Course 4: Assets, Threats, & Vulnerabilities
* [ ] Begin CVE #1 (SQL Injection on DVWA) under VulnForge
* [ ] Add another SecureScholar polish (UI or small feature)
* [ ] Expand new_case.py with an optional metadata field (e.g., attack_type)

---

## **Weekly Reflection (Sat 11/22)**

This week I completed **Course 3: Networks and Network Security**, which covered routing, switching, firewalls, IDS/IPS, WiFi security, and network hardening. I built a real feature for SecureScholar by adding full scoring and feedback to the Module 2 quiz. I also launched **VulnForge from scratch**, created the full repo, and built my first automation tool (`new_case.py`) that generates CVE folders and notes automatically. These two real coding deliverables (front-end JS logic + back-end Python automation) show that I’m starting to combine cybersecurity theory with practical coding. This sets me up perfectly for Course 4 and my first real CVE reproduction next week.
