<h1>Blue Team Enterprise Lab</h1>

<h2>Description</h2>
This project focused on building an enterprise-style blue team cybersecurity lab using Active Directory, Wazuh SIEM, Sysmon, Windows Server 2022, Windows 10, Ubuntu Server, VirtualBox, PowerShell, and Windows Event Viewer to simulate real-world SOC analyst monitoring and threat investigation workflows.

The lab was designed to demonstrate centralized authentication, endpoint onboarding, Sysmon telemetry collection, Windows process monitoring, PowerShell activity generation, SIEM alert investigation, MITRE ATT&CK mapping, and enterprise security monitoring within a controlled virtualized environment.
<br />

<h2>Languages and Utilities Used</h2>

- <b>Wazuh SIEM</b>
- <b>Sysmon</b>
- <b>Windows Server 2022</b>
- <b>Windows 10</b>
- <b>Ubuntu Server</b>
- <b>Active Directory Domain Services</b>
- <b>VirtualBox</b>
- <b>PowerShell</b>
- <b>Windows Event Viewer</b>
- <b>Wazuh Agent</b>

<h2>Environments Used</h2>

- <b>Windows Server 2022 Domain Controller</b>
- <b>Windows 10 Domain-Joined Endpoint</b>
- <b>Ubuntu Server Wazuh SIEM</b>
- <b>VirtualBox Bridged Networking</b>

<h2>Project Walk-through:</h2>

<p align="center">

Installed and configured Sysmon on the Windows 10 endpoint to enhance process creation monitoring and advanced endpoint telemetry collection: <br/>
<img src="https://i.imgur.com/izPEqkg.png"/>
<br />
<br />

Verified successful Sysmon Operational logging in Windows Event Viewer, confirming that endpoint telemetry and Event ID 1 process creation logs were being generated: <br/>
<img src="https://i.imgur.com/pzSrhSN.png"/>
<br />
<br />

Generated endpoint activity using PowerShell commands such as <code>whoami</code>, <code>ipconfig</code>, <code>net user</code>, and <code>tasklist</code> to create process execution telemetry for investigation: <br/>
<img src="https://i.imgur.com/wRtmhZ1.png"/>
<br />
<br />

Reviewed running processes from the Windows endpoint to observe active system activity and command execution behavior: <br/>
<img src="https://i.imgur.com/MT0QFUP.png"/>
<br />
<br />

Executed PowerShell process monitoring commands to simulate common administrative and attacker-used command-line activity: <br/>
<img src="https://i.imgur.com/7hPnwmN.png"/>
<br />
<br />

Simulated suspicious encoded PowerShell execution to generate potentially malicious command-line telemetry for SOC investigation: <br/>
<img src="https://i.imgur.com/ozCQv7O.png"/>
<br />
<br />

Confirmed that the Windows endpoint was actively communicating with the Wazuh SIEM and generating centralized security alerts: <br/>
<img src="https://i.imgur.com/M1lADGm.png"/>
<br />
<br />

Investigated Wazuh security alerts generated from the Windows endpoint, including authentication and security configuration events: <br/>
<img src="https://i.imgur.com/dP4LZpu.png"/>
<br />
<br />

Analyzed MITRE ATT&CK mapped alert activity within Wazuh, including Windows logon activity associated with <code>T1078 Valid Accounts</code>: <br/>
<img src="https://i.imgur.com/07LypBQ.png"/>
<br />
<br />

Validated centralized blue team monitoring by combining Sysmon telemetry, Windows endpoint activity, Wazuh alerts, and MITRE ATT&CK investigation context inside the SIEM dashboard: <br/>
<img src="https://i.imgur.com/HVQsZhu.png"/>
<br />
<br />

</p>

<h2>Conclusion</h2>

This lab provided hands-on experience with blue team endpoint monitoring, Sysmon telemetry collection, Windows process tracking, PowerShell activity analysis, Wazuh SIEM alert investigation, and MITRE ATT&CK mapped security monitoring.

The project strengthened practical SOC analyst skills by demonstrating how endpoint activity can be generated, collected, reviewed, and investigated through centralized SIEM monitoring in an enterprise-style lab environment.
