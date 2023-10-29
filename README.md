<h1>Failed RDP to IP Geolocation Information</h1>

<h2>Description</h2>
<b>The Powershell script that's found in this repository is used to parse out Windows Event Log information for failed RDP attacks.  A third-party API is used to collect the associated geographic information about the attacker's location.</b>
<br />
<br />
The script is used in this project where I have setup Azure Sentinel (SIEM) and connected it to a live virtual machine that was acting as a honey pot.  The aim was to capture and observe live attacks (RDP Brute Force) from around the world.  I used a custom PowerShell script to lookup the attackers' Geolocation information and plotted it on an Azure Sentinel Map.
<br />
<br />

<p align="center">
<img src="https://i.imgur.com/ZDd5czc.png" height="85%" width="85%" alt="RDP event fail logs IP Geographic information"/>
<br />
<br />
<h2><b>Languages Used</b></h2>
- <b>Powershell: </b> Extract RDP failed logon logs from Windows Event Viewer
<br />
<br />
<h2><b>Utilities Used</b></h2>
- <b>ipgeolocation.io:</b> IP Address to Geolocation API
<br />
<br />
<h2><b>Attacks from Kazakhstan coming in; Custom logs being output with geodata</b></h2>
<p align="center">
<img src="https://i.imgur.com/fDgxwty.png" height="85%" width="85%" alt="RDP event fail logs IP Geographic information"/>
<br />
<br />
<h2><b>World map of incoming attacks after 6 hours (built custom logs including geodata)</b></h2>
<p align="center">
<img src="https://i.imgur.com/TDiPo1o.png" height="85%" width="85%" alt="RDP event fail logs IP Geographic information"/>
