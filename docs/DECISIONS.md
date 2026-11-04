# Architecture & Documentation Decisions

| ID | Decision | Rationale / constraint | Status |
|---|---|---|---|
| D-001 | Public-first, reproducible documentation | Save user time; publish only safe technical evidence | Agreed |
| D-002 | Keep raw `.backup` and `.rsc` exports outside Git | Sensitive configuration may be present | Agreed |
| D-003 | Plan custom hAP Lite LAN/WAN configuration rather than relying permanently on default | Learning goal; implement only with backup, hardening and testing | Agreed for Phase 1 |
| D-004 | Upstream Wi-Fi via hAP Lite `wlan1` station; Ethernet LAN | Requested wired connectivity from Wi-Fi WAN | Proposed, untested |
| D-005 | Zabbix Ubuntu bridged LAN + host-only for CHR management | Single internet default gateway, direct CHR management monitoring | Proposed, untested |
| D-006 | Start with Ubuntu 2 vCPU / 3 GiB / 25 GiB dynamic disk, CHR1 1 vCPU / 256 MiB | Fit within host constraints, measure usage before expansion | Resource estimate |
| D-007 | Screenshots only when valuable; no Phase 0 screenshots mandatory | Avoid redundant evidence collection | Agreed |

No scope expansion was authorized. Revisit any design only with validation evidence and change record.
