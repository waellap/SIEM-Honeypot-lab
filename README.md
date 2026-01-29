# SIEM-Honeypot-lab

##  Objective
Detecting Malware using Splunk and Sysmon

The objective of this project is to **design and implement a cloud-based cybersecurity home lab featuring a honeypot, leveraging Microsoft Azure and Microsoft Sentinel to monitor, analyze, and visualize real-world attack activity, while gaining hands-on experience in security operations and threat detection**.

### Skills Learned
“I learned to set up a cloud lab, use a honeypot, analyze security logs, detect threats, and visualize attack data.”

- Cloud Infrastructure Setup – Creating and configuring Azure resources, including virtual machines and workspaces.
- Honeypot Deployment – Setting up a honeypot to attract and monitor real-world cyber attacks.- Basic cybersecurity operations
- SIEM configuration and usage – working with Microsoft Sentinel to ingest, analyze, and visualize log data from your environment.
-Log analytics and querying – using tools such as Kusto Query Language (KQL) to pull meaningful insights from collected security events.
- Development of critical thinking and problem-solving skills in cybersecurity.
- Threat detection and visualization – interpreting attack patterns, generating geographic maps of attacker IP sources, and tracking security events in real time.

### Tools Used
Microsoft Azure, Azure Virtual Machine (VM), Log Analytics Workspace, Microsoft Sentinel (SIEM), and Kusto Query Language (KQL).

- 🟦 Microsoft Azure – the cloud platform where the home lab is hosted.
- 🖥️ Azure Virtual Machine (VM) – runs a server exposed to the internet to attract attacker traffic.
- 📊 Log Analytics Workspace – a central location in Azure for collecting logs from the VM.
- 🛡️ Microsoft Sentinel (SIEM) – cloud-native SIEM used to receive logs, run queries, detect threats, and visualize activity.
- 🔍 Kusto Query Language (KQL) – used for querying data inside Sentinel’s log analytics.

##  Steps
Lab photo demonstration.


-Creating the Malware using msfvenom.
<img src="https://imgur.com/a/tVJUh6l#xeLw4R0.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />


-After creating the malware in this step, we will exploit.

<img src="https://imgur.com/qHgRqD3.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />


-Creating the HTTP.Server.

<img src="https://imgur.com/8LWykK9.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />


-Turning down the malware detector in Windows Defender.


<img src="https://imgur.com/zxRYS7f.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />


-Connecting to the server and choosing the exe file, aka (malware folder).


<img src="https://imgur.com/loAu4PC.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />


-Download the exe file (Resume.pdf.exe) and run it


<img src="https://imgur.com/bcXDOsy.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />


-After running the malware folder, checking it through the cmd by running Netstat -anob. Then The 
connection is established

<img src="https://imgur.com/L6SZByZ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />



-Ingesting the sysmon and creating an index called endpoint 
-Setting->index->new index-> endpoint->Apps->Search and reporting->index endpoint.


<img src="https://imgur.com/Fp16zSS.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />



-Searching for the malware name (Resume.pdf.exe), I found 13 events.

<img src="https://imgur.com/yd4OxpT.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />


-I use process guid in the search menu and found 5 events. I clean up the query and looked into the statistics.


<img src="https://imgur.com/G9rWjyY.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />


