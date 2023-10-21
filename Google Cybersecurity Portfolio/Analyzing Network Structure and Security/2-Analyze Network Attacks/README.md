**TASK**

I work as a security analyst for a travel agency, which promotes sales and promotions on its website. Our company's employees frequently access the sales webpage to search for vacation packages suitable for our customers.

One afternoon, I received an automated alert from our monitoring system, indicating an issue with the web server. To investigate, I tried to access the company's website but encountered a connection timeout error message in my browser.

To identify the problem, I employed a packet sniffer to capture data packets traveling to and from the web server. It became evident that an unusual volume of TCP SYN requests was originating from an unfamiliar IP address. The web server was struggling to handle this influx of traffic, resulting in an overwhelming number of SYN requests. This raised suspicions of a malicious attack.

As a response, I temporarily took the server offline to allow it to recover and return to normal operation. Additionally, I configured the company's firewall to block the IP address responsible for the abnormal SYN requests. However, I was aware that this IP blocking solution was not a long-term fix, as an attacker could potentially employ IP address spoofing to circumvent this block.

Recognizing the urgency of the situation, I promptly contacted my manager to report the issue and discuss our next steps for mitigating the attack and preventing future occurrences.

The first thing we did was to try and identify the type of network attack this was. We did this by considering the type of attack that will result in the indications of attack in the scenario, difference between a DOS and DDOS attack and why the website was taking so long to load and reporting a connection timeout error. 

We reviewed the wireshark log and tried to identify patterns in the logged network traffic.

This project serves as a demonstration of my proficiency in managing critical incidents, addressing imminent threats, and devising comprehensive strategies to protect an organization's digital assets.
