---
layout: default
title: "Pocket Brain — electrical architecture"
permalink: /pocket-brain/electrical-architecture/
device: pocket-brain
snapshot_date: 2026-10-04
---

# Pocket Brain — electrical architecture

> **Public documentation snapshot**  
> Device: Pocket Brain  
> Source authority: private Pocket Brain engineering repository  
> Public snapshot date: 2026-10-04  
> Engineering evidence checked: 2026-10-03

This is not the fabrication or engineering authority. Raw engineering source remains private. Underlying engineering source retained in private source repository.

## Stage 6: architecture, not implementation

Stage 6 establishes the first electrical architecture and major component-selection authority. Fifteen major part numbers are selected; package identities are verified for 13/13 major packages. Pin-map authority is **PARTIAL**, with full capture remaining a subsequent implementation task.

**No schematic, PCB, netlist or routing exists.** ERC and DRC are not applicable yet. “Electronics complete” is not an accurate description.

| Block | Defined architecture | Unresolved boundary |
|---|---|---|
| Compute | i.MX 8M Plus compute architecture | Board integration, software/system performance and power validation. |
| Memory / storage | LPDDR4X, eMMC and recovery NOR selections | Implemented interconnect, signal integrity and availability qualification. |
| Power | Charger/power path, companion PMIC, PD sink and fuel-gauge selections | Schematic, rail sequencing, safety, thermal and real pack validation. |
| USB-C | USB 2.0 data + charging, UFP only | Mating/anchor fit and circuit integration. |
| Pogo | Five-contact power/ground/identification/service architecture | Custom module and charger-side qualification. |
| RF | Wi-Fi/BLE module and antenna/feed architecture | Footprint/height fit and metal-enclosure RF performance. |
| Interconnect | Main-to-I/O FFC architecture and pin allocation | Full pin capture, continuity and signal-integrity validation. |

Magnetic coupling remains product intent: magnets are not established in the device model. Interface names must not be read as hardware certification.

Battery requirements do not identify a qualified cell. Charging, capacity and runtime remain unverified. See [battery methodology]({{ '/pocket-brain/sources-evidence/' | relative_url }}#battery-methodology).
