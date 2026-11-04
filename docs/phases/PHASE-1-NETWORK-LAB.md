# 🔌 Phase 1 — Network Lab Preparation
![Stage](https://img.shields.io/badge/phase-1_IN_PROGRESS-2563eb?style=flat-square) ![Active](https://img.shields.io/badge/subphase-1.1_PHYSICAL_CONNECTION-f59e0b?style=flat-square)

> [!IMPORTANT]
> **Current active subphase: 1.1 — Physical Connection.** This file is an implementation checklist, not a report of completed configuration.

## 🎯 Phase outcomes

| Subphase | Objective | Expected evidence | Status |
|:---|:---|:---|:---|
| **1.1 · Physical Connection** | Connect Windows laptop and hAP Lite safely, without disturbing home networking | Ethernet link and management access validated | 🔵 In progress |
| **1.2 · Basic Router Configuration** | Implement planned custom Wi-Fi WAN and Ethernet LAN while preserving management access | Validated RouterOS configuration | ⚪ Not started |
| **1.3 · Connectivity Validation** | Test interface state, addressing, gateway, ICMP and Internet reachability | Actual connectivity test results | ⚪ Not started |
| **1.4 · Security and Backup** | Restrict management access; verify firewall and backups | Security checklist and recoverable configuration | ⚪ Not started |

## 🗺️ Planned roles

| Wireless WAN | Ethernet LAN | Virtual monitoring |
|:---|:---|:---|
| `wlan1` as 2.4 GHz WPA2 client of the home network | `bridge-lan` gateway `10.77.10.1/24` | Ubuntu bridged LAN; CHR management on a separate Host-only segment |

The planned addressing details are in [IP-PLAN.md](../IP-PLAN.md), and the network diagram is in [ARCHITECTURE.md](../ARCHITECTURE.md).

## 🛡️ Safety and acceptance gates

| Gate | Requirement |
|:---|:---|
| 🔌 Physical safety | Inspect cabling and link LEDs; do not connect the lab router upstream by Ethernet without an approved design |
| 🔐 Management access | Confirm WinBox access before and after any future changes |
| 💾 Backup | Preserve existing backup copies before a destructive change |
| 🧱 Firewall | Do not remove default protections before replacements are prepared and validated |
| 🧪 Evidence | Use a small number of meaningful, sanitized results; never publish raw backups or credentials |
| 🎓 Mastery | Explain WAN versus LAN, default and connected routes, and recovery procedure |

## 📍 Current next action

Verify the existing cable from Windows Ethernet to a LAN port on the hAP Lite, confirm physical link and WinBox access, and report the result before continuing to subphase 1.2.

**No custom router configuration, Zabbix installation, or CHR deployment has been performed as part of Phase 1 yet.**
