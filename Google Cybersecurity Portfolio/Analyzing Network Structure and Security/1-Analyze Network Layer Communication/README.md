**TASK**

In this Scenario, I was a cybersecurity analyst employed by a company specializing in IT consulting services. Multiple customers had reached out to the company, reporting their inability to access the company website, www.yummyrecipesforme.com. They encountered the error message "destination port unreachable" after an extended loading period.

My assignment was to investigate the issue and identify which network protocol was impacted. My investigation commenced with a visit to the website, where I also encountered the "destination port unreachable" error message. Subsequently, I activated my network analysis tool, tcpdump, and reloaded the webpage. This time, I observed a significant influx of packets in my network analyzer.

My analysis revealed that when I send UDP packets and receive an ICMP response back to the host, these responses contained an error message indicating "udp port 53 unreachable." I examined the DNS and ICMP log for the following;

1. My initial outgoing request to the DNS server for the IP address of www.yummyrecipesforme.com. Request was sent in  UDP packet
2. Timestamps that indicated when the event happened
3. The source and destination IP address
4. Next was the protocol and port number which indicated the protocol that was used to handle communication and the port it was delivered to

I examined the rest of the log to understand what the main issues were. Afterwards, i did a follow-up report which is attached to the task. Also, This project highlighted my capacity to scrutinize network traffic and pinpoint the underlying source of network-related problems, a vital competency for cybersecurity analysts.

