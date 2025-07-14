# kali-vmware-network-audit
# Kali VMware Network Audit Script

A Bash script to collect network, virtualization, and DHCP history details from Kali Linux running inside VMware.

## ✅ Features

- Detects virtualization platform (e.g. VMware)
- Shows hostname, machine ID, and IP/MAC addresses
- Filters `NetworkManager` DHCP logs using custom date/time input
- Saves output to `vm_net_report.txt`

## 🧪 Use Cases

- Investigate IP changes during pentesting labs
- Audit VMware networking (Bridged/NAT/Host-only)
- Troubleshoot or trace DHCP lease behavior
- Capture and archive daily networking snapshots

## ▶️ Usage

```bash
# Basic (defaults to yesterday → now)
sudo ./vm_info.sh

# Specific date
sudo ./vm_info.sh "2025-07-10" "2025-07-10 23:59"

# Last 2 hours
sudo ./vm_info.sh "2 hours ago" "now"
