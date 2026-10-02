---
layout: default
title: "Ring — electrical architecture"
permalink: /ring/electrical-architecture/
ring: true
---

# Ring — electrical architecture

> **Public documentation snapshot**  
> Device: Pocket Brain Ring  
> Source authority: private Pocket Brain engineering repository  
> Public snapshot date: 2026-10-02  
> Engineering state: [current-state.md]({{ '/ring/current-state/' | relative_url }})

This is a curated public summary, not the engineering authority or a fabrication release. Evidence statements below are reported from the private engineering record checked on 2026-10-02; this publication does not independently revalidate hardware. Underlying engineering source retained in private source repository.

## Current maturity

**RECONCILIATION_REQUIRED.** KiCad v0.1 is at KC-C5 human manual-routing handoff, not routing closure. Earlier pin-map verification and electrical-gate PASS claims were withdrawn as hardware validation claims.

## Intended devices and material discrepancies

| Device | Intended role | Open discrepancy |
|---|---|---|
| U4 nRF52840-CKAA-R7 | BLE MCU, 94-ball WLCSP | Schematic QIAA/aQFN-style 74-pin symbol incompatible with 94 PCB WLCSP pads — RING-E1 CRITICAL |
| U3 DRV8210 | Haptic H-bridge | Physical DSG pins 4/5/6/7/8 miswired — RING-E2 CRITICAL |
| U2 LSM6DSV16X | Six-axis IMU | Symbol-function labels incorrect; mapping not closed — RING-E3 |
| U1 BQ25180 | Single-cell charger | SYS/BAT both tied to VBAT; separated power path not implemented — RING-E4 |
| Charging provision | Inductive charging intent | Receiver/rectifier missing; coil nets are single-node islands — RING-E5 |
| U4 decoupling/GPIO | MCU support | Wrong DEC2/DEC3 assignments retained at E2/E3, which are P0.10/NFC2 and P1.06 — RING-E6 |
| U5 TPS7A02 | 1.8 V regulation | Order-code/package disagreement: SOT-23-5 versus 4-pad DQN; intended DQN code TPS7A0218PDQNR; rated 200 mA, not 25 mA — RING-E7 |
| Schematic–PCB association | Source synchronization | Footprint assignments/references broken — RING-E8 CRITICAL |

## Power and interfaces

I²C, SWD debug, BAT_MON divider, haptic drive and status indication are intended interfaces. The coil-to-charger-to-battery flow is intended architecture, not implemented charging circuitry. Temperature sense uses a fixed resistor, not implemented battery temperature sensing. Battery protection architecture, cell supplier, capacity, runtime and thermal limits are unresolved.

## PCB and RF

Placement exists; connectivity closure does not. Reported PCB counts: 32 footprints, 174 pads (127 with nets / 47 without), 64 retained track segments, 68 vias and 3 zones. There is no accepted routed release. Four-layer HDI, stackup, via technology and fabrication capability require confirmation.

BLE is intended but unvalidated. Matching implementation, antenna tuning, reference clock, impedance, VNA measurements, body detuning and metal-shell effects remain open. NFC is SPECULATIVE and excluded from frozen functions.

See [current state]({{ '/ring/current-state/' | relative_url }}) and [open issues]({{ '/ring/open-issues-validation/' | relative_url }}).
