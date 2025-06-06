# My Proxmox (Cyberlab) Setup for Cybersecurity Learning

**Host:** Proxmox VE (Debian)  
**Virtualization:** QEMU/KVM

---

## Network Setup

- `vmbr0` — Main bridge for Proxmox server access  
- `vmbr0.30` — Isolated VLAN bridge for vulnerable machines

I also created **two Bash scripts**:
- **Enable Internet** on the isolated bridge (for updates)
- **Disable Internet** (for testing)

---

## Virtual Machines (VMs)

- **Kali Linux** (Attacker machine, runs on my main Arch system)
- **Kioptrix Level 1** (Target)
- **DVWA** (Planned)
- **Metasploitable 2** (Planned)
- **SOC Stack** (Planned)

---

## Remote Access

- **Tailscale** — Encrypted mesh VPN
- **ACL Rules** — Restricted friend access for lab safety

---

## Additional Notes

I built this lab to **learn cybersecurity** hands-on, focusing on **network segmentation** for safe exploitation. My goal was to avoid infecting my home network while exploring offensive security techniques.

- **Host machine:** HP ProBook 6570b running Debian 12 (Proxmox)
- **Attacker machine:** Lenovo T480 running Arch Linux + Hyprland

Networking took a bit of trial and error, but I wanted it **as safe as possible**. My setup currently includes:
- `vmbr0` (server access)
- `vmbr0.30` (isolated VLAN for vulnerable targets)

I plan to add:
- **DVWA** and **Metasploitable 2** for web and system exploitation practice
- A **home SOC** and **honeypot** for real-world defense simulations

---

This Cyberlab helps me build skills in:
- Offensive and defensive cybersecurity
- Networking
- System administration
