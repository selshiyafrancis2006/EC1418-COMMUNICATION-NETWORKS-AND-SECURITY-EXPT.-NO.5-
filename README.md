# Analysis of HTTP and HTTPS Traffic Using Wireshark
# AIM
To capture and analyze network traffic using Wireshark, compare the security characteristics of HTTP and HTTPS traffic, and simulate a controlled Man-in-the-Middle (MITM) attack scenario to assess vulnerabilities and mitigation measures.
# EQUIPMENTS REQUIRED
●	Computer/Laptop with Internet connection
●	Wireshark software
●	Web browser (Google Chrome/Firefox)
# PROCEDURE
# Part A: Capturing Network Traffic
1.	Open Wireshark.
2.	Go to Capture → Options.
3.	Select the active Wi-Fi/Ethernet network interface.
4.	Click Start to begin capturing packets.
5.	Open a web browser and generate some web traffic.
6.	After collecting sufficient packets, stop the capture in Wireshark.
 

# Part B: Analysis of HTTP Traffic
1.	In the Wireshark display filter bar, enter:
http
2.	Press Enter.
3.	Observe the HTTP packets generated during web browsing.
4.	Select an HTTP request packet and inspect the packet details.
5.	Observe information such as:
○	Request method (GET/POST)
○	Host name
○	Requested resource
○	HTTP headers
6.	Note that normal HTTP communication does not provide encryption for the application data.
 
# Part C: Analysis of HTTPS Traffic
1.	Clear the previous display filter.
2.	Apply the filter:
tls
3.	Press Enter.
4.	Visit an HTTPS-enabled website.
5.	Observe the TLS/HTTPS packets.
6.	Inspect the TLS handshake packets and identify information such as:
○	Client Hello
○	Server Hello
○	Certificate exchange
○	Encrypted application data
7.	Compare these packets with HTTP traffic.
8.	Observe that the actual application data is encrypted and is not directly readable in the packet capture.
# OUTPUT

<img width="1011" height="592" alt="Screenshot 2026-08-28 154443" src="https://github.com/user-attachments/assets/43ba854d-9fed-4cf1-8a20-429f758087d6" />
<img width="1021" height="668" alt="Screenshot 2026-08-28 152545" src="https://github.com/user-attachments/assets/ef61e97a-6a61-4f5a-bd8b-eb490105f81c" />


# RESULT
Thus, the network traffic was successfully captured and analyzed using Wireshark. HTTP traffic was found to transmit data without encryption, making it vulnerable to interception and modification. .

