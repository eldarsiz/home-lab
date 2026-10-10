# Home Lab: OPNsense Firewall and Network Segmentation

A virtual network lab built in VirtualBox to practise firewalling,
VLANs and network security. Built while studying for CompTIA Network+.

## Lab 1: OPNsense firewall (done)

- **Platform:** VirtualBox on Windows
- **VM:** OPNsense 26.7, 2 vCPU, 2-4 GB RAM, 20 GB disk
- **Design:** WAN on NAT (internet side), LAN on an internal
  network (`lan1`)
- **Result:** LAN 192.168.1.1/24, WAN 10.0.2.15/24, internet
  reachable (ping to 8.8.8.8 works)

![Console menu](screenshots/01-opnsense-console.png)
![WAN ping test](screenshots/02-ping-test.png)

### What I learned
- Why OPNsense needs two interfaces (WAN and LAN)
- How internal networks isolate VMs in VirtualBox
- Why snapshots help before changing a firewall

## Roadmap
- [ ] Lab 2: client VM and web interface
- [ ] Lab 3: VLANs and firewall rules
- [ ] Lab 4: VPN and monitoring
