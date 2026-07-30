# Screenshot Explanation

## Capture Overview

This screenshot shows the ICMP packets captured after executing the Ping command.

Four Echo Requests and four Echo Replies can be observed. 

It can be observer that TTL on request packets is 128 and on reply its 117 . Using this information , we can determine that there were total of 11 hops between source and destination network . 



## Packet Details

This screenshot expands one ICMP packet.

Important fields:

- Source IP = 192.168.1.37(private)
- Destination IP = 142.250.182.238(public google)
- ICMP Type = 8 request
- Code = 0
- Identifier = 1
- Sequence Number = 5 
- TTL = 128



## Packet Bytes

This section displays the raw hexadecimal representation of the captured packet.

Wireshark interprets these bytes and organizes them into Ethernet, IP, and ICMP headers.

This is the actual data transmitted over the network. 
