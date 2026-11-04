# 📝 Design Decisions
![Decision log](https://img.shields.io/badge/record-Phase_0-2563eb?style=flat-square)

| ID | Decision | Reason | State |
|:---|:---|:---|:---|
| D-001 | Public-first documentation | Publish useful evidence with less unnecessary overhead | ✅ Agreed |
| D-002 | Exclude raw `.backup` and `.rsc` exports | Raw configurations may contain sensitive data | ✅ Agreed |
| D-003 | Build custom hAP Lite WAN/LAN configuration in Phase 1 | Understand and validate every rule | ✅ Planned implementation |
| D-004 | Use 2.4 GHz home Wi-Fi as hAP Lite WAN | Provide Ethernet LAN from wireless upstream | 🟡 Proposed; untested |
| D-005 | Ubuntu bridged LAN + Host-only CHR management | Monitoring on two directly connected segments | 🟡 Proposed; untested |
| D-006 | Ubuntu: 2 vCPU / 3 GiB / 25 GiB dynamic; CHR1: 1 vCPU / 256 MiB | Restrained resource allocation | 🟡 Estimate |
| D-007 | Evidence screenshots only when they add value | Keep documentation concise and reviewable | ✅ Agreed |
| D-008 | Close Phase 0 based on knowledge reassessment and review of the submitted local architecture/IP-plan documentation; start Phase 1.1 | Keep implementation within the approved roadmap | ✅ Accepted for project progression; remote repository verification remains separate |

> [!IMPORTANT]
> No scope change is recorded. Revisit untested choices only when validation evidence justifies it.
