<h1>Failed RDP to IP Geolocation Information</h1>

### Project Overview

<h2>Description</h2>
<b>This repository houses a PowerShell script designed to parse failed RDP attack logs from Windows Event Viewer and enrich these logs with geographic information of the attackers by leveraging a third-party API. This script plays a crucial role in visualizing the origin of cyber-attacks on a global scale, utilizing Azure Sentinel for real-time analysis and mapping.</b>
<br />
<br />
In this demonstration, a live virtual machine acts as a honeypot to attract RDP Brute Force attacks from across the globe. The custom PowerShell script extracts failed login attempts, queries an IP Geolocation API for the attackers' location data, and visualizes this on a map within Azure Sentinel.
<br />
<br />

<h2>Key Technologies</h2>

- <b>PowerShell:</b> Used for extracting failed RDP logon attempts and interacting with the IP Geolocation API.
- <b>Azure Sentinel:</b> Microsoft's SIEM system for real-time analytics and mapping of cyber-attacks.
- <b>Virtual Machine:</b> Set up as a honeypot to monitor and analyze RDP Brute Force attacks.

<h2>Utilities Used</h2>

- <b>IP Geolocation API (ipgeolocation.io):</b> Provides geographic information based on IP addresses of attackers.

<h2>Insights into Attack Patterns</h2>

As the honeypot VM exposes vulnerabilities to the internet, it swiftly becomes a target for attackers worldwide. The collected data unveils patterns, frequency, and geographical distribution of cyber-attacks, highlighting the global nature of cyber threats.

<h2>Visualization of Attack Data</h2>

<p align="center">
<b>Initial Findings:</b> Snapshot of attack origins with geolocation data.
<br />
<img src="https://i.imgur.com/2MViSiL.jpg" height="85%" width="85%" alt="Initial attack data visualization"/>
</p>

<p align="center">
<b>24-Hour Analysis:</b> Comprehensive world map showing the distribution of attacks after 24 hours, enriched with custom geodata logs.
<br />
<img src="https://i.imgur.com/krRFrK5.png" height="85%" width="85%" alt="24-hour attack data analysis"/>
</p>

This project underscores the importance of robust cybersecurity measures and demonstrates the utility of honeypots in understanding and mitigating cyber threats.
