# ArchiveMaster Light 1.0.0 — Installation Guide

This document provides step-by-step instructions for downloading, verifying, and installing **ArchiveMaster Light 1.0.0** on 64-bit Windows systems (x64 and ARM64).

---

## Choosing the Correct Architecture

ArchiveMaster Light 1.0.0 provides native installers for both major 64-bit Windows architectures:

- **Windows x64 (`ArchiveMaster Light-1.0.0-Setup-x64.exe`):**  
  Select this for standard Intel (Core, Xeon, Celeron) or AMD (Ryzen, Athlon, EPYC) 64-bit processors. This covers the vast majority of Windows desktop and laptop PCs.

- **Windows ARM64 (`ArchiveMaster Light-1.0.0-Setup-arm64.exe`):**  
  Select this for devices running Windows on ARM processors, such as Qualcomm Snapdragon X Elite, Snapdragon X Plus, Snapdragon 8cx, Microsoft SQ1/SQ2/SQ3 (Surface Pro 9/11 5G), or Windows running under ARM virtual machines.

> **Tip:** If you are unsure which architecture your computer uses, open Windows **Settings** → **System** → **About** and look at **System type** (it will specify either *"64-bit operating system, x64-based processor"* or *"64-bit operating system, ARM-based processor"*).

---

## System Requirements

- **Operating System:** Windows 10 or Windows 11 (64-bit, x64 or ARM64).
- **Available Storage:** Sufficient free space for selected source files and generated archive sets.
- **Destinations:** Configured storage locations or optical disc preparation staging folders with sufficient usable capacity.
- **Hardware/Software:** Optical recording hardware and disc burning software if burning prepared image sets to physical media (CD, DVD, Blu-ray, M-DISC).

---

## Step 1 — Download the Official Installer

Download the setup executable matching your system architecture directly from the GitHub Releases page:

- **Official Release:** [https://github.com/rampoldijr/ArchiveMasterLight-Release/releases/tag/v1.0.0](https://github.com/rampoldijr/ArchiveMasterLight-Release/releases/tag/v1.0.0)
- **Windows x64 Installer:** `ArchiveMaster Light-1.0.0-Setup-x64.exe`
- **Windows ARM64 Installer:** `ArchiveMaster Light-1.0.0-Setup-arm64.exe`

> **Security Note:** Only download installers from the official release page above. Never execute binaries obtained from third-party mirrors or unverified sources.

---

## Step 2 — Verify the SHA-256 Checksum

Before running the installer, verify its cryptographic hash to ensure that the file was downloaded intact and without tampering.

Open PowerShell and execute the command corresponding to your downloaded file:

### For Windows x64:
```powershell
Get-FileHash -Algorithm SHA256 "ArchiveMaster Light-1.0.0-Setup-x64.exe"
```
*Expected hash:*
```text
674d5facc355096db04c6fab8f6237527ca410d7d97a3bd4a3384b2e09d12f62
```

### For Windows ARM64:
```powershell
Get-FileHash -Algorithm SHA256 "ArchiveMaster Light-1.0.0-Setup-arm64.exe"
```
*Expected hash:*
```text
47e0b1c8acd092797095b7c4f8acdcaef9257a25028c13a6f03537a5a75c0315
```

You can also download and check the companion [`SHA256SUMS.txt`](SHA256SUMS.txt) manifest.

---

## Step 3 — Run the Installer

1. Double-click the installer for your architecture.
2. Follow the on-screen setup wizard to choose the installation folder and desktop shortcut preferences.
3. The installer requests administrative privileges to write files to `Program Files` and register the application. After installation, ArchiveMaster Light runs as a standard user process (`asInvoker`).

---

## Step 4 — Handling Windows SmartScreen Warnings

Because these installers are currently **unsigned** (distributed without a commercial Authenticode code-signing certificate), Windows Defender SmartScreen will present a warning on first launch:

> *"Windows protected your PC — Microsoft Defender SmartScreen prevented an unrecognized app from starting."*

To proceed after verifying the SHA-256 checksum:
1. Click **"More info"** (*"Mais informações"*).
2. Click **"Run anyway"** (*"Executar assim mesmo"*).

---

## Step 5 — First-Use Precautions

- ArchiveMaster Light operates as an ephemeral single-session application: it does not maintain an external database and processes files per active project session.
- Pre-build capacity validation will check your selected destination drives and Safety Margins prior to initiating any file operations.
- Maintain independent backups of all critical data before performing bulk file movements or archiving workflows.

---

## Step 6 — Troubleshooting and Support

If you encounter installation or runtime issues on either x64 or ARM64, please submit an issue on the official distribution repository:
https://github.com/rampoldijr/ArchiveMasterLight-Release/issues

Please consult [SUPPORT.md](SUPPORT.md) for reporting guidelines.
