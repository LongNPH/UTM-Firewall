# UTM Firewall with OPNsense

This repository contains the design, implementation notes, and test plans for an academic Unified Threat Management (UTM) firewall project based on OPNsense.

## Project objectives

- Deploy OPNsense as a virtualized security gateway.
- Control traffic between an external WAN and an isolated internal LAN.
- Demonstrate firewalling, NAT, DHCP, logging, IDS/IPS, VPN, and web-filtering capabilities.
- Record repeatable test procedures and evidence for the final evaluation.

## Planned lab systems

| System | Role | Minimum allocation |
|---|---|---|
| OPNsense | UTM firewall and default gateway | 2 vCPU, 3–4 GB RAM, 2 network adapters |
| Ubuntu | LAN test client | 2 vCPU, 2 GB RAM |
| Windows | LAN test client | 2 vCPU, 4 GB RAM |

The OPNsense WAN adapter connects to VMware NAT and receives its address by DHCP. Its LAN adapter connects to an isolated virtual network using `192.168.10.1/24`.

## Documentation

- [Week 2: Network Design and Firewall Policy Test Plan](docs/week-2-network-design.md)

## Project status

Week 2 defines the intended topology, addressing, traffic flows, and expected firewall behavior. Live configuration, execution evidence, and measured results will be added during the implementation and testing phases.
