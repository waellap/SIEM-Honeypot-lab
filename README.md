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


-Creating a resource group and virtual network(home router).
<img src="https://imgur.com/oBWor6Q.png" height="80%" width="80%" alt="Disk Sanitization Steps"/><img src="https://imgur.com/qUTCQrW.png" height="80%" width="80%" alt="Disk Sanitization Steps"/><img src="https://imgur.com/5cR54n5.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>


<br />
<br />


-Creating the honeypot, which will be Windows 10.

<img src="https://imgur.com/casE3Ic.png" height="80%" width="80%" alt="Disk Sanitization Steps"/><img src="https://imgur.com/DnBGFgk.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<br />
<br />


-Now we created everything which we the network security group is the firewall, network interface, and ethernet port.

<img src="https://imgur.com/9ci2vJG.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />


-I add inbound traffic,  which can receive traffic from any any.


<img src="https://imgur.com/g700mVm.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />


Log in to Windows 10, aka (Honeypot).


<img src="https://imgur.com/YTwr0rc.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />


-Turning the WF.msc or the Windows Firewall off


<img src="https://imgur.com/wA58yIy.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />


-Creating a log repository, then add it to the SIEM.

<img src="https://imgur.com/GdhGsYC.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> <img src="https://imgur.com/zcwnR4x.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />



-Creating Data collection rule.

<img src="https://imgur.com/ZwLKSKZ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />


-Querying the logs repository with KQL and searching for a security event.


<img src="https://imgur.com/vb3AvSb.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
-Time generated, Account, computer, eventId, activity, ipaddress.
<br />
<br />
<img src="https://imgur.com/z6tu1Sz.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://imgur.com/vb3AvSb.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

- I added a Jason file to my Sentinel workbook to see the location of the attacks in the map and where they're coming from.


<img src="https://imgur.com/1W3lAy1.png" height="80%" width="80%" alt="Disk Sanitization Steps"/><img src="https://imgur.com/URGYW2r.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> <img src="https://imgur.com/GkNG2Cq.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>


<br />
<br />



