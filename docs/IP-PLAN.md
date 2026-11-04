# IP Addressing Plan — Proposed, Not Applied

All IPs below describe the **future lab design**, not a verified live configuration.

| Segment | Device/interface | Planned address | Gateway / notes |
|---|---|---|---|
| Upstream home Wi-Fi | MikroTik `wlan1` WAN | DHCP from upstream | Internet / NAT, no secrets committed |
| NetWatch LAN `10.77.10.0/24` | hAP Lite `bridge-lan` | `10.77.10.1/24` | LAN router |
| NetWatch LAN | Windows Ethernet | `10.77.10.10/24` | Gateway `10.77.10.1` if using router for internet |
| NetWatch LAN | Ubuntu Zabbix bridged NIC | `10.77.10.20/24` | Gateway `10.77.10.1` |
| NetWatch LAN | MikroTik DHCP pool | `10.77.10.100–10.77.10.200` | Excludes planned static assignments |
| Host-only `192.168.56.0/24` | Windows VirtualBox adapter | `192.168.56.1/24` candidate | No default gateway |
| Host-only | Ubuntu Zabbix NIC | `192.168.56.20/24` | No default gateway |
| Host-only | CHR1 `ether1` | `192.168.56.30/24` | Management, candidate |
| GNS3 virtual `10.77.20.0/24` | CHR1 `ether2` | `10.77.20.1/24` | Virtual lab network |
| Future optional CHR2/Linux host | TBD | TBD | Subject to resource/route validation |

## Outstanding validation

- Confirm planned subnets do not conflict with currently inactive VPN/VM networks.
- Confirm LAN network is isolated from upstream and DHCP exists only on intended LAN.
- Inspect VirtualBox host-only DHCP range and change plan before assigning fixed addresses; no assumptions about automatic IP or gateway.
- Verify proposed static IPs unused at deployment.
- Test host/VM/CHR reachability and routing in both directions.
