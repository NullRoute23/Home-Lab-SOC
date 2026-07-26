# Home Lab SOC Project

Building a home lab to simulate real-world attacks and defenses using VMware Workstation Pro and Kali Linux. The goal is to gain hands-on experience with offesnive security tools and detection/monitoring workflows.

## Planned Architecture
- **Attacker Box**: Kali Linux (offensive tooling).
- **Target Boxes**: Metasploitable2, and later a Windows/AD environment.
- **Detection/Monitoring Box**: Security Onion or Wazuh (log analysis, alerting).
- **Networking**: Isolated internal/host-only network, no bridging to home network.

## Progress Log

### [07/25/2026] - Environment Setup
- Installed VMware Workstation Pro (26H1)
- Downloaded and imported Kali Linux VM
- Successfully booted Kali Linux inside VMware

## Setup Decisions

**Side-channel mitigations: kept enabled**
This lab intentionally runs exploits and attack tools in one VM alongside other VMs on the same host. Disabling CPU side-channel mitigations for a performance gain would increase the risk of cross-VM information leakage through CPU caches and branch predictions.

## Next Steps
- [ ] Set up isolated internal network in VMware
- [ ] Import and configure Metasploitable2
- [ ] Run first exploit (Kali + Metasploitable)
- [ ] Set up Security Onion for detection/logging
- [ ] Document first attack/document writeup
