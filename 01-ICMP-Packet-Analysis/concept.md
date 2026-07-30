# ICMP Packet Analysis

## Objective

The objective of this lab is to understand how Internet Control Message Protocol (ICMP) packets are exchanged between two hosts during a Ping operation using Wireshark.



# What is ICMP?

Internet Control Message Protocol (ICMP) is a Layer 3 protocol used for network diagnostics, error reporting, and connectivity testing.

Unlike TCP and UDP, ICMP does not transport application data. Instead, it communicates information about the status of IP communications.

One of its most common uses is the **Ping** command.



# Common Uses

- Testing network connectivity
- Measuring response time
- Reporting unreachable destinations
- Time Exceeded messages (Traceroute)
- Network troubleshooting



# ICMP Echo Process

When a user runs:

```
ping google.com
```

The following process occurs:

1. The destination IP address is resolved (DNS).
2. The source sends an **ICMP Echo Request (Type 8)**.
3. The destination replies with an **ICMP Echo Reply (Type 0)**.
4. The process repeats until all packets are exchanged.



# Important ICMP Fields

- Source IP Address
- Destination IP Address
- Type
- Code
- Checksum
- Identifier
- Sequence Number
- Time To Live (TTL)



# Key Observations

- ICMP works directly over IP.
- No TCP or UDP ports are used.
- Every Echo Request should receive a corresponding Echo Reply.
- If ARP information is already cached, ARP packets will not appear before the Ping.



# Tools Used

- Wireshark
- Windows 10
- Command Prompt



# Learning Outcome

After completing this lab, I understood how ICMP packets travel across the network and how Wireshark can be used to inspect packet-level communication for troubleshooting and network analysis.
