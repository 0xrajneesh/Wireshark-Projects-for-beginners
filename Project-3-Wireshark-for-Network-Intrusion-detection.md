# Wireshark for Network Intrusion Detection

## Introduction

In this project, you'll learn how to use Wireshark for network intrusion detection. Identifying and analyzing suspicious network activities is crucial for maintaining network security and responding to potential threats.

## Pre-requisites

- Basic understanding of networking concepts
- Wireshark installed on your computer
- A sample PCAP file containing network intrusions (e.g., from [Contagio Dump](http://contagiodump.blogspot.com/))

## Lab Set-up and Tools

1. **Wireshark**: Download and install Wireshark from [https://www.wireshark.org/download.html](https://www.wireshark.org/download.html).
2. **Sample PCAP File**: Download a sample PCAP file containing network intrusion data for analysis.

## Exercises

### Exercise 1: Load a Sample PCAP File

#### Steps

1. Open Wireshark.
2. Go to "File" > "Open" and select the sample PCAP file you downloaded.
3. The file will load, and the captured traffic will be displayed.

#### Expected Output

- The sample PCAP file containing network traffic loaded in Wireshark.

### Exercise 2: Identify Indicators of Compromise (IOCs)

#### Steps

1. Look for common indicators of compromise, such as:
    - Unusual IP addresses
    - Known malicious ports
    - Suspicious protocols (e.g., IRC, SMB)
2. Use filters to isolate suspicious traffic. Examples include:
    - `ip.addr == x.x.x.x` (replace `x.x.x.x` with a known malicious IP address)
    - `tcp.port == 23` (to filter Telnet traffic)
    - `dns.qry.name contains "malicious.com"` (to identify DNS requests to suspicious domains)

#### Expected Output

- Suspicious traffic and potential indicators of compromise identified.

### Exercise 3: Analyze Suspicious Packets

#### Steps

1. Select a packet that appears suspicious based on the identified IOCs.
2. Click on the packet to view its details in the packet details pane.
3. Expand the relevant protocol sections to examine the packet details, such as headers, payload data, and any anomalies.

#### Expected Output

- Detailed information about a suspicious packet analyzed.

### Exercise 4: Follow the Intrusion's Communication Stream

#### Steps

1. Right-click on a suspicious packet and select "Follow" > "TCP Stream" or "UDP Stream" to view the entire conversation.
2. Analyze the conversation for indicators of an intrusion, such as unusual commands, unexpected data transfers, or encoded communications.

#### Expected Output

- A complete communication stream of the intrusion analyzed.

### Exercise 5: Document and Report Findings

#### Steps

1. Take notes on the suspicious activities and patterns you identified in the traffic.
2. Document key findings, including IP addresses, ports, payload data, and any other relevant details.
3. Summarize your findings in a report format, which can be used for further investigation or as part of a security incident report.

#### Expected Output

- A detailed report documenting the findings from your network intrusion analysis.

## Conclusion

By completing these exercises, you have learned how to detect and analyze network intrusions using Wireshark. These skills are essential for maintaining network security, identifying potential threats, and responding to security incidents.
