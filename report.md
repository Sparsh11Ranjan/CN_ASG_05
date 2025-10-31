Network Traffic Capture and Protocol Analysis using Wireshark:

Objective:

    The objective of this experiment is to capture and analyze live network traffic using Wireshark, identify various network protocols such as ICMP, DNS, and HTTP, and interpret important packet-level details like headers, fields, and communication patterns.

Tools Used:

    Wireshark (for packet capture and analysis)

    Windows Command Prompt / Terminal (for ping and browsing activities)

    (Optional) tshark (for command-line extraction of HTTP requests)

Procedure:

1. Opened Wireshark and selected the active Wi-Fi interface.

    Started packet capture and simultaneously:

    Visited a few websites (e.g., example.com, wikipedia.org).

2. Executed the command ping 8.8.8.8.

3. Stopped capture after about 2 minutes and saved the file as capture_lab1.pcap.

4. Applied protocol filters:

    icmp → to view ping request and reply packets.

    http → to observe HTTP GET and response packets.

    dns → to view DNS query and response traffic.

5. Selected one packet each from ICMP, HTTP, and DNS and noted details like Source IP, Destination IP, TTL, Packet Length, and Flags in a table (screenshots included).

6. Created a custom display filter to show only packets originating from my system using ports 80 or 443

7. Exported filtered packets as filtered_packets.pcap.

Key Insights:

    ICMP (Internet Control Message Protocol) is used for diagnostics such as the ping command. It helps check reachability between devices.

    DNS (Domain Name System) translates human-readable domain names (like wikipedia.org) into IP addresses.

    HTTP (Hypertext Transfer Protocol) is used for web communication between browsers and servers.

    Most captured packets belonged to HTTP and DNS, indicating active web browsing during capture.

    No suspicious or abnormal traffic was observed.

    The packet analysis helped understand how multiple network layers (Frame, Ethernet, IP, and Transport) interact in real-time communication.

Conclusion:

    This experiment provided practical exposure to packet capture and analysis using Wireshark.
    By applying filters, examining headers, and creating custom display filters, it became clear how different protocols operate and communicate within a network.
    Overall, the activity enhanced understanding of real-time data transmission and network behavior at the packet level.