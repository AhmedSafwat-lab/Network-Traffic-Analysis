# Network Traffic Analysis Report

## Objective

The objective of this task is to analyze network traffic in order to identify potential security threats and understand how packets travel within a network.

## Tools Used

Wireshark
Kali Linux

## Traffic Generation

Network traffic was generated using the following command:

ping 8.8.8.8

This command sends ICMP packets from the local machine to the destination server.

## Traffic Capture

The packets were captured using Wireshark while the ping command was running.

## Observations

1. ICMP Echo Requests

These packets were sent from the local host to the destination server.

Source IP: Local machine  
Destination IP: 8.8.8.8

2. ICMP Echo Replies

These packets were received from the destination server as a response to the requests.

Source IP: 8.8.8.8  
Destination IP: Local machine

3. Response Time

Each request was followed by a reply indicating successful communication.

## Potential Security Concerns

Although ICMP is commonly used for network diagnostics, excessive ICMP traffic may indicate:

Network scanning  
ICMP flooding attacks  
Denial of Service attempts

## Recommendations

Monitor ICMP traffic regularly  
Implement firewall rules to limit excessive ICMP requests  
Use network intrusion detection systems  
Log unusual network activities

## Conclusion

Network traffic analysis is an important part of cybersecurity. By analyzing captured packets, security professionals can identify unusual patterns and take action to protect network infrastructure.
