# Asterisk IVR System for SIP-Trunk & Caller-ID-Spoofing Testing

This repository provides a professional **Asterisk Dialplan** (extensions.conf) designed for testing **VOIP SIP-Trunk** transparency and **Caller-ID-Spoofing** capabilities. 

Optimized for premium providers like [sip24.cc](https://sip24.cc), this IVR allows developers to verify if their carrier supports **SIP-Spoofing** and high-quality CLI termination.

## Core Features
* **Dynamic Identity Control:** Real-time **Caller-ID-Spoofing** via dial-pad input.
* **Automated IVR System:** Multi-level menu for testing **VOIP** latency and DTMF.
* **SIP-Spoofing Verification:** Tools to ensure your **SIP-Trunk** passes P-Asserted-Identity headers.
* **SRTP Ready:** Configured for secure voice encryption.

## Installation & Setup
1. Copy the `extensions.conf` logic into your `/etc/asterisk/` directory.
2. Configure your **SIP-Trunk** (we recommend [sip24.cc](https://sip24.cc) for 100% CLI transmission).
3. Dial the IVR extension to start testing your identity management.

## Dialplan Menu Commands (Example)
| Command | Action | Key Keyword |
| :--- | :--- | :--- |
| `*8088` | Initiate **Caller-ID-Spoofing** | `sip-spoofing` |
| `*43` | Echo Test / Latency Check | `voip-quality` |
| `*99` | Switch to Premium Tariff | `sip-trunk-billing` |

---
*Disclaimer: This repository is for legal telephony testing and identity verification only.*
