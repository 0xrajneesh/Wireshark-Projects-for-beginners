# Decrypting and Analyzing SSL/TLS Traffic

## Introduction

In this project, you'll learn how to use Wireshark to decrypt and analyze SSL/TLS traffic. Understanding SSL/TLS traffic is essential for diagnosing issues with secure communications and ensuring the security of data in transit.

## Pre-requisites

- Basic understanding of networking and encryption concepts
- Wireshark installed on your computer
- Access to SSL/TLS server private keys (for decryption purposes)
- A sample PCAP file containing SSL/TLS traffic

## Lab Set-up and Tools

1. **Wireshark**: Download and install Wireshark from [https://www.wireshark.org/download.html](https://www.wireshark.org/download.html).
2. **Sample PCAP File**: Download a sample PCAP file containing SSL/TLS traffic.
3. **Private Key File**: Obtain the private key for the SSL/TLS server used in the sample PCAP file.

## Exercises

### Exercise 1: Load a Sample PCAP File

#### Steps

1. Open Wireshark.
2. Go to "File" > "Open" and select the sample PCAP file you downloaded.
3. The file will load, and the captured traffic will be displayed.

#### Expected Output

- The sample PCAP file containing network traffic loaded in Wireshark.

### Exercise 2: Configure SSL/TLS Decryption

#### Steps

1. In Wireshark, go to "Edit" > "Preferences".
2. Expand the "Protocols" list and select "SSL" or "TLS".
3. In the "RSA keys list" section, click "Edit".
4. Add a new entry with the following details:
    - IP address: The IP address of the SSL/TLS server
    - Port: The port number used (e.g., 443 for HTTPS)
    - Protocol: `http` or `ssl`
    - Key file: Path to the private key file
5. Click "OK" to save the settings.

#### Expected Output

- Wireshark configured to use the provided private key for SSL/TLS decryption.

### Exercise 3: Filter SSL/TLS Traffic

#### Steps

1. In the filter bar at the top, enter the filter `ssl` or `tls` and press Enter.
2. Wireshark will display only the SSL/TLS traffic from the capture.

#### Expected Output

- Displayed SSL/TLS traffic filtered from the overall capture.

### Exercise 4: Decrypt and Analyze SSL/TLS Packets

#### Steps

1. Select a decrypted SSL/TLS packet from the filtered traffic.
2. Click on the packet to view its details in the packet details pane.
3. Expand the "Secure Sockets Layer" or "Transport Layer Security" section to view detailed information about the handshake, encryption parameters, and decrypted data.

#### Expected Output

- Detailed information about decrypted SSL/TLS packets displayed.

### Exercise 5: Follow SSL/TLS Streams

#### Steps

1. Right-click on a decrypted SSL/TLS packet and select "Follow" > "TCP Stream" to view the entire conversation.
2. Analyze the decrypted stream to understand the data being transmitted and identify any potential security issues.

#### Expected Output

- A complete, decrypted SSL/TLS communication stream analyzed.

## Conclusion

By completing these exercises, you have learned how to decrypt and analyze SSL/TLS traffic using Wireshark. These skills are essential for diagnosing issues with secure communications, ensuring data security, and understanding encrypted network traffic.
