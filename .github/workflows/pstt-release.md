<!-- ===========================================================================
     RELEASE PAGE TEMPLATE FOR PS.Tweak.Tools
     ---------------------------------------------------------------------------
     This file is used by the GitHub Actions workflow pstt-release.yml
     to build the release body dynamically.

     The following placeholders are replaced at runtime by the workflow:
       {{LOGO_URL}}          -> Raw URL to the project logo image
       {{ZIP_FILENAME}}      -> Full ZIP filename (e.g. PS.Tweak.Tools-1.00.00-Release.zip)
       {{DOWNLOAD_URL}}      -> Full direct download URL for the ZIP file
       {{REPO_URL}}          -> GitHub repository base URL
       {{VERSION}}           -> Version number (e.g. 1.00.00)
       {{UNOFFICIAL_BANNER}} -> Empty string OR unofficial warning banner
       {{RELEASE_NOTES}}     -> Additional release notes or default placeholder
       {{SYNC_STATUS}}       -> Cross-repo sync result line (set by Step 7)
=========================================================================== -->

{{UNOFFICIAL_BANNER}}
<p align="center">
  <img src="{{LOGO_URL}}" alt="PS.Tweak.Tools Logo" width="480" />
</p>

## 🖥️ **File Download:**

**📦 [`{{ZIP_FILENAME}}`]({{DOWNLOAD_URL}})**
<br>

## ℹ️ System Requirements:
- Windows 10 / Windows 11
- PowerShell 5.1 or higher
- No administrator privileges required for standard usage
<br>

## 🪛 Installation / Usage:

### 📂 Option A — Direct Import *(local, no installation required)*:
1. Download the ZIP archive from the link above.
2. Extract the archive to a location of your choice.
3. Open PowerShell and navigate to the extracted folder.
4. Import the module directly for the current session:
   ```powershell
   Import-Module .\PS.Tweak.Tools\PS.Tweak.Tools.psm1
   ```
5. Refer to the included `README.md` for detailed usage instructions.

### 🌍 Option B — Global Module Installation *(persistent, user-wide)*:
1. Download and extract the ZIP archive.
2. Determine your personal PowerShell module directory:
   ```powershell
   $env:PSModulePath -split ';'
   ```
3. Inside that `Modules` directory, create a new subfolder named exactly `PS.Tweak.Tools`.
4. Copy all extracted files into that new subfolder.
5. The module is now permanently available in every PowerShell session:
   ```powershell
   Import-Module PS.Tweak.Tools
   ```
6. To verify the installation:
   ```powershell
   Get-Module -ListAvailable PS.Tweak.Tools
   ```
<br>

## 🔄 Cross-Repo Synchronization:

{{SYNC_STATUS}}
<br>

## 📜 License/Copyright:

**PS.Tweak.Tools** is licensed for **private, non-commercial use only**.

- ❌ Commercial use of any kind is strictly prohibited.
- ❌ Editing, modifying, or manipulating this software in any form or manner without the explicit written consent of the developer is not permitted.
- ⚠️ Use of PS.Tweak.Tools is entirely at the user's own risk. No liability is assumed for any damage to hardware and/or software that may occur.
- ⚠️ Any consequences arising from the use of PS.Tweak.Tools are solely the responsibility of the user.

> **PS.Tweak.Tools™** · © 2026 by WinTwin-Fusion · All rights reserved.
<br>

## 🛟 Security Advise:

> ⚠️ **Important:** The official and only trusted source for PS.Tweak.Tools is:
>
> 🔗 **[https://github.com/WinTwin-Fusion/PS.Tweak.Tools](https://github.com/WinTwin-Fusion/PS.Tweak.Tools)**
>
> It is **strongly recommended** to download PS.Tweak.Tools **exclusively** from this official source. Do not use copies from unknown or untrusted third-party sources, as these may have been tampered with or contain malicious code.
<br>

## 📝 Additional Notes:

{{RELEASE_NOTES}}
<br>

---
Part of the WinTwin.Fusion Framework · [WinTwin-Fusion Organization](https://github.com/WinTwin-Fusion)
