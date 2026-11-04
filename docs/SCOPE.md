# 🎯 Project Scope
![Scope](https://img.shields.io/badge/scope-FROZEN_v1.0-16a34a?style=flat-square)

## ✅ In scope / ⛔ Out of scope

| ✅ Included | ⛔ Excluded |
|:---|:---|
| Ubuntu Server monitoring VM and Zabbix (server, database, frontend) | Kubernetes or high-availability cluster |
| Physical MikroTik hAP Lite | Multi-cloud or paid cloud infrastructure |
| Up to two virtual MikroTik CHR routers | Enterprise SD-WAN, production-scale BGP/OSPF |
| One optional monitored Linux VM if resources allow | Full SIEM/SOC or AI/ML anomaly detection |
| ICMP, SNMP, metrics supported by each device | Prometheus/Grafana stack, LibreNMS |
| Dashboard, triggers, notifications, controlled outages | Custom full-stack web dashboard |
| Incident investigation, recovery testing and reproducible documentation | Automated self-healing or new paid hardware |

**Python automation:** Optional future work; not required for the core project.

## 🔄 Change control

| Step | Action |
|:---|:---|
| 🔍 Evidence | Describe the issue and observed evidence |
| 🛠️ Minimal fix | Choose the smallest correction that preserves scope |
| 📐 Impact | Document effect on milestones and deliverables |
| 🗳️ Decision | Obtain approval for any scope change |
| 📝 Record | Update decisions or changelog when relevant |

## 🔐 Publishing rules

> [!CAUTION]
> Never publish binary device backups, unreviewed RouterOS exports, passwords, Wi-Fi credentials, SNMP secrets, SSH private keys, API tokens, sensitive device identifiers or VM disk images. Examples must be sanitized and reproducible; evidence must reflect actual tests.
