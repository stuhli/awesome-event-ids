# Awesome Event IDs

> Collection of Event ID resources useful for Digital Forensics and Incident Response

In incidents, analysts are often faced with the problem of interpreting unknown event IDs.
The event itself does not always contain the desired information.
In addition, it is impossible to remember them all, given the huge number of event IDs and log sources.

## Contents

- [Awesome Event IDs](#awesome-event-ids)
  - [Contents](#contents)
  - [Resources](#resources)
    - [Event ID databases](#event-id-databases)
    - [Event ID documentation](#event-id-documentation)
    - [Event ID configuration and monitoring suggestions](#event-id-configuration-and-monitoring-suggestions)
    - [Event ID analysis](#event-id-analysis)
  - [Contributing](#contributing)

## Resources

### Event ID databases

- [EventID.net](http://www.eventid.net/search.asp) - Database
- [EventTracker Knowledgebase](https://kb.eventtracker.com/) - Database
- [MyEventlog.com](https://www.myeventlog.com/) - Database

### Event ID documentation

- [Kaspersky Security for Microsoft Exchange](https://support.kaspersky.com/KS4Exchange/9.6/en-US/127197.htm) - Official resource.
- [Microsoft Defender Antivirus](https://docs.microsoft.com/en-us/microsoft-365/security/defender-endpoint/troubleshoot-microsoft-defender-antivirus?view=o365-worldwide#microsoft-defender-antivirus-event-ids) - Official resource.
- [Microsoft Windows Security Auditing](https://docs.microsoft.com/en-us/windows/security/threat-protection/auditing/security-auditing-overview) - Official resource.
- [Microsoft Windows Security Auditing by Randy Franklin Smith](https://www.ultimatewindowssecurity.com/securitylog/encyclopedia/) - Better known as _Ultimate Windows Security_.
- [Notable Event IDs](https://github.com/TonyPhipps/SIEM/blob/master/Notable-Event-IDs.md) - Collection of common event IDs with descriptions.
- [Sysmon](https://docs.microsoft.com/en-us/sysinternals/downloads/sysmon#events) - Official resource.
- [Symantec Endpoint Protection 14.0.X](https://knowledge.broadcom.com/external/article/170359/endpoint-protection-140x-event-log-entri.html) - Official resource.
- [Symantec Endpoint Protection Manager](https://knowledge.broadcom.com/external/article/157017/endpoint-protection-manager-event-log-en.html) - Official resource.
- [McAfee VirusScan Enterprise 8.x](https://kcm.trellix.com/corporate/index?page=content&id=KB54827) - VirusScan Enterprise entries in the Windows Application Event Log (Official resource).
- [Compilation of Event IDs](http://www.chicagotech.net/wineventid.htm) - Collection of event IDs from 1 to 9999 and above.
- [Events and Errors - Windows Server 2008](https://docs.microsoft.com/en-us/previous-versions/windows/it-pro/windows-server-2008-r2-and-2008/cc754424(v=ws.10)) - Collection of event IDs from different windows event source. Applies to Windows Server 2008 and similar. (Official resource)
- [Finding Forensic Goodness In Obscure Windows Event Logs](https://nasbench.medium.com/finding-forensic-goodness-in-obscure-windows-event-logs-60e978ea45a3) - List of lesser-known Event IDs.

### Event ID configuration and monitoring suggestions

- General
  - [SIEM Tactics, Techniques, and Procedures](https://github.com/TonyPhipps/SIEM) - Comprehensive SIEM resources be TonyPhipps.
  - [Windows Auditing Mindmap](https://github.com/mdecrevoisier/Windows-auditing-mindmap) - Set of Mindmaps providing a detailed overview of the different Windows auditing capacities and event log files.
- PowerShell
  - [Script Block Logging](https://docs.microsoft.com/en-us/powershell/module/microsoft.powershell.core/about/about_logging_windows?view=powershell-7.1#viewing-the-powershell-event-log-entries-on-windows) - Enable 4104.
  - [Module Logging](https://docs.microsoft.com/en-us/powershell/module/microsoft.powershell.core/about/about_group_policy_settings?view=powershell-7.1#turn-on-module-logging)
  - [Malware Archeology PowerShell Logging Cheat Sheet](https://www.malwarearchaeology.com/s/Windows-PowerShell-Logging-Cheat-Sheet-ver-Sept-2018-v22.pdf)
  - [Greater Visibility Through PowerShell Logging](https://www.mandiant.com/resources/greater-visibilityt)
  - [PowerShell Logging for the Blue Team](https://www.blackhillsinfosec.com/powershell-logging-blue-team/)
- Security Auditing
  - [Command line Process Auditing](https://docs.microsoft.com/en-us/windows-server/identity/ad-ds/manage/component-updates/command-line-process-auditing#configuration) - Enable 4688 featuring command line.
  - [Events to Monitor](https://docs.microsoft.com/en-us/windows-server/identity/ad-ds/plan/appendix-l--events-to-monitor) - Official resource.
  - [Monitoring Guidance](https://github.com/JSCU-NL/logging-essentials) - Event monitoring guidance from JSCU (Joint SIGINT Cyber Unit) from Netherlands. With  volume estimates, and WEC/WEF configurations.
  - [Malware Archeology Windows Logging Cheat Sheet](https://www.malwarearchaeology.com/s/Windows-Logging-Cheat-Sheet_ver_Feb_2019.pdf)
  - [Malware Archeology Advanced Windows Logging Cheat Sheet](https://www.malwarearchaeology.com/s/Windows-Advanced-Logging-Cheat-Sheet_ver_Feb_2019_v12.pdf)
  - [Malware Archeology Splunk Logging Cheat Sheet](https://www.malwarearchaeology.com/s/Windows-Splunk-Logging-Cheat-Sheet-v222.pdf) - about specific exclusions to avoid getting noise from the Splunk Universal Forwarder agent.
  - [Malware Archeology File Auditing Cheat Sheet](https://www.malwarearchaeology.com/s/Windows-File-Auditing-Cheat-Sheet-ver-Nov-2017-3fwr.pdf)
  - [Malware Archeology Registry Auditing Cheat Sheet](https://www.malwarearchaeology.com/s/Windows-Registry-Auditing-Cheat-Sheet-ver-Aug-2019.pdf)
  - [Malware Archeology ATT&CK Logging Cheat Sheet](https://www.malwarearchaeology.com/s/Windows-ATTCK_Logging-Cheat-Sheet_ver_Sept_2018.pdf) - From 2018.
  - [US NSA Spotting the Adversary with Windows Event Log Monitoring](https://apps.nsa.gov/iaarchive/library/ia-guidance/security-configuration/applications/assets/public/upload/Spotting-the-Adversary-with-Windows-Event-Log-Monitoring.pdf) - Covers quite a lot of ground.
    - [US NSA Event Forwarding Guidance](https://github.com/nsacyber/Event-Forwarding-Guidance) - Companion repository with WEF configurations, scripts to configure WEF, and WEB subscriptions in XML format.
  - [UK NCSC - Logging Made Easy WEC (Windows Event Collection) Configuration File](https://github.com/ukncsc/lme/blob/master/Chapter%201%20Files/lme_wec_config.xml)
  - [Windows Security Monitoring - Policy & Event IDs](https://docs.google.com/spreadsheets/d/1BhR3cymZ53ZJfJdKAGKszuB-jgsr8GBJBOCJl50WGKE/edit?usp=sharing) - Spreadsheet with recommendations sorted by system functions.
  - [EventID Policy Map](https://docs.google.com/spreadsheets/d/16WuMNL5WWjE4YJIKrt1ut3fZWTbPPKnAGBjGilLrzBE/edit#gid=1714197816) - Spreadsheet with policy map as well as reference collection.
  - [Windows security event log library](https://www.manageengine.com/products/active-directory-audit/kb/windows-event-log-id-list.html) - Small database with explanations and monitoring suggestions.

- Sysmon
  - [Configuration by SwiftOnSecurity](https://github.com/SwiftOnSecurity/sysmon-config) - Configuration file template with default high-quality event tracing.
    - [Fork of SwiftOnSecurity by Neo23x0 Florian ROTH](https://github.com/Neo23x0/sysmon-config) - Same as above, with all PR.
  - [Configuration by olafhartong](https://github.com/olafhartong/sysmon-modular) - A repository of Sysmon configuration modules.
  - [Malware Archeology Sysmon Logging Cheat Sheet](https://www.malwarearchaeology.com/s/Windows-Sysmon-Logging-Cheat-Sheet_Jan_2020-g7sl.pdf)
  - [Sysmon Community Guide](https://github.com/trustedsec/SysmonCommunityGuide)

### Event ID analysis

- General
  - [EVTX Attack Samples](https://github.com/sbousseaden/EVTX-ATTACK-SAMPLES) - EVTX samples recorded during attack simulations by sbousseaden.
  - [EVTX-to-MITRE-Attack](https://github.com/mdecrevoisier/EVTX-to-MITRE-Attack) - More than 170 EVTX samples matched to MITRE TTPs provided by [mdecrevoisier](https://twitter.com/mdecrevoisier)
  - [Tool Analysis Result Sheet](https://jpcertcc.github.io/ToolAnalysisResultSheet/#) - Logs analyzed after tool execution by JPCERT.
  - [EvtxECmd Map Repository](https://github.com/EricZimmerman/evtx/tree/master/evtx/Maps) - Maps used by Eric Zimmerman's EvtxECmd which provide examples of Event IDs with documentation, lookup tables, and important values within each respective event ID which are parsed by EvtxECmd using the associated Map.
  - [Event Log Observer](https://lizard-labs.com/event_log_observer.aspx) - View, analyze and monitor events recorded in Microsoft Windows event logs.
- PowerShell
  - [Attack and Defense Around PowerShell Event Logging](https://nsfocusglobal.com/attack-and-defense-around-powershell-event-logging/) - PowerShell logging deep dive from different perspectives by Mina Hao.
- RDP
  - [RDP Logon / Logoff events 1](https://ponderthebits.com/2018/02/windows-rdp-related-event-logs-identification-tracking-and-investigation/) - RDP event chain by Jonathon Poling.
  - [RDP Logon / Logoff events 2](https://dfironthemountain.wordpress.com/2019/02/15/rdp-event-log-dfir/) - RDP deep dive on 1149 by Mike Cary.
- Task Scheduler
  - [Common Task Scheduler Event IDs](https://www.cyprich.com/blog/2017/03/29/common-task-scheduler-event-ids/) - List of the most common Event IDs for Windows Scheduled Tasks by djc.

## Contributing

This repo is dedicated to everything that has an event ID and the knowledge about it.
Please ask yourself before submitting a PR if it really fits to this.
In particular, please do not contribute tools, as these are already comprehensively summarized in the following great repositories.

- [awesome-incident-response](https://github.com/meirwah/awesome-incident-response)
- [awesome-forensics](https://github.com/cugu/awesome-forensics)
- [awesome-forensicstools](https://github.com/ivbeg/awesome-forensicstools)
- [awesome-security](https://github.com/sbilly/awesome-security)
