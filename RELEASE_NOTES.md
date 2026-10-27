# ArchiveMaster Light 1.0.0 — Release Notes

**Initial Public Release**

ArchiveMaster Light 1.0.0 is the first public release of ArchiveMaster Light, a dedicated Windows desktop application designed to organize files into structured archive sets for long-term optical storage media (CD, DVD, Blu-ray, and M-DISC workflows).

---

## Key Highlights

- **Ephemeral Single-Session Engine:** Operates without a persistent database or background tracking; state is kept in memory during the active session with automatic temporary file cleanup.
- **250 GB Source Quota:** Tailored for optical media projects up to 250 GB with decimal unit formatting and real-time quota indicator.
- **Pre-Build Capacity Gate:** Evaluates configured destinations, Safety Margins, and disc bin-packing feasibility prior to starting a build to prevent mid-operation failures.
- **Multi-Destination Distribution:** Distributes discs across configured destination paths automatically when individual drives or locations reach capacity limits.
- **Responsive Execution Controls:** Reliable pause, resume, and instant sub-100ms cancellation with immediate deterministic cleanup of in-flight `.part` files.
- **Multilingual Support:** Fully localized user interface and in-app documentation across 5 languages: English, Portuguese, Spanish, German, and French.

---

## Distribution & Verification

- **Platform:** Windows 10 / 11 (64-bit x64)
- **Installer File:** `ArchiveMaster Light-1.0.0-Setup-x64.exe`
- **File Size:** `98,948,415 bytes` (~94.36 MB)
- **SHA-256 Checksum:** `674d5facc355096db04c6fab8f6237527ca410d7d97a3bd4a3384b2e09d12f62`
- **Verification Manifest:** [`SHA256SUMS.txt`](SHA256SUMS.txt)

---

## Important Installation & Security Notice

- **Unsigned Executable:** The installer is currently unsigned (distributed without an Authenticode certificate). Windows Defender SmartScreen will display an informational warning upon first launch.
- **Verification:** Always verify that the SHA-256 hash matches the published checksum before proceeding via *"More info"* → *"Run anyway"*.
- **Licence:** ArchiveMaster Light is freeware provided under a proprietary licence. It is free to use but **not open source**. Source code is maintained separately in a private repository.

---

## Feedback & Voluntary Support

- **Bug Reports & Feedback:** Please open an issue at [https://github.com/rampoldijr/ArchiveMasterLight-Release/issues](https://github.com/rampoldijr/ArchiveMasterLight-Release/issues).
- **Voluntary Developer Support:** If you wish to support continued development, you may contribute via [PayPal](https://www.paypal.com/donate/?hosted_button_id=PQQ56UXLVMT5A).
