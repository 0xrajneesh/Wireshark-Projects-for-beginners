# Capturing and Analyzing VoIP Traffic

## Introduction

In this project, you'll learn how to use Wireshark to capture and analyze VoIP (Voice over IP) traffic. VoIP analysis is essential for diagnosing issues with voice communications, ensuring call quality, and identifying potential security vulnerabilities.

## Pre-requisites

- Basic understanding of networking and VoIP concepts
- Wireshark installed on your computer
- Access to a VoIP network or a sample PCAP file containing VoIP traffic

## Lab Set-up and Tools

1. **Wireshark**: Download and install Wireshark from [https://www.wireshark.org/download.html](https://www.wireshark.org/download.html).
2. **VoIP Network or Sample PCAP File**: Access a VoIP network or download a sample PCAP file containing VoIP traffic.

## Exercises

### Exercise 1: Capture VoIP Traffic

#### Steps

1. Open Wireshark.
2. Select the network interface that connects to the VoIP network.
3. Click on the "Start Capture" button (the blue shark fin icon).
4. Initiate a VoIP call on the network.
5. Let the call proceed for a few moments and then stop the capture in Wireshark by clicking on the red square icon.

#### Expected Output

- A capture file containing VoIP traffic, including call setup, RTP streams, and teardown messages.

### Exercise 2: Filter VoIP Traffic

#### Steps

1. In Wireshark, go to the filter bar at the top.
2. Enter the filter `sip || rtp` and press Enter.
3. Wireshark will display only the SIP and RTP traffic from the capture.

#### Expected Output

- Displayed SIP and RTP traffic filtered from the overall capture.

### Exercise 3: Analyze SIP Packets

#### Steps

1. In the filtered VoIP traffic, locate a SIP INVITE packet.
2. Click on the SIP INVITE packet to view its details in the packet details pane.
3. Expand the "Session Initiation Protocol" section to see detailed information about the call setup, such as the calling and called parties, and session parameters.

#### Expected Output

- Detailed information about a SIP INVITE packet displayed.

### Exercise 4: Analyze RTP Streams

#### Steps

1. In the filtered VoIP traffic, locate an RTP packet.
2. Click on the RTP packet to view its details in the packet details pane.
3. Expand the "Real-Time Transport Protocol" section to see detailed information about the RTP stream, such as payload type, sequence number, and timestamp.
4. Go to "Telephony" > "RTP" > "Stream Analysis" to analyze the RTP stream quality and metrics.

#### Expected Output

- Detailed information about RTP packets and analysis of the RTP stream quality.

### Exercise 5: Playback VoIP Calls

#### Steps

1. In Wireshark, go to "Telephony" > "VoIP Calls".
2. Select the VoIP call you captured and click on "Player".
3. Use the player controls to play back the audio of the VoIP call.
4. Analyze the audio for any issues, such as packet loss, jitter, or poor quality.

#### Expected Output

- VoIP call audio playb
