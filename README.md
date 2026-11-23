# 🦉 OBLEScan

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Linux-0a0c10?style=flat-square"/>
  <img src="https://img.shields.io/badge/Category-Security-blue?style=flat-square"/>
  <img src="https://img.shields.io/badge/License-Proprietary-orange?style=flat-square"/>
  <img src="https://img.shields.io/badge/Part%20of-OwlSec%20Toolkit-7b5ea7?style=flat-square"/>
  <img src="https://img.shields.io/badge/Version-1.0-cyan?style=flat-square"/>
</p>

> **OBLEScan** — part of the OwlSec Toolkit.

---

> ⚠️ **AUTHORISED USE ONLY** — Use only on systems you own or have explicit written permission to test. Unauthorised use is illegal.

---

## 📌 Overview

OBLEScan analyzes Bluetooth LE captures (pcap/pcapng of HCI or advertising frames) you have already collected. It lists every advertising device, decodes its advertising data, company ID and service UUIDs, and classifies the device type. It flags privacy and tracking exposure such as static addresses. It reads captures only and does not scan, connect to or transmit on any radio.

---

## ✨ Features

- BLE advertisement parser: AD structures, company IDs, 16-bit service UUIDs, address type and Apple subtypes
- Device enumeration and classification
- Privacy and tracking exposure flags
- Offline synthetic BLE capture generator (no radio)
- Findings graded A+ to F with MITRE ATT&CK mapping
- Reports in TXT / JSON / Markdown / CSV / SARIF; exits with code 3 on CRITICAL/HIGH findings

---

## ⚙️ Requirements

- **Linux**
- **No Python installation needed** — runs as a standalone executable

---

## 🚀 Usage

```bash
./OBLEScan                                   # interactive menu
./OBLEScan --analyze ble_capture.pcapng
./OBLEScan --generate --out synth.pcap
./OBLEScan --demo
```

Run `./OBLEScan --help` for the full list of options.

---

## 📦 Part of OwlSec Toolkit

This tool is part of the **OwlSec** suite — a collection of 275+ security and privacy tools.

🔗 [owlsec.org](https://owlsec.org)

---

## ©️ License

Proprietary — © 2026 Owlsec LLC. All rights reserved.

*Tools are distributed as pre-built executables. Source code is proprietary.*
