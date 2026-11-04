# 🧮 IP Addressing Plan
![Addressing](https://img.shields.io/badge/IP_plan-PROPOSED-f59e0b?style=flat-square)

> [!NOTE]
> Addresses below are **planned**, not applied. Do not treat these as current device configuration.

## 🌍 WAN and physical LAN

| Device / interface | Address | Assignment | Role |
|:---|:---|:---|:---|
| Home Wi-Fi / hAP Lite `wlan1` | Upstream network | DHCP client | Wireless WAN |
| hAP Lite `bridge-lan` | `10.77.10.1/24` | Static | LAN gateway |
| Windows Ethernet | `10.77.10.10/24` | Planned static | Host administration |
| Ubuntu Zabbix bridged | `10.77.10.20/24` | Planned static | Monitoring and Internet via gateway `.1` |
| MikroTik DHCP pool | `10.77.10.100–200` | Dynamic | Client allocations |

## 🧪 Virtual management and GNS3

| Device / interface | Address | Default gateway |
|:---|:---|:---|
| Windows VirtualBox Host-only | `192.168.56.1/24` candidate | None |
| Ubuntu Zabbix Host-only | `192.168.56.20/24` | None |
| CHR1 `ether1` management | `192.168.56.30/24` | None on management segment |
| CHR1 `ether2` virtual LAN | `10.77.20.1/24` | Routing to be designed |
| Optional CHR2/Linux host | TBD | Subject to Phase 4 design |

## 🔎 Before applying addresses

| Check | Reason |
|:---|:---|
| 🔍 Inspect inactive VPN/VM subnets | Avoid address conflicts |
| 🔧 Fix Host-only adapter mismatch | Host previously displayed a `169.254.x.x` address |
| 🔒 Separate LAN and upstream DHCP | Prevent overlap with home network |
| 📡 Confirm static IPs unused | Pool exclusion alone does not guarantee no manually assigned duplicate |
| 🔁 Test both directions | Routing, return path and firewall must agree |
