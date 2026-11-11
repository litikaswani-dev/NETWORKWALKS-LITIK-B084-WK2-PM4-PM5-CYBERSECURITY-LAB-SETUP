# W2-PM4: Footprinting Using theHarvester

## NetworkWalks Cybersecurity Internship – Week 2

**Intern:** Litik Aswani  
**Batch:** B084  
**Date:** 11 November 2026  
**Operating System:** Kali Linux  
**Tool:** theHarvester 4.11.1

---

## 1. Objective

The objective was to perform passive reconnaissance using theHarvester and identify publicly available information associated with a target domain.

The activity focused on discovering:

- IP addresses
- Email addresses
- Hostnames
- Publicly indexed information

## 2. Tools Used

- Kali Linux
- theHarvester 4.11.1
- Oracle VirtualBox
- Kali Linux Terminal

## 3. Target Information

**Target Domain:** `microsoft.com`

The exercise involved public-source reconnaissance only. No direct exploitation or vulnerability testing was performed.

## 4. Task 1: Footprinting Using Baidu

### Command

```bash
theHarvester -d microsoft.com -l 1000 -b baidu
```

### Parameters

| Parameter | Description |
|---|---|
| `-d microsoft.com` | Specifies the target domain |
| `-l 1000` | Sets the result limit |
| `-b baidu` | Selects Baidu as the source |

### Results

| Information | Count |
|---|---:|
| IP addresses | 0 |
| Email addresses | 0 |
| People | 0 |
| Hosts | 0 |

The Baidu scan returned no matching results.

### Screenshot – Baidu Scan

![Baidu Scan Results](screenshots/PM4_Task1_Baidu.png)

## 5. Task 2: Footprinting Using All Sources

### Command

```bash
theHarvester -d microsoft.com -l 50 -b all
```

### Parameters

| Parameter | Description |
|---|---|
| `-d microsoft.com` | Specifies the target domain |
| `-l 50` | Sets the result limit |
| `-b all` | Uses the supported data sources |

### Screenshot – Command Execution

![All Sources Command](screenshots/PM4_Task2_Command.png)

### Results

| Information | Count |
|---|---:|
| IP addresses | 111 |
| Email addresses | 3 |
| Host entries | 9,488 |
| People | 0 |

The scan returned publicly indexed information from multiple available sources.

The counts represent tool-reported results and were not independently verified.

### Screenshot – IP Addresses

![Discovered IP Addresses](screenshots/PM4_Task2_IPs.png)

### Screenshot – Emails and Hosts

![Email and Host Results](screenshots/PM4_Task2_Emails_and_Hosts.png)

## 6. API Key Limitations

Some data sources returned missing API key warnings.

These services require authentication or an API key to retrieve information.

The scan continued using other available sources.

### Screenshot – API Warnings

![API Key Warnings](screenshots/PM4_Task2_API_Warnings.png)

## 7. Observations

1. Different data sources can produce different reconnaissance results.
2. Baidu did not return matching information in this exercise.
3. The all-sources search returned substantially more information.
4. Some reconnaissance services require API keys.
5. Publicly indexed information may reveal details about an organization's online infrastructure.
6. Discovered hosts and IP addresses are not necessarily active or vulnerable.

## 8. Conclusion

This module helped me understand how passive reconnaissance works and how theHarvester gathers publicly available information.

I gained experience executing reconnaissance commands, interpreting results, understanding source limitations, and documenting findings.

---

**Module:** W2-PM4  
**Status:** Completed

[Back to Main Repository](../README.md)
