# Awesome Event IDs

> Collection of Event ID ressources useful for Digital Forensics and Incident Response

In incidents, analysts are often faced with the problem of interpreting unknown event ids.
The event itself does not always contain the desired information.
In addition, it is impossible to remember them all, given the huge number of event ids and log sources.

## Contents

- [Event ID search engines](#event-id-search-engines)
- [Event ID collections](#event-id-collections)
- [Event ID configuration and monitoring suggestions](#event-id-configuration-and-monitoring-suggestions)
- [Event ID attack results](#event-id-attack-results)

## Ressources

### Event ID search engines

* [EventID.net](http://www.eventid.net/search.asp)
* [MyEventlog.com](https://www.myeventlog.com/)
* [EventTracker Knowledgebase](https://kb.eventtracker.com/)

### Event ID collections

* [Kaspersky Security for Microsoft Exchange](https://support.kaspersky.com/KS4Exchange/9.4/en-US/127197.htm) - Official resource
* [Microsoft Defender Antivirus](https://docs.microsoft.com/en-us/microsoft-365/security/defender-endpoint/troubleshoot-microsoft-defender-antivirus?view=o365-worldwide#microsoft-defender-antivirus-event-ids) - Official resource
* [Microsoft Windows Security Auditing](https://docs.microsoft.com/en-us/windows/security/threat-protection/auditing/security-auditing-overview) - Official resource
* [Microsoft Windows Security Auditing by Randy Franklin Smith](https://www.ultimatewindowssecurity.com/securitylog/encyclopedia/) - Better known as _Ultimate Windows Security_
* [Sysmon](https://docs.microsoft.com/en-us/sysinternals/downloads/sysmon#events) - Official resource

### Event ID configuration and monitoring suggestions

* PowerShell
    * [Script block logging](https://docs.microsoft.com/en-us/powershell/module/microsoft.powershell.core/about/about_logging_windows?view=powershell-7.1#viewing-the-powershell-event-log-entries-on-windows) - How to activate
* Security Auditing
    * [Command line process auditing](https://docs.microsoft.com/en-us/windows-server/identity/ad-ds/manage/component-updates/command-line-process-auditing#configuration) - How to activate
    * [Events to monitor](https://docs.microsoft.com/en-us/windows-server/identity/ad-ds/plan/appendix-l--events-to-monitor) - Official resource
* Sysmon
    * [Configuration by SwiftOnSecurity](https://github.com/SwiftOnSecurity/sysmon-config) - Configuration file template with default high-quality event tracing
    * [Configuration by olafhartong](https://github.com/olafhartong/sysmon-modular) - A repository of sysmon configuration modules

### Event ID attack results

* [EVTX Attack Samples by sbousseaden](https://github.com/sbousseaden/EVTX-ATTACK-SAMPLES)
* [Tool Analysis Result Sheet by JPCERT](https://jpcertcc.github.io/ToolAnalysisResultSheet/#)
