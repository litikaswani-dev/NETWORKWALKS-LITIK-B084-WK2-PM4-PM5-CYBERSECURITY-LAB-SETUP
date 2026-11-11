# W2-PM5: Network Scanning Using Zenmap

## NetworkWalks Cybersecurity Internship – Week 2

**Intern:** Litik Aswani  
**Batch:** B084  
**Date:** 11 November 2026  
**Operating System:** Windows 11  
**Tool:** Zenmap / Nmap 7.99.3

---

## 1. Objective

The objective was to discover active devices on an authorized local network using Zenmap.

The exercise involved:

- Identifying the local network configuration
- Performing host discovery
- Reviewing scan results
- Generating a network topology visualization

## 2. Tools Used

- Windows 11
- Command Prompt
- Zenmap
- Nmap 7.99.3

## 3. Identifying the Local Network

The following command was executed:

```cmd
ipconfig
```

This displayed the IPv4 address, subnet mask, and default gateway.

### Network Configuration

| Parameter | Value |
|---|---|
| Network | 192.168.0.0/24 |
| Subnet Mask | 255.255.255.0 |
| Network Type | Private LAN |

### Screenshot – IP Configuration

![IP Configuration](screenshots/PM5_01_IP_Configuration.png)

## 4. Configuring Zenmap

Zenmap was configured with the following settings:

**Target:** `192.168.0.0/24`  
**Profile:** Ping scan

### Command

```bash
nmap -sn 192.168.0.0/24
```

The `-sn` option performs host discovery without a port scan.

### Screenshot – Zenmap Configuration

![Zenmap Configuration](screenshots/PM5_02_Zenmap_Configuration.png)

## 5. Performing the Network Scan

The ping scan was executed against the local network.

### Scan Results

| Metric | Result |
|---|---|
| IP addresses scanned | 256 |
| Active hosts | 5 |
| Scan duration | 4.81 seconds |
| Scan type | Ping scan |
| Nmap version | 7.99.3 |

Five hosts were reported as active during the scan.

### Screenshot – Ping Scan Results

![Ping Scan Results](screenshots/PM5_03_Ping_Scan_Results.png)

## 6. Network Topology

After completing the scan, the Topology tab in Zenmap was used to visualize discovered devices.

The resulting diagram represented the discovered hosts in relation to the scanning machine.

### Screenshot – Network Topology

![Network Topology](screenshots/PM5_04_Network_Topology.png)

### Exported Topology

[View Network Topology PDF](PM5_04_Network_Topology.pdf)

## 7. Observations

1. Zenmap provides a graphical interface for Nmap.
2. The ping scan identified five responsive hosts.
3. Host-discovery results represent the network state at the time of scanning.
4. The Topology tab helped visualize the discovered devices.
5. Host discovery alone does not confirm security vulnerabilities.

## 8. Security Considerations

- The scan was restricted to an owned or authorized local network.
- No exploitation or credential attacks were performed.
- Private network identifiers should be redacted before public sharing.
- Further testing requires appropriate permission.

## 9. Conclusion

This module provided practical experience using Zenmap for network discovery.

I learned how to identify local network settings, configure a ping scan, interpret results, and visualize network topology.

These skills are useful during the initial discovery stages of cybersecurity assessments.

---

**Module:** W2-PM5  
**Status:** Completed

[Back to Main Repository](../README.md)
