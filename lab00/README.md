Shane Ferrell

EEL4598 Fall 2023

# Lab 0 Report

**Summary**

This lab included the setting and exploration of Wireshark, a packet analyzer that can be used to capture and investigate messages sent over a network.

**Running Wireshark**

Wireshark is an open-source packet sniffer and packet analyzer tool. A packet sniffer is a software tool that can passively capture and inspect data packets on a computer network. A packet analyzer is a software tool that can passively capture data packets on a computer network and provides advanced analysis features to inspect packets.

The Wireshark packet capture library serves as the underlying infrastructure that allows Wireshark to capture, dissect, and analyze network packets from various network interfaces. The library receives a copy of every data link layer frame sent and received by the computer. A data link layer frame is a data packet format that operates at the data link layer of the OSI or second layer of the TCP/IP model and is responsible for transmitting data over a physical medium (e.g. ethernet cables, Wi-Fi).

After downloading and installing the Wireshark application, a user can launch the application to the startup screen shown in Figure 1.

![](RackMultipart20230903-1-x8sc22_html_4791116f46383488.jpg)

_Figure 1: Wireshark startup screen_

The user can view the capture interfaces by selecting the Capture button. The interfaces are shown in Figure 2. ![](RackMultipart20230903-1-x8sc22_html_2b2e41da99226f37.jpg)

_Figure 2: Wireshark capture interfaces_

Packet capture begins when interfaces are selected. Figure 3 shows packets on the network that were captured by Wireshark. Some common protocols of these messages are TCP, DNS, and SSDP.

![](RackMultipart20230903-1-x8sc22_html_8aaa2235e5a97e28.jpg)

_Figure 3: List of packets captured by Wireshark_

To test the capture of HTTP requests, a browser was used to visit a sample web page. The web page is shown in Figure 4.

![](RackMultipart20230903-1-x8sc22_html_cb52fbd7da0bc999.jpg)

_Figure 4: Sample web page_

The packets captured by Wireshark when the web page is accessed are shown in Figure 5.

![](RackMultipart20230903-1-x8sc22_html_97d40c0c7d608564.jpg)

_Figure 5: Packets captured when accessing web page_

Messages matching certain criteria can be filtered. Figure 6 shows Wireshark when a filter is applied to display only HTTP messages.

![](RackMultipart20230903-1-x8sc22_html_b4b542f9e3a98229.jpg)

_Figure 6: Captured HTTP messages from web page_

The computer running Wireshark sent an HTTP GET request message to the web page server and received an HTTP OK message 0.025 seconds after. The address of the web page server is 23.34.82.10 and the address of my computer is 192.168.0.172.

Figure 7 shows the HTTP GET request message. The HTTP protocol information is displayed.

![](RackMultipart20230903-1-x8sc22_html_e3ffdc6c267ce7c.jpg)

_Figure 7: HTTP GET request message details_
