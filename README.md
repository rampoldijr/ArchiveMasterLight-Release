# ArchiveMaster Light

**Prepare and organize files for reliable, structured long-term optical storage.**

ArchiveMaster Light is a Windows desktop application designed to prepare structured archive sets for optical storage media, including CD, DVD, Blu-ray, and M-DISC workflows.

**Free to use · Windows x64 & Windows ARM64 · Version 1.0.0 (First Public Release)**

---

## About the Project & Developer Note

Version 1.0.0 represents the **first publicly available software release** by the developer. This project was developed as a focused utility to solve practical optical storage staging needs and as part of an active journey of learning and improvement in software engineering.

Constructive feedback, reproducible bug reports, and usability suggestions are warmly welcomed to help improve future versions.

---

## Download & Installation

The official 64-bit Windows installers are published exclusively on the [Releases](https://github.com/rampoldijr/ArchiveMasterLight-Release/releases) page of this repository.

### Available Installers:

| Target System | Processor Architecture | Installer Filename | SHA-256 Checksum |
| :--- | :--- | :--- | :--- |
| **Windows x64** | Intel / AMD (Standard PCs) | `ArchiveMaster Light-1.0.0-Setup-x64.exe` | `674d5facc355096db04c6fab8f6237527ca410d7d97a3bd4a3384b2e09d12f62` |
| **Windows ARM64** | Snapdragon X / Surface ARM | `ArchiveMaster Light-1.0.0-Setup-arm64.exe` | `47e0b1c8acd092797095b7c4f8acdcaef9257a25028c13a6f03537a5a75c0315` |

- **Official Release Page:** [ArchiveMaster Light 1.0.0 Release](https://github.com/rampoldijr/ArchiveMasterLight-Release/releases/tag/v1.0.0)
- **Verification Manifest:** [`SHA256SUMS.txt`](SHA256SUMS.txt)

For detailed verification and installation instructions, see [INSTALLATION.md](INSTALLATION.md).

> **Important Security Notice (Unsigned Executable):**  
> The installer executables are currently unsigned (distributed without an Authenticode certificate). When launching the installer for the first time, Windows Defender SmartScreen may display an informational warning (*"Windows protected your PC"*). Verify the SHA-256 hash using `Get-FileHash` before proceeding by clicking **"More info"** and then **"Run anyway"**.

---

## Features & Capabilities

- **Optical Archive Preparation:** Organize files into structured disc layouts according to optical media capacities (CD 700 MB, DVD 4.7 GB / 8.5 GB, Blu-ray 25 GB / 50 GB / 100 GB, M-DISC, or custom sizes).
- **Pre-Build Capacity Gate:** Verifies usable space across configured destinations and user-defined Safety Margins before initiating any write operations, preventing builds from halting due to insufficient capacity.
- **Multiple Destination Routing:** Distribute discs across multiple storage folders or staging drives automatically.
- **Single-Session Ephemeral Workflow:** Operates with an in-memory session model without background database tracking, cleanly clearing temporary `.part` files on cancellation.
- **Build Progress & Responsive Controls:** Monitor real-time file copying progress with sub-100ms cancellation response and in-memory continuation.
- **Multilingual User Interface:** Complete localization in 5 languages: English, Portuguese, Spanish, German, and French.

*Note:* Archive creation requires user judgement regarding destination choices and disc organization. Users should always inspect generated archive output and maintain independent backups of critical data.

---

## Free Use and Licensing Terms

ArchiveMaster Light is provided free of charge under its proprietary software licence.

**Free of charge does not mean open source.** The application's source code is maintained in a separate private repository and is not distributed in this repository. No general permission is granted to decompile, reverse engineer, modify, sublicense, or redistribute the software without express authorization.

Please consult the [LICENSE](LICENSE) file for the full terms and conditions.

---

## Support the Developer (Optional)

ArchiveMaster Light is completely free to use. If you find the software valuable and would like to support the developer's ongoing learning, application maintenance, documentation improvements, and future iterations, voluntary contributions are gratefully accepted:

👉 **[Donate via PayPal](https://www.paypal.com/donate/?hosted_button_id=PQQ56UXLVMT5A)**

*Official PayPal link:* `https://www.paypal.com/donate/?hosted_button_id=PQQ56UXLVMT5A`

*Disclaimer: Voluntary donations are purely optional and do not include or imply commercial support warranties, guaranteed response times, or promised future features.*

---

## Support & Reporting Issues

If you experience bugs, installation problems, or have feature ideas, please submit an issue on GitHub:
👉 [Open an Issue](https://github.com/rampoldijr/ArchiveMasterLight-Release/issues)

See [SUPPORT.md](SUPPORT.md) for bug report guidelines.

---

© 2026 ArchiveMaster. All rights reserved.
