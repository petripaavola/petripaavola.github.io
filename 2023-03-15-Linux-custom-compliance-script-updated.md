---
layout: post
title: Intune Linux Custom Compliance script updated
subtitle: Create your own Linux Custom Compliance checks
thumbnail-img: /assets/img/Intune_Linux_CustomComplianceCheck_Compliant.png
share-img: /assets/img/Intune_Linux_CustomComplianceCheck_Compliant.png
tags: [Intune, Linux, Powershell]
comments: true
---
Last year I created Intune Linux Custom Compliance script and it has been running few months now without any problems.

There are new compliance checks compared to original version so I updated script to my GitHub site.  

GitHub page has more documentation on how script works so go and check that out.
[Linux Custom Compliance script on my GitHub](https://github.com/petripaavola/Intune/tree/master/Linux)

![Intune_Linux_CustomComplianceCheck_Compliant.png](/assets/img/Intune_Linux_CustomComplianceCheck_Compliant.png)

Bash script includes Powershell script inside which will do the actual compliance checks so prereq is to install Powershell. And why wouldn't you install Powershell to your Linux anyway ?-)

## Custom Compliance checks in this version:
* **Powershell is installed**
* **Powershell version**
  * 7.3.3 minimum currently configured in json
* **Reboot Required check**
  * file should not exist /var/run/reboot-required)
* **MS Edge**
  * Check MS Edge is installed
    * file should exist /opt/microsoft/msedge/msedge
  *	Check MS Edge version
* **Kernel version**
  *	Check Kernel version
    * 5.19.35-generic minimum currently configured in json
  *	Check Kernel patch level
  *	Check Kernel flavour
  *	Check Kernel tainted state
* **SecureBoot status**
  * require SecureBoot configured in json
* **sysctrl values** (placeholder to check any value)
  *	user.max_user_namespaces
* **gsettings values**  (placeholder to check any value)
  *	org.gnome.desktop.screensaver lock-enabled
  * org.gnome.desktop.screensaver idle-activation-enabled
  * org.gnome.desktop.session idle-delay (10 minutes currently configured in json)
* **Defender for Endpoint on Linux status**
  * MicrosoftDefenderForEndpointOnLinux_Installed
  * MicrosoftDefenderForEndpointOnLinux_RegisteredToOrganization
  * MicrosoftDefenderForEndpointOnLinux_Healthy
  * MicrosoftDefenderForEndpointOnLinux_DefinitionsStatus_up_to_date
  * MicrosoftDefenderForEndpointOnLinux_real_time_protection_enabled

In Non-Compliant situation Intune Company Portal shows clear message which custom compliant check is out of compliance. You can customize messages and url's in .json configuration file.

![Intune_Linux_CustomComplianceCheck_RebootRequired_NotCompliant.png](/assets/img/Intune_Linux_CustomComplianceCheck_RebootRequired_NotCompliant.png)

Go to my [GitHub site](https://github.com/petripaavola/Intune/tree/master/Linux) for the files and more documentation.

I'm happy to hear your feedback for doing more custom checks in this script :)
