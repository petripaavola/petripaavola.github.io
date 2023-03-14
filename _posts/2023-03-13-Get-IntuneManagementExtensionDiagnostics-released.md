---
layout: post
title: Get-IntuneManagementExtensionDiagnostics released
subtitle: Analyze Intune logs, create event Timeline and troubleshoot with LogViewerUI
gh-repo: petripaavola/Get-IntuneManagementExtensionDiagnostics
gh-badge: [star, fork, follow]
tags: [Intune, Autopilot, Powershell]
comments: true
---

New tool: Intune (IME) log Timeline analyzer and LogViewerUI released today:  
[Get-IntuneManagementExtensionDiagnostics](https://github.com/petripaavola/Get-IntuneManagementExtensionDiagnostics)

![Get-IntuneManagementExtensionDiagnostics-Observed_Timeline_v1.1.png](/assets/img/Get-IntuneManagementExtensionDiagnostics-Observed_Timeline_v1.1.png)
![Get-IntuneManagementExtensionDiagnostics-LogViewerUI01_1.1.png](/assets/img/Get-IntuneManagementExtensionDiagnostics-LogViewerUI01_1.1.png)

Quick start guide:

**Download script from Powershell Gallery:**
```powershell
Save-Script Get-IntuneManagementExtensionDiagnostics -Path ./
```

**Run script with or without -Online option:**
```powershell
./Get-IntuneManagementExtensionDiagnostics.ps1 -Online
```

**LogViewUI can be run with command:**
```powershell
./Get-IntuneManagementExtensionDiagnostics.ps1 -Online -ShowLogViewerUI -ConvertAllKnownGuidsToClearText
```

Tool makes Timeline analysis from Intune Management Extension logs. It also includes powerfull LogViewerUI which has text search, filtering, found events and GUID conversion to known names - this alone helps a lot with Intune troubleshooting!

Tool helps a lot with Windows Autopilot and any other Intune debugging. Events are shown for
*  Win32pp
*  WinGetApp
*  Powershell scripts
*  Proactive Remediation scripts
*  custom Compliance Policy scripts.

Tool also shows Win32App download statistics and you can see if **Delivery Optimization** was working in download.  
![Win32App-DeliveryOptimization](/assets/img/Win32App-DeliveryOptimization.png)

And with WinGetApps we are interested in download/install times because we rely on 3rd party websites.

It can also show possible Powershell script ErrorOut and StdOut. Powershell script may not fail but still produce a lot of errors without admin ever knowing (seen that on customers logs). Script also has many other features...

Check out project site for more details and documentation:  
[Get-IntuneManagementExtensionDiagnostics](https://github.com/petripaavola/Get-IntuneManagementExtensionDiagnostics)

Happy Intune logs troubleshooting :)
