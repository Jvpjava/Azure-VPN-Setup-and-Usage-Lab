# Azure VPN & IP Behavior Analysis Lab

<p align="center">
  <img src="img/vpnproton.jpg" alt="Azure VPN Lab Cover" width="900">
</p>

## Overview
This project demonstrates how VPNs affect public IP addresses, geolocation, and web browsing behavior using Microsoft Azure and ProtonVPN.

The goal was to simulate real-world scenarios where users access the internet from different geographic regions and analyze how websites respond to those changes.

---

## Objectives
- Identify and record public IP addresses before and after VPN usage  
- Deploy a cloud-based virtual machine in a different geographic region  
- Route traffic through a VPN server in another country  
- Analyze how websites behave based on location changes  

---

## Technologies Used
- Microsoft Azure  
- Windows 10 Virtual Machine  
- ProtonVPN (Free Tier)  
- Remote Desktop Protocol (RDP)  
- Web tools: whatismyipaddress.com  

---

## Lab Breakdown

### 1. Baseline IP Check
- Checked my local machine's public IP address using:
  - https://whatismyipaddress.com  
- Recorded IP and location details  

📎 Reference: Initial IP verification step :contentReference[oaicite:0]{index=0}  

<p align="center">
  <img src="img/2. LocalHost IP Address.png"  width="900">
</p>


---

### 2. Azure Environment Setup
- Created a **Resource Group**
- Deployed a **Windows 10 Virtual Machine** in a different region  

📎 Example: VM deployed outside my original location (different country) :contentReference[oaicite:1]{index=1}  

---

### 3. Remote Access
- Connected to the VM using **Remote Desktop (RDP)**
- Verified new public IP from within the VM  

---

### 4. VPN Configuration
- Installed **ProtonVPN** inside the VM  
- Connected to a VPN server in another country (e.g., Japan)  

📎 VPN connection step :contentReference[oaicite:2]{index=2}  

---

### 5. IP Address Comparison
| Stage | IP Address Location |
|------|--------------------|
| Local Machine | Original location (USA) |
| Azure VM | Different region (e.g., Korea) |
| VPN Enabled | Third region (e.g., Japan) |

---

### 6. Web Behavior Analysis
Tested websites like:
- Google  
- Disney  
- TikTok  

Observed:
- Language changes  
- Region-specific content  
- Different URLs and layouts  

📎 Example behavior change instructions :contentReference[oaicite:3]{index=3}  

---

### 7. Cleanup
- Deleted Azure Resource Group to avoid unnecessary costs  

📎 Cleanup step :contentReference[oaicite:4]{index=4}  

---

## Key Takeaways
- VPNs mask your real IP and replace it with the server’s IP  
- Web services use IP-based geolocation to customize content  
- Cloud environments allow testing from multiple regions without physical travel  
- Network behavior can change significantly based on geographic origin  

---

## Project Value
This lab demonstrates practical understanding of:
- Network security concepts  
- VPN functionality  
- Cloud-based infrastructure  
- Real-world troubleshooting and analysis  

---

## Future Improvements
- Automate IP logging with PowerShell  
- Capture packet data using Wireshark  
- Compare latency across regions  
- Integrate firewall rules and monitoring  


---

## 👨‍💻 Author
Giovanny Perdomo  
Aspiring IT Professional | Networking | Security | Cloud Labs
