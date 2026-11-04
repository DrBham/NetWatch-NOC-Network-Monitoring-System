# Progress Log

```yaml
project: NetWatch NOC
baseline: v1.0
current_phase: 0
current_subphase: '0.4'
status: IN_PROGRESS
completed_subphases:
  - '0.1 Environment Inventory (assessment completed)'
  - '0.2 Physical MikroTik Assessment (assessment completed)'
  - '0.3 Architecture & Network Planning (planning completed)'
pending_tasks:
  - 'Review and publish Phase 0 baseline repository'
  - 'Security-review staged files before first push'
  - 'Confirm GitHub and LinkedIn entries exist'
  - 'Run Phase 0 formal assessment before closure'
verified_configuration:
  - 'No new NetWatch custom router configuration deployed'
  - 'Physical router default baseline was assessed; current live state not revalidated'
decisions:
  - 'Public-first documentation, tested sanitized configs later'
  - 'Plan WLAN WAN and Ethernet LAN on physical MikroTik'
  - 'Plan Zabbix bridged LAN plus host-only CHR management'
open_issues:
  - 'RAM and disk headroom limited'
  - 'VirtualBox host-only IPv4 mismatch pending correction'
  - 'Wi-Fi WAN and bridged VM connectivity untested'
  - 'Route and return-path for lab subnets TBD'
assessment_status: 'Phase 0 final assessment NOT_STARTED'
last_commit: null
next_action: 'Create GitHub repository, review files, commit, push, then portfolio entry'
```

## Evidence summary

- Phase 0.1: CPU, RAM, storage, host OS, VirtualBox/GNS3 versions inventoried. Ubuntu Server ISO not yet available.
- Phase 0.2: hAP Lite RouterOS/hardware/interface/DHCP/firewall/NAT reviewed. User reported local backup and export downloads. Raw backups are private and not included here.
- Phase 0.3: Proposed topology, routing segmentation, resource plan and security constraints discussed. No configuration changes are claimed for the custom plan.

*Update this log after actual actions. A documentation file existing locally is not proof it has been pushed to GitHub.*
