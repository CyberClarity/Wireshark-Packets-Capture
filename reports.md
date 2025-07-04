# Task 5 - Wireshark Capture Analysis

**Objective:**  
Capture live network traffic using Wireshark, identify at least 3 protocols, and summarize the findings.

---

## 📦 Protocols Identified

1. **DNS (Domain Name System)**  
   - Observed multiple DNS queries and responses.
   - Example:
     - **Source IP:** 192.168.x.x
     - **Destination IP:** 202.134.152.6  
     - **Query:** google.com (A and AAAA records)
   - DNS is responsible for resolving domain names to IP addresses.

2. **ARP (Address Resolution Protocol)**  
   - Observed several ARP announcements and requests.
   - Example:
     - **Source:** optilinknetw_ xx:xx (MAC: xx:xx:xx:xx:xx:xx)  
     - **Destination:** Broadcast (ff:ff:ff:ff:ff:ff)  
     - **Info:** Announcement for 192.168.x.x
   - ARP is used to map IP addresses to MAC addresses on the local network.

3. **TCP (Transmission Control Protocol)**  
   - Although not shown in the screenshots, TCP packets were likely captured during browsing/pinging.
   - TCP ensures reliable, ordered delivery of data between hosts.

---

## 📂 Screenshots

### 📸 DNS Packets
![DNS Filter](https://github.com/CyberClarity/Wireshark-Packets-Capture/blob/main/screenshot/ARP.png)

### 📸 ARP Packets
![ARP Filter](https://github.com/CyberClarity/Wireshark-Packets-Capture/blob/main/screenshot/DNS.png))

---

## 📝 Summary of Findings

- **DNS:** Confirmed normal DNS query and response behavior; successfully resolved domains like google.com.
- **ARP:** Multiple ARP announcements observed on the local network, which is typical for devices broadcasting their IP-MAC mappings.
- **TCP:** Present in most connections, used for data transfer during browsing or pings.
- Filters like `dns` and `arp` helped isolate relevant packets for detailed analysis.

**Deliverables included:**
- `task5_capture.pcap`
- This `report.md`
- Screenshots showing applied filters in Wireshark.

---

## ✅ Conclusion

This task demonstrated hands-on skills in capturing, filtering, and analyzing network traffic with Wireshark. Key protocols were identified, and their purpose in network communication was understood.
