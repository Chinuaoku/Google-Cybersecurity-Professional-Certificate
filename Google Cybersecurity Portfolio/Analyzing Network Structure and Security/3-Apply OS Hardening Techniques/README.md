**TASK**


I am a cybersecurity analyst for yummyrecipesforme.com, a website specializing in the sale of recipes and cookbooks. Recently, we encountered a security breach when an upset baker decided to make our best-selling recipes available to the public for free.

The baker employed a brute force attack to gain access to our web host. This involved repeated attempts to enter various known default passwords for the administrative account until they successfully guessed the correct one. Once they had the login credentials, they accessed the admin panel and manipulated the website's source code. In doing so, they embedded a JavaScript function that triggered visitors to download and run a file upon entering the website. This led our customers to be redirected to a fraudulent version of our site where our recipes were accessible for free.

Within hours of the attack, multiple customers contacted our helpdesk, reporting that our website had prompted them to download a file for a browser update. After running the file, they noticed changes in the website's address, and their personal computers started to operate slowly.

In response, our website owner attempted to log in to the admin panel but was unsuccessful. Consequently, they contacted our website hosting provider. As cybersecurity analysts, we were assigned the task of investigating this security incident.

To address the situation, I established a sandbox environment to monitor the suspicious behavior of the website. I utilized the network protocol analyzer tcpdump and input the URL for our website, yummyrecipesforme.com. Upon loading the website, I encountered a prompt to download an executable file for a browser update. I accepted the download and allowed the file to run, subsequently observing a browser redirection to a different URL, greatrecipesforme.com. This new site was designed to mimic our original website, but it now featured our company's recipes available for free.

The logs showed the following process; The browser requested a DNS resolution of the yummyrecipesforme.com URL, the DNS replied with the correct IP address, the browser initiated a http request for the webpage and the download of malicious software. The browser also requested another DNS resolution for greaterrecipesforme.com, the DNS server responded with the new IP address and the browser initiated a http request to the new address.

Upon analysis, a senior analyst confirmed that the website had indeed been compromised. The source code examination revealed the insertion of JavaScript code, prompting visitors to download an executable file. Analysis of the downloaded file disclosed a script that redirected visitors' browsers from yummyrecipesforme.com to greatrecipesforme.com.

The cybersecurity team's assessment indicated that the web server had been subjected to a brute force attack. The ease with which the disgruntled baker guessed the password was attributed to the continued use of the default password for the admin account. Furthermore, the absence of effective controls to prevent a brute force attack was identified as a contributing factor to the incident.

This project demonstrated my proficiency in evaluating incidents, mitigating threats, and formulating proactive security strategies.
