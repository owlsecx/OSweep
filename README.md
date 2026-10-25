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


OSweep is a network host-discovery, inventory and watch toolkit — not a port scanner — that answers which hosts are alive, what they are called, who made them and what has changed since the last sweep. It fuses TCP connect, ICMP, ARP, ip-neigh and arping probes with reverse DNS, NetBIOS and mDNS name resolution and an embedded OUI vendor table. A watch mode reports new/gone/changed deltas, and inventories export to TXT, CSV, JSON or Markdown.

---

## ✨ Features


- Flexible targets: CIDR, dash/octet ranges, hostnames, @host-list files, exclusions and caps
- Multi-probe engine (TCP connect, ICMP, ARP cache, ip neigh, arping) with a fused live-host score
- Name resolution via reverse DNS, NetBIOS NBSTAT and mDNS reverse PTR, all degrading gracefully
- Embedded OUI vendor table plus an optional light service hint (not a full scan)
- Topology summary (per-subnet density, chatty vs silent hosts, vendor mix) and a watch mode with deltas
- Export TXT/CSV/JSON/Markdown or live-IPs-only, with clipboard copy and persisted settings

---

## ⚙️ Requirements

- **Linux**
- **No Python installation needed** — runs as a standalone executable

---

## 🚀 Usage


```bash
./OSweep --local --topology
./OSweep -n 192.168.1.0/24 --hint --json -o hosts.json
./OSweep -n 10.0.0.0/24 --watch 60 --rounds 10
./OSweep --vendor 00:1a:2b:3c:4d:5e
./OSweep --help
```

---

## 📦 Part of OwlSec Toolkit

This tool is part of the **OwlSec** suite — a collection of 300+ security and privacy tools.

🔗 [owlsec.org](https://owlsec.org)

---

## ©️ License

MIT License — © Khaled S. Haddad

*Tools are distributed as pre-built executables. Source code is proprietary.*
