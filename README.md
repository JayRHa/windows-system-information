<!-- jr-brand:start -->
<p align="center">
  <a href="https://jannikreinhard.com/">
    <img src="https://raw.githubusercontent.com/JayRHa/.github/main/assets/readme/brand-header.png" alt="Jannik Reinhard — I help enterprises ship secure AI agents" width="100%">
  </a>
</p>
<p align="center">
  <a href="https://jannikreinhard.com/">Website</a> ·
  <a href="https://www.linkedin.com/in/jannik-r/">LinkedIn</a> ·
  <a href="https://x.com/jannik_reinhard">X</a> ·
  <a href="https://www.youtube.com/@jannikreinhard">YouTube</a>
</p>
<!-- jr-brand:end -->

# Windows system information

**Type:** Tool or application · **Status:** Community project

## Overview

PowerShell-based system information gathering tool for Windows endpoint diagnostics.

The System Information Tool shows important Windows device details in one place. It also provides practical actions for troubleshooting Microsoft Intune and the Intune Management Extension. You can add your own scripts for self-service support.

![System Information Tool](assets/toolView.png)

## Quickstart

Get the source locally:

```bash
git clone https://github.com/JayRHa/windows-system-information.git
cd windows-system-information
```

Entry points: [`scripts`](scripts).

## Installation

```powershell
git clone https://github.com/JayRHa/windows-system-information.git
cd windows-system-information
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

[Articles and guides](https://jannikreinhard.com/) · [Repository index](https://github.com/JayRHa/.github/blob/main/REPOSITORIES.md)
<!-- jr-brand-footer:end -->
