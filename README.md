<!-- jr-brand:start -->
<div align="center">
  <a href="https://jannikreinhard.com/">
    <img src="https://raw.githubusercontent.com/JayRHa/.github/main/assets/readme/brand-header.png" alt="Jannik Reinhard — Driving AI with passion" width="100%">
  </a>
  <h1>System Information Tool</h1>
  <p><strong>PowerShell-based system information gathering tool for Windows endpoint diagnostics.</strong></p>
  <p>
  <a href="https://jannikreinhard.com/"><img src="https://img.shields.io/badge/Website-146CDD?style=flat-square&amp;logo=wordpress&amp;logoColor=white" alt="Website"></a>
  <a href="https://github.com/JayRHa"><img src="https://img.shields.io/badge/GitHub-081427?style=flat-square&amp;logo=github&amp;logoColor=white" alt="GitHub"></a>
  <a href="https://www.linkedin.com/in/jannik-r/"><img src="https://img.shields.io/badge/LinkedIn-0795FF?style=flat-square&amp;logo=linkedin&amp;logoColor=white" alt="LinkedIn"></a>
  <a href="https://x.com/jannik_reinhard"><img src="https://img.shields.io/badge/X-081427?style=flat-square&amp;logo=x&amp;logoColor=white" alt="X"></a>
  <a href="https://www.youtube.com/@jannikreinhard"><img src="https://img.shields.io/badge/YouTube-146CDD?style=flat-square&amp;logo=youtube&amp;logoColor=white" alt="YouTube"></a>
  </p>
  <p><sub>Driving AI with passion · Microsoft Foundry · Intune · Azure</sub></p>
</div>
<!-- jr-brand:end -->

## Overview

The System Information Tool shows important Windows device details in one place. It also provides practical actions for troubleshooting Microsoft Intune and the Intune Management Extension. You can add your own scripts for self-service support.

![System Information Tool](assets/toolView.png)

## Installation

```powershell
git clone https://github.com/JayRHa/SystemInformationTool.git
cd SystemInformationTool
Get-ChildItem -Recurse *.dll | Unblock-File
.\Install-SystemInformationTool.ps1
```

The installation wrapper creates the Start menu entry and prepares the bundled libraries.

## Start the Tool

```powershell
.\Start-SystemInformationTool.ps1
```

## Features

### Information View

Review the hostname, IP addresses, serial number, memory and other device attributes.

### Microsoft Intune and Support Actions

Run common troubleshooting actions for Microsoft Intune and the Intune Management Extension.

![Microsoft Intune actions](assets/intune.png)

### Custom Self-Service Actions

Place a PowerShell script in the `scripts/` folder and register its display name and file name in `_actions.json`.

![Custom support actions](assets/support.png)

## License

This project is available under the terms in [LICENSE](LICENSE).

<!-- jr-brand-footer:start -->

---

<div align="center">
  <p><sub>Built and maintained by <a href="https://jannikreinhard.com/">Jannik Reinhard</a> · Microsoft MVP for Security and AI Platform.</sub></p>
  <p><a href="https://www.buymeacoffee.com/jannikreinf">Support the open-source work</a></p>
  <p><strong>Stay healthy, Cheers Jannik</strong></p>
</div>

<!-- jr-brand-footer:end -->
