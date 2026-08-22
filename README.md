# networkwalks-internship-B082-week2-Footprinting-Networkscanning
# Week 2 – Footprinting & Network Scanning

## Cybersecurity & Ethical Hacking Internship

**Author:** Aman Varshney
**Program/Batch:** B082 – Networkwalks
**Week:** 02
**Date:** 22 August 2026
**Modules:** W2-PM4 – The Harvester | W2-PM5 – Zenmap

---

## 📌 Project Overview

This repository contains my Week 2 practical work completed as part of my **Cybersecurity & Ethical Hacking Internship at Networkwalks**.

The project focuses on two important phases of penetration testing:

1. **Footprinting & Reconnaissance** using **theHarvester**
2. **Network Scanning & Discovery** using **Zenmap (Nmap GUI)**

These activities helped me understand how publicly available information can be gathered during reconnaissance and how live hosts can be identified within an authorized local network.

---

## 🎯 Objectives

* Understand the fundamentals of footprinting and reconnaissance.
* Gather publicly available information related to a target domain.
* Identify domain-related information using theHarvester.
* Understand different reconnaissance sources.
* Identify live hosts on a local network using Zenmap.
* Understand IP and MAC address discovery.
* Generate and analyze basic network topology.
* Document cybersecurity findings and potential risks.
* Perform all activities within an authorized scope.

---

## 🛠️ Tools & Technologies

| Tool             | Purpose                                                     |
| ---------------- | ----------------------------------------------------------- |
| **Kali Linux**   | Operating system used for reconnaissance                    |
| **theHarvester** | Collection of publicly available domain-related information |
| **Zenmap**       | GUI-based network scanning and host discovery               |
| **Nmap**         | Scanning engine used by Zenmap                              |
| **Windows CMD**  | Identifying local IP and MAC address information            |

---

## 🔎 Module 1 – Footprinting with theHarvester

### Objective

The objective of this activity was to perform authorized footprinting and reconnaissance against the `networkwalks.com` domain.

### Activities Performed

TheHarvester was executed in Kali Linux to collect publicly available information associated with the target domain.

Example commands used:

```bash
theHarvester -d networkwalks.com -l 1000 -b baidu
```

The above command was used to search for publicly available information using the specified source.

Another command used was:

```bash
theHarvester -d networkwalks.com -l 50 -b all
```

This was used to search across the available supported sources.

### Information Gathered

The reconnaissance activity focused on information such as:

* Email IDs
* Hosts
* IP-related information
* Subdomains/domain-related information
* Publicly indexed organizational information

The collected outputs were documented separately and screenshots were captured as evidence.

---

## 🌐 Module 2 – Network Scanning with Zenmap

### Objective

The objective of this activity was to perform network discovery on my **own local network** using Zenmap.

### Activities Performed

First, the Windows `ipconfig` command was used to identify the local IP address and LAN subnet.

```cmd
ipconfig
```

The identified subnet was then entered into Zenmap.

A **Ping Scan** was performed to identify active hosts on the local network.

### Scan Results

The practical scan identified:

* **One live host**
* The live host corresponded to my own device.
* A MAC address was also identified during the activity.

The Zenmap **Topology** feature was then used to visualize the network environment, and the resulting topology was saved in PDF format.

---

## 📊 Risk Analysis

The activities resulted in the following observations:

| Finding                                       | Potential Impact                                     | Risk Level |
| --------------------------------------------- | ---------------------------------------------------- | ---------- |
| Publicly available organizational information | May assist attackers during initial reconnaissance   | Medium     |
| Domain-related information identifiable       | Can contribute to further reconnaissance             | Low        |
| Search-engine reconnaissance possible         | Publicly indexed information may support enumeration | Low        |
| Multi-source reconnaissance possible          | Information from multiple sources can be correlated  | Medium     |
| One live host identified on local network     | Confirms the presence of the tested host             | Low        |

> **Note:** These are observations from reconnaissance and scanning activities and are **not confirmed vulnerabilities**. No exploitation or vulnerability validation was performed.

---

## 🔐 Security Recommendations

Based on the observations, the following security practices are recommended:

### 1. Minimize Public Information Exposure

Regularly review publicly available organizational information and remove unnecessary sensitive details.

### 2. Monitor the External Attack Surface

Conduct periodic authorized assessments to identify newly exposed domains, services and organizational information.

### 3. Review DNS and Web Configuration

Regularly review DNS records, HTTP responses and web configurations to reduce unnecessary technical information disclosure.

### 4. Perform Regular Network Scanning

Authorized network scans should be performed periodically to identify unexpected or unauthorized hosts and services.

### 5. Keep Systems Updated

Operating systems, web applications, plugins and other software should be regularly updated and patched.

---

## 📁 Repository Structure

```text
Week-2-Footprinting-Network-Scanning/
│
├── README.md
│
├── Report/
│   └── W2-PM-FINAL-Sample-Report-v2.pdf
│
├── TheHarvester/
│   └── outputs/
│
├── Zenmap/
│   ├── scan-results/
│   └── topology/
│
└── Evidence/
    └── screenshots/
```

---

## 📸 Evidence

Screenshots and supporting evidence from the practical activities are included in the repository where applicable.

Evidence includes:

* theHarvester execution
* theHarvester output
* Windows `ipconfig` output
* Zenmap scan results
* Zenmap topology
* Other relevant practical screenshots

---

## ⚠️ Legal & Ethical Disclaimer

All activities documented in this repository were performed only on systems and devices for which I had authorization or on systems/devices owned by me.

This project is intended **strictly for educational and research purposes**.

Do not use these techniques against systems without proper authorization. Unauthorized reconnaissance, scanning or access may violate organizational policies and applicable laws.

The author and Networkwalks are not responsible for misuse of the information contained in this repository.

**Always obtain proper authorization before performing security testing.**

---

## 📚 Learning Outcomes

Through this Week 2 practical work, I gained hands-on experience in:

* Footprinting and reconnaissance
* Public information gathering
* Domain reconnaissance using theHarvester
* Understanding search-source based enumeration
* Network discovery using Zenmap
* Identifying live hosts
* Understanding IP and MAC addresses
* Basic network topology visualization
* Risk identification and documentation
* Authorized cybersecurity testing

---

## 📝 Conclusion

This Week 2 project provided practical exposure to the **reconnaissance and network scanning phases of penetration testing**.

Using **theHarvester**, I learned how publicly available information related to a domain can be gathered from different sources. Using **Zenmap**, I learned how to perform network discovery and identify active hosts within my own authorized local network.

Overall, these exercises strengthened my understanding of how reconnaissance and scanning contribute to cybersecurity assessments and reinforced the importance of performing security testing within an authorized scope.

---

## 👤 Author

**Aman Varshney**
Cybersecurity Student – B082
Networkwalks Cybersecurity Program

---

⭐ **If you find this project useful, consider giving the repository a star!**
