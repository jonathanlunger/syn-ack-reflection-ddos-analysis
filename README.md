# syn-ack-reflection-ddos-analysis

 SYN/ACK Reflection DDoS Analysis

This repository documents a network forensic investigation into a suspected
SYN/ACK reflection Distributed Denial of Service (DDoS) attack that caused
a public-facing server outage.

## Investigation Summary

A 30-minute packet capture was analyzed using Wireshark to determine:

- The most frequently targeted IP address
- The most prevalent TCP flags
- The attack timeline
- The number of unique source IPs involved
- Whether the traffic represented a DDoS attack or legitimate activity

## Key Findings

- Targeted IP: 10.10.10.10
- ~12,000 SYN and ACK packets delivered within ~0.2 seconds
- 7,057 unique source IP addresses
- Attack classified as SYN/ACK reflection DDoS
- Concurrent SSH PSH packets observed (possible smokescreen activity)

## Skills Demonstrated

- PCAP analysis in Wireshark
- TCP flag interpretation and protocol analysis
- Endpoint and conversation statistics analysis
- Timeline reconstruction
- Botnet pattern recognition
- DDoS attack classification
- Defensive mitigation strategy development

📄 Full Report: [View Investigation](./docs/SYN-ACK-Reflection-DDoS-Investigation.pdf)

## Tools Used

- Wireshark
- TCP display filters
- Endpoint and conversation statistics
- Traffic timeline analysis
