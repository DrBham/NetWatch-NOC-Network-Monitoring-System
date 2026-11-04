# Phase 0 — Assessment Summary (Public)

**This is a sanitized summary, not a configuration dump or proof of a deployed NOC.**

## 0.1 Environment Inventory

Host: Windows 11 Home, 12 GB RAM, Intel Core i5-12450HX; VirtualBox 7.2.14 and GNS3 2.2.61 present at assessment. Windows RAM available at one measurement ~4.4 GB. Storage headroom was limited (system partition especially). Ubuntu Server ISO not yet downloaded. **Outcome:** inventory completed; deployment capacity risk open.

## 0.2 Physical MikroTik Assessment

Physical MikroTik hAP Lite assessed with RouterOS 7.20.7; default interface, bridge, IP/DHCP, firewall and NAT reviewed. User reported downloads of local binary backup and text export. **Outcome:** initial baseline inventory completed; original backup/export excluded from public repository. Device identifiers, credentials and raw WinBox views are intentionally omitted.

## 0.3 Architecture and Network Planning

Proposed custom routed Wi-Fi WAN (2.4 GHz WPA2) → MikroTik Ethernet LAN (`10.77.10.0/24`), Ubuntu Zabbix bridged LAN + host-only CHR management (`192.168.56.0/24`), CHR virtual LAN (`10.77.20.0/24`). **Outcome:** initial plan formulated. Integration, addressing conflicts, NAT, routing and connectivity remain to be tested during relevant implementation phases.

## 0.4 Repository & Project Baseline

**IN PROGRESS** until the repository exists, files have been reviewed and committed/pushed, and Phase 0 acceptance/assessment completed. LinkedIn project is separate and optional for this milestone.

## Security and evidence policy

Raw device backups, device-unique identifiers, Wi-Fi passwords, SNMP community strings, keys, and non-sanitized exports are intentionally not included. Later phases will publish *tested* clean configuration templates, diagrams, and verification results.
