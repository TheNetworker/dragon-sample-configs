---
title: 'Dragon sample configs: synthetic Cisco NX-OS configurations for the Train Your Dragon demo'
---

# What these are

Five Cisco NX-OS configurations for the "Try it" page of the Train Your Dragon demo, which converts NX-OS to Junos with a small, locally trained specialist model and proves every answer on a Junos lab switch.

Every file is synthetic. The customer, Northwind, is invented; its data centre, addresses, names and secrets are made up, and no file comes from a real network. Each file is written as a correct NX-OS configuration.

| File | What it is |
| --- | --- |
| `nxos/dc1-leaf1-running-config.txt` | Leaf switch, Northwind DC1: the whole running configuration |
| `nxos/tenant-vrf-evpn.txt` | Tenant network (VRF) with EVPN routes |
| `nxos/evpn-overlay.txt` | EVPN overlay between leaf switches |
| `nxos/bgp-underlay-bfd.txt` | Underlay BGP with fast failure detection (BFD) |
| `nxos/vpc-dual-homed.txt` | Dual-homed server links (vPC to ESI-LAG) |

# How to use one

1. Open a file and copy its text, for example `nxos/evpn-overlay.txt`.
2. On the demo's "Try it" page, paste it into "or paste your own Cisco NX-OS configuration".
3. Press "Convert to Junos".

The page accepts Cisco NX-OS only, at most 300 lines, and deletes a pasted configuration when its run ends.

# License

MIT, see `LICENSE`.
