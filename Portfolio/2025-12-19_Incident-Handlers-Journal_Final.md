
# Incident Handler’s Journal

**Course:** Google Cybersecurity Certificate
**Purpose:** Documentation of incident response investigations and tool usage

---

## **Entry 1**

### **Date**

December 19, 2025

### **Entry**

1

### **Description**

This entry documents a ransomware incident that disrupted a small U.S. healthcare clinic. The investigation focused on identifying the cause, impact, and timeline of the incident. This activity aligns primarily with the **Detection and Analysis** phase of the NIST Incident Response Lifecycle.

### **Tool(s) Used**

No direct cybersecurity tools were used during this phase. Information was gathered through employee reports, system behavior observations, and the displayed ransom note.

### **The 5 W’s**

* **Who:** An organized ransomware group targeting healthcare organizations caused the incident.
* **What:** Ransomware encrypted critical systems and displayed a ransom note demanding payment.
* **When:** Tuesday morning at approximately 9:00 a.m.
* **Where:** The internal network of a small U.S.-based healthcare clinic.
* **Why:** Employees opened phishing emails containing malicious attachments, allowing malware execution.

### **Reflections / Notes**

This incident highlights how phishing remains a primary attack vector in healthcare environments. Improved email filtering and security awareness training could have reduced risk. Backup strategy maturity would be critical for recovery. Understanding attacker motivation and entry points is essential for long-term mitigation.

---

## **Entry 2**

### **Date**

December 19, 2025

### **Entry**

2

### **Description**

This entry documents the analysis of a suspicious network packet to identify potential malicious activity. The task focused on recognizing abnormal traffic patterns and aligns with the **Detection and Analysis** phase of the NIST Incident Response Lifecycle.

### **Tool(s) Used**

* Packet capture tools were used to inspect network traffic.
* Packet headers and payload data were examined for anomalies.
* IP addresses and protocols were reviewed to identify suspicious behavior.
* Traffic patterns were compared against expected baseline activity.

### **The 5 W’s**

Not applicable. This entry focuses on technical analysis using a cybersecurity tool rather than a full incident investigation.

### **Reflections / Notes**

Packet analysis improves visibility into network behavior and supports early threat detection. Learning to interpret packet data helps identify unauthorized access attempts. This skill is critical for SOC analysts when responding to alerts. Understanding normal traffic baselines is essential.

---

## **Entry 3**

### **Date**

December 19, 2025

### **Entry**

3

### **Description**

This entry documents the investigation of a suspicious file hash to determine whether it was associated with known malware. The activity supports the **Detection and Analysis** phase of the NIST Incident Response Lifecycle.

### **Tool(s) Used**

* A file hash lookup tool was used to analyze the suspicious hash.
* Threat intelligence databases were queried for known malware signatures.
* Results were compared against trusted sources to confirm malicious status.
* Findings were used to assess potential system risk.

### **The 5 W’s**

* **Who:** A potentially malicious actor distributed the file.
* **What:** A suspicious file was identified and analyzed via its hash.
* **When:** During routine investigation following a security alert.
* **Where:** On an endpoint within the organization’s environment.
* **Why:** The hash matched known malicious indicators, suggesting compromise.

### **Reflections / Notes**

File hash analysis is an efficient method for validating malware presence. Threat intelligence integration strengthens detection accuracy. This activity emphasized the importance of trusted databases. Hashing supports rapid triage during investigations.

---

## **Entry 4**

### **Date**

December 220, 2025

### **Entry**

4

### **Description**

This entry documents the use of a SIEM tool to perform log analysis and investigate suspicious activity. The task focused on querying logs to identify patterns and supports the **Detection and Analysis** phase of the NIST Incident Response Lifecycle.

### **Tool(s) Used**

* A SIEM platform was used to query security logs.
* Filters were applied to isolate relevant events.
* Timestamp correlations helped reconstruct activity timelines.
* Results supported incident validation and scope determination.

### **The 5 W’s**

Not applicable. This entry emphasizes tool usage rather than a standalone incident narrative.

### **Reflections / Notes**

SIEM tools centralize log analysis and improve investigation efficiency. Querying logs enables rapid identification of anomalies. Correlating events across systems provides critical context. This activity reinforced the importance of log retention and structured querying skills.

