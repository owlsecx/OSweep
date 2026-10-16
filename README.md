# 🦉 OSweep

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Linux-0a0c10?style=flat-square"/>
  <img src="https://img.shields.io/badge/Category-OScan-blue?style=flat-square"/>
  <img src="https://img.shields.io/badge/License-MIT-green?style=flat-square"/>
  <img src="https://img.shields.io/badge/Part%20of-OwlSec%20Toolkit-7b5ea7?style=flat-square"/>
  <img src="https://img.shields.io/badge/Version-1.0.0-cyan?style=flat-square"/>
</p>

> **OSweep** — Network Host Discovery & Live Sweep

---

> ⚠️ **AUTHORISED USE ONLY** — Use only on systems you own or have explicit written permission to test. Unauthorised use is illegal.

---

## 📌 Overview

Network host discovery, inventory & live sweep

---

## ✨ Features

- Target parser: CIDR, dash ranges, octet ranges, hostnames, host-list files, exclusions, caps
- Multi-probe engine: TCP connect, ICMP (raw or system ping fallback), ARP cache, ip neigh, arping
- Live-host scoring that fuses all probe signals
- Name resolution: reverse DNS, NetBIOS NBSTAT, mDNS reverse PTR query (all degrade gracefully)
- Embedded compact OUI vendor table
- Light service hint (small port set, not a scan)
- Topology summary: per-subnet density, chatty vs silent hosts, vendor mix
- Watch mode with new/gone/changed host deltas
- Export: TXT / CSV / JSON / Markdown inventory
- Settings persisted to ~/OSweep/config.json

---

## ⚙️ Requirements

- **Linux**
- **No Python installation needed** — runs as a standalone executable

---

## 🚀 Usage

```bash
./OSweep
```

---

## 📦 Part of OwlSec Toolkit

This tool is part of the **OwlSec** suite — a collection of 300+ security and privacy tools.

🔗 [owlsec.org](https://owlsec.org)

---

## ©️ License

MIT License — © Khaled S. Haddad

*Tools are distributed as pre-built executables. Source code is proprietary.*
