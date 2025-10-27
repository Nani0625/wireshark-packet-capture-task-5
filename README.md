# Wireshark Packet Capture Analysis

## Task Overview
This project demonstrates basic packet capture, protocol analysis, and network troubleshooting using Wireshark. The goal is to capture live network traffic, identify protocols, and summarize key findings as per the internship task guidelines.

## Steps Performed

1. **Wireshark Installation**
    - Installed via:  
      ```
      sudo apt update
      sudo apt install wireshark
      ```
2. **Packet Capture**
    - Started Wireshark and selected the active network interface (typically `wlan0` or `eth0`).
    - Began packet capturing and generated network traffic by browsing websites and running `ping` commands.
3. **Capture Filtering**
    - Used protocol filters:
      - HTTP: `http`
      - DNS: `dns`
      - TCP: `tcp`
    - Identified at least three protocols within the traffic.
4. **Export**
    - Saved the capture as `network_capture.pcap`.
5. **Analysis & Reporting**
    - Summarized protocols and notable packet details.
    - Answered key interview questions (see below).

## Protocols Identified
- **TCP**: Reliable connection protocol used in web browsing and connections.
- **DNS**: Resolves domain names to IP addresses.
- **ICMP**: Used for ping and network diagnostics.

## Notable Packet Details

| No. | Protocol | Source IP         | Destination IP    | Info                          |
|-----|----------|-------------------|-------------------|-------------------------------|
| 1   | TCP      | 192.168.1.X       | 8.8.8.8           | SYN packet (connection start) |
| 2   | DNS      | 192.168.1.X       | 8.8.8.8           | Query: google.com             |
| 3   | ICMP     | 192.168.1.X       | 142.250.185.46    | Echo request (ping)           |

## Screenshots
All relevant screenshots are in the `screenshots/` directory, showing:
- The Wireshark home screen
- Active packet capture
- Applied filters
- Export operation

