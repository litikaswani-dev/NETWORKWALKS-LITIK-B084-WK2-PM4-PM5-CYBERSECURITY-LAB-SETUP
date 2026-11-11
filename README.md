# NetworkWalks Cybersecurity Internship – Week 2

### Reconnaissance, Footprinting & Network Scanning

**Intern:** Litik Aswani  
**Batch:** B084  
**Date:** 11 November 2026  
**Organization:** NetworkWalks

---

## About This Repository

This repository documents the practical tasks completed during Week 2 of my Cybersecurity Internship at NetworkWalks.

The activities focused on two important phases of cybersecurity assessment:

- **Reconnaissance & Footprinting** using theHarvester
- **Network Scanning & Discovery** using Zenmap (Nmap)

The repository contains separate documentation for each module, practical screenshots, scan findings, and a final penetration testing report.

## Modules Completed

### PM4 – Footprinting Using theHarvester

**Environment:** Kali Linux (VirtualBox)  
**Tool:** theHarvester 4.11.1  
**Target:** microsoft.com

Performed passive reconnaissance using Baidu and multiple supported data sources to gather publicly available information.

**Key Findings:**

| Finding | Result |
|---|---:|
| Baidu Search Results | 0 |
| IP Addresses | 111 |
| Email Addresses | 3 |
| Host Entries | 9,488 |

Some data sources required API keys, which limited the completeness of the scan.

[View PM4 Documentation & Screenshots](PM4-theHarvester/README.md)

---

### PM5 – Network Scanning Using Zenmap

**Environment:** Windows 11  
**Tool:** Zenmap / Nmap 7.99.3  
**Scan Type:** Ping Scan

Performed host discovery on an authorized local network and generated a network topology diagram.

**Key Findings:**

| Metric | Result |
|---|---:|
| IP Addresses Scanned | 256 |
| Active Hosts Discovered | 5 |
| Scan Duration | 4.81 seconds |
| Scan Profile | Ping Scan |

The scan helped identify responsive hosts and visualize the local network structure.

[View PM5 Documentation & Screenshots](PM5-Zenmap/README.md)

---

## Tools & Technologies

| Tool | Purpose |
|---|---|
| Kali Linux | Cybersecurity testing environment |
| Oracle VirtualBox | Virtualization |
| theHarvester | Passive reconnaissance |
| Windows Command Prompt | Network configuration |
| Zenmap | Graphical network scanning |
| Nmap | Network host discovery |
| GitHub | Documentation and version control |
| Markdown | Technical reporting |

---

## Repository Structure

```text
NetworkWalks-Week2/
│
├── README.md
├── REPORT.md
│
├── PM4-theHarvester/
│   ├── README.md
│   └── screenshots/
│       ├── PM4_Task1_Baidu.png
│       ├── PM4_Task2_Command.png
│       ├── PM4_Task2_API_Warnings.png
│       ├── PM4_Task2_IPs.png
│       └── PM4_Task2_Emails_and_Hosts.png
│
└── PM5-Zenmap/
    ├── README.md
    ├── screenshots/
    │   ├── PM5_01_IP_Configuration.png
    │   ├── PM5_02_Zenmap_Configuration.png
    │   ├── PM5_03_Ping_Scan_Results.png
    │   └── PM5_04_Network_Topology.png
    │
    └── PM5_04_Network_Topology.pdf
```

---

## Final Penetration Testing Report

The complete Week 2 report includes:

- Liability disclaimer
- Introduction and objectives
- Tools and technologies
- Practical activities and commands
- Scan results and observations
- Risk analysis and potential impact
- Security recommendations
- Conclusion and evidence

### [View Full Week 2 Report](REPORT.md)

---

## Key Learnings

Through these activities, I gained practical experience in:

- Performing passive reconnaissance using publicly available sources.
- Using theHarvester for domain-based information gathering.
- Understanding API key requirements and reconnaissance limitations.
- Identifying local network configurations.
- Performing host discovery using Zenmap and Nmap.
- Interpreting network scanning results.
- Generating network topology diagrams.
- Documenting findings in a structured cybersecurity report.
- Protecting sensitive information when publishing evidence.

## Ethical & Security Disclaimer

All activities documented in this repository were performed for educational purposes as part of the NetworkWalks Cybersecurity Internship.

Reconnaissance was limited to publicly available information, and network scanning was performed on an owned or authorized local network.

No unauthorized access, exploitation, password attacks, or vulnerability exploitation was conducted.

Sensitive network identifiers should be redacted from publicly shared evidence.

The findings represent observations from the tools used and do not establish confirmed security vulnerabilities.

---

## Acknowledgment

I would like to thank **NetworkWalks** for providing this opportunity to gain practical cybersecurity experience through hands-on assignments.

These exercises helped strengthen my understanding of reconnaissance, network discovery, ethical security practices, and technical documentation.

---

**NetworkWalks Cybersecurity Internship**  
**Week 2 – Practical Project Submission**  
**Prepared by Litik Aswani | Batch B084**
