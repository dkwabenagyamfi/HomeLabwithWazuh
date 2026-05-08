<h1>Wazuh Home Lab</h1>


<h2>Description</h2>
This project transformed a spare Ubuntu server into a fully functional Security Information and Event Management (SIEM) system using Wazuh (open-source). A Kali Linux machine was set up as an agent to simulate a monitored endpoint. Over 48 hours, the system successfully monitored file integrity and logged over 500 security events.

Most importantly, I configured an automated active response that integrates with VirusTotal. When a malicious file (tested safely using the EICAR standard file) was created on the agent, the Wazuh manager automatically detected it, queried VirusTotal for reputation, confirmed the threat, and instantly deleted the file from the agent's disk – without any human intervention

<br />


<h2>Key Achievements</h2>

- <b>✅ Installed and configured Wazuh indexer, server/manager, and dashboard on a single VM.</b> 
- <b>✅ Deployed a Wazuh agent on a separate Linux VM.</b>
- <b>✅ Built a custom dashboard (alerts over time, top agents, top rules).</b>
- <b>✅ Integrated VirusTotal API for file reputation lookup.</b>
- <b>✅ Implemented an active response script to auto-delete malicious files.</b>
- <b>✅ Tested the full workflow safely using the EICAR test virus file.</b>


## 🛠️ Tools Used

| Tool                  | Purpose                                   | License                |
|-----------------------|-------------------------------------------|------------------------|
| Ubuntu 22.04 LTS      | Operating system for both server and agent | Free                   |
| Wazuh (Indexer, Server, Dashboard) | SIEM platform                          | Open Source (GNU GPL)  |
| Wazuh Agent           | Endpoint monitoring                       | Open Source            |
| VirusTotal API        | File reputation service                   | Free (with API key)    |
| EICAR file            | Safe malware test signature               | Free                   |
| Custom Bash Script    | Active response to delete malicious files | Custom script          |


<h2>Program walk-through:</h2>

<p align="center">
Launch the utility: <br/>
<img src="https://i.imgur.com/62TgaWL.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Select the disk:  <br/>
<img src="https://i.imgur.com/tcTyMUE.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Enter the number of passes: <br/>
<img src="https://i.imgur.com/nCIbXbg.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Confirm your selection:  <br/>
<img src="https://i.imgur.com/cdFHBiU.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Wait for process to complete (may take some time):  <br/>
<img src="https://i.imgur.com/JL945Ga.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Sanitization complete:  <br/>
<img src="https://i.imgur.com/K71yaM2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Observe the wiped disk:  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
