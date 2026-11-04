# Project Scope — Baseline v1.0

## In scope

- One Ubuntu Server monitoring VM with Zabbix server, database and web frontend.
- One physical MikroTik hAP Lite router.
- Up to two MikroTik CHR virtual routers.
- Up to one additional monitored Linux VM if laptop resources permit.
- ICMP, SNMP, availability, uptime, supported CPU/RAM/interface metrics.
- Dashboard, triggers, alerts, controlled outages and incident response.
- GitHub documentation, reproducible sanitized configurations and final demonstration.

## Out of scope

Kubernetes, HA cluster, multi-cloud, production-scale SD-WAN/BGP/OSPF, AI/ML anomaly detection, complete SIEM/SOC, Prometheus/Grafana addition, LibreNMS, custom full-stack dashboard, automated self-healing, new paid hardware/cloud/services.

Python automation is not a core-project requirement.

## Change control

Record problem evidence, smallest fix, impact, and classification (Bug Fix / Implementation Adjustment / Scope Change). Scope changes need explicit approval and a recorded decision.

## Publishing policy

Publish only safe, necessary and reproducible project content. Never push raw binary backups, unreviewed `.rsc` exports, credentials, private keys, secrets, unredacted identification data, `.vdi/.vmdk` images, or personal data. Keep only relevant sanitized evidence.
