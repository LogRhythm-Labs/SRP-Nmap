# SRP-Nmap
```
LogRhythm Strategic Integrations Team
zack[dot]rowland@logrhythm[dot]com
julian[dot]crowley@logrhythm[dot]com
v1.0 -- July, 2018
```
SmartResponse Plugin/PowerShell Script - Copyright 2018 LogRhythm Inc. - See licensing details below

## [About]

Nmap is a free and open source utility for network discovery and security auditing. This SmartResponse plugin integrates Nmap with LogRhythm SIEM, allowing users to execute Nmap queries "on-demand" via the LogRhythm Web Console, or as automatic remediation actions triggered by a LogRhythm SIEM Alarm. Several commonly used Nmap queries are included in the plugin as pre-defined actions, as well as a "custom" action that can be configured using any of the available Nmap options.

## [Additional Information]

Pre-defined Nmap SmartResponse actions available in this plugin include:
* Intense Scan (Nmap command `nmap -T4 -A -v`)
* Ping Scan (Nmap command `nmap -sn`)
* Quick Scan (Nmap command `nmap -T4 -F`)
* Regular Scan (Nmap command `nmap`)
* Custom Scan (Nmap command `nmap`; any additional flags/options can be specified manually)

Included Nmap Version: nmap-7.70-win32

## [Install and Usage]

This plugin utilizes the Nmap "Command-line" binary package, combined with a PowerShell script as an intermediary between LogRhythm and the Nmap executable(s). The Nmap executables require that the [Microsoft Visual C++ 2013 Redistributable Package](http://www.microsoft.com/download/details.aspx?id=40784) be installed on any host(s) that will execute the plugin; this is the only required prerequisite.

## [License]

PowerShell code © 2018 LogRhythm Inc.   

PowerShell code is Licensed under the MIT License. See LICENSE file in the project root for full license information.

LogRhythm integrated code (SmartResponse and Dashboards) is licensed pursuant to the LogRhythm End User License Agreement located at [https://logrhythm.com/about/logrhythm-terms-and-conditions/](https://logrhythm.com/about/logrhythm-terms-and-conditions/) (“License Agreement”) and by downloading and using this content you agree to the terms and conditions of the License Agreement unless you have a separate signed end user license agreement with LogRhythm in which case that signed agreement shall govern your licensed use of this content. For purposes of the applicable end user license agreement, this content constitutes LogRhythm Software.

The Nmap Security Scanner is © 1996-2018 Insecure.Com LLC ("The NmapProject"). Nmap is also a registered trademark of the Nmap Project. Nmap is free software; you may redistribute and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation; Version 2 ("GPL"), BUT ONLY WITH ALL OF THE CLARIFICATIONS AND EXCEPTIONS DESCRIBED HEREIN¹.

¹Full license available at [https://nmap.org/book/man-legal.html](https://nmap.org/book/man-legal.html)