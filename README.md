# Azure VPN Setup and Usage Lab

## Overview
This project demonstrates how to configure and use a VPN to change public IP address and geographic location using a cloud-based virtual machine in Microsoft Azure.

The goal was to understand how VPNs route traffic through different locations and how IP addresses change based on network origin.

## Technologies Used
- Microsoft Azure (Virtual Machines)
- Windows 10 VM
- ProtonVPN
- Remote Desktop (RDP)

## Project Steps
1. Checked public IP address from local machine.
2. Created a Windows 10 Virtual Machine in Azure (different geographic region).
3. Verified the VM’s public IP and location.
4. Installed and configured ProtonVPN inside the VM.
5. Connected to a VPN server in another country (Japan).
6. Verified IP address change and location shift using an IP lookup tool.
7. Tested website behavior based on new geographic location.

## Results
- Local machine IP showed a United States location.
- Azure VM showed a different U.S. data center location.
- VPN connection changed the IP location to Japan, confirming traffic was routed through a remote server.  [oai_citation:0‡Lab 4 Checklist_ VPN Setup and Usage (Proton VPN).pdf](sediment://file_00000000002471f58231376be4ce31a6)

## Skills Demonstrated
- Cloud VM deployment (Azure)
- Remote access using RDP
- VPN configuration and usage
- IP addressing and geolocation analysis
- Understanding network routing and tunneling

## Key Takeaways
- VPNs hide the original IP address and replace it with the VPN server’s IP.
- Network traffic can appear to originate from different geographic locations.
- Cloud environments can be used to simulate real-world networking scenarios.
