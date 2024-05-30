# Analyzing HTTP Traffic with Wireshark

## Introduction

In this project, you'll learn how to use Wireshark to capture and analyze HTTP traffic. HTTP traffic analysis is crucial for understanding web communication, identifying potential security issues, and investigating anomalies in network traffic.

## Pre-requisites

- Basic understanding of networking concepts
- Wireshark installed on your computer
- A web browser for generating HTTP traffic

## Lab Set-up and Tools

1. **Wireshark**: Download and install Wireshark from [https://www.wireshark.org/download.html](https://www.wireshark.org/download.html).
2. **Web Browser**: Any modern web browser (e.g., Chrome, Firefox) for generating HTTP traffic.

## Exercises

### Exercise 1: Capture HTTP Traffic

#### Steps

1. Open Wireshark.
2. Select the network interface that connects to the internet.
3. Click on the "Start Capture" button (the blue shark fin icon).
4. Open your web browser and navigate to a website that uses HTTP (e.g., http://example.com).
5. Let the page load completely and then stop the capture in Wireshark by clicking on the red square icon.

#### Expected Output

- A capture file containing network traffic, including HTTP requests and responses.

### Exercise 2: Filter HTTP Traffic

#### Steps

1. In Wireshark, go to the filter bar at the top.
2. Enter the filter `http` and press Enter.
3. Wireshark will display only the HTTP traffic from the capture.

#### Expected Output

- Displayed HTTP traffic filtered from the overall capture.

### Exercise 3: Analyze HTTP Requests

#### Steps

1. In the filtered HTTP traffic, locate an HTTP GET request.
2. Click on the GET request to view its details in the packet details pane.
3. Expand the "Hypertext Transfer Protocol" section to see detailed information about the request, such as the requested URL, headers, and parameters.

#### Expected Output

- Detailed information about an HTTP GET request displayed.

### Exercise 4: Analyze HTTP Responses

#### Steps

1. In the filtered HTTP traffic, locate the corresponding HTTP response for the GET request you analyzed.
2. Click on the response to view its details in the packet details pane.
3. Expand the "Hypertext Transfer Protocol" section to see detailed information about the response, such as the status code, headers, and content type.

#### Expected Output

- Detailed information about an HTTP response displayed.

### Exercise 5: Extract and Examine Payload Data

#### Steps

1. In the HTTP response details, look for the payload data (e.g., HTML content).
2. Right-click on the response packet and select "Follow" > "TCP Stream" to view the entire HTTP conversation.
3. Examine the payload data in the TCP stream window to understand the content being transferred.

#### Expected Output

- Payload data from the HTTP response extracted and examined.

## Conclusion

By completing these exercises, you have learned how to capture, filter, and analyze HTTP traffic using Wireshark. These skills are essential for understanding web communication, troubleshooting network issues, and performing security investigations.
