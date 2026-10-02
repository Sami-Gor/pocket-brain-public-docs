---
layout: default
title: "Ring — open issues and validation"
permalink: /ring/open-issues-validation/
ring: true
---

# Ring — open issues and validation

> **Public documentation snapshot**  
> Device: Pocket Brain Ring  
> Source authority: private Pocket Brain engineering repository  
> Public snapshot date: 2026-10-02  
> Engineering state: [current-state.md]({{ '/ring/current-state/' | relative_url }})

This is a curated public summary, not the engineering authority or a fabrication release. Evidence statements below are reported from the private engineering record checked on 2026-10-02; this publication does not independently revalidate hardware. Underlying engineering source retained in private source repository.

## Reconciled issue register

The private canonical audit register remains the authority for issue closure. Removing a website feature or correcting public copy does not mark an engineering issue closed. Historical visualization/copy findings below are dated audit records, not claims about the cleaned-up website's current runtime.

| ID | Finding | Severity | Canonical status |
|---|---|---|---|
| RING-M1 | M3 production adoption unresolved | HIGH | OPEN |
| RING-E1 | MCU symbol/package/pin-map mismatch (QIAA/aQFN symbol, 74 pins incl. EP, no footprint; PCB 94 WLCSP pads; schematic-to-PCB pin mapping untrustworthy) | CRITICAL | OPEN |
| RING-E2 | DRV8210 symbol/pin connectivity incorrect (physical pins 4/5/6/7/8 miswired; functional circuit defect, not ERC convention) | CRITICAL | OPEN |
| RING-E3 | IMU symbol-function mapping inconsistent; ERC interpretation compromised; no pin-map closure until revalidated | HIGH | OPEN |
| RING-E4 | BQ25180 SYS/BAT architecture unresolved (SYS and BAT both connected to VBAT; R9 removal correct) | HIGH | OPEN |
| RING-E5 | Inductive charging receiver/rectifier missing (COIL_1/COIL_2 single-node islands on L1 only; DC charger input) | HIGH | OPEN |
| RING-E6 | PCB retains erroneous DEC2/DEC3 GPIO assignments (U4 pads E2/E3; CKAA functions P0.10/NFC2 and P1.06; C6/C7 remain on PCB) | HIGH | OPEN |
| RING-E7 | LDO package/order-code identity unresolved (schematic PDBVR/SOT-23-5 vs PCB 4-pad DQN vs documented PDRVR; correct DQN = PDQNR; 200 mA not 25 mA) | MEDIUM | OPEN |
| RING-E8 | Schematic/PCB association broken (23 refs without footprints; parity 32 extra / 31 duplicate / 23 missing) | CRITICAL | OPEN |
| RING-EV1 | Historical visualization did not establish detailed in-Ring electronics placement | HIGH | OPEN |
| RING-EV2 | Historical visualization lifecycle defects recorded in the audit | MEDIUM | OPEN |
| RING-RF1 | RF implementation/validation incomplete | HIGH | OPEN |
| RING-RF2 | Historical unsupported NFC product-copy claim; current website copy states NFC is speculative/excluded | MEDIUM | OPEN |

## Additional unresolved validation

- Battery cell selection, swelling, protection, discharge behaviour and capacity/runtime.
- Terminal conductor, insulation, strain relief, fatigue and tight separation.
- RF tuning, shell attenuation, body detuning and confirmed impedance/stackup.
- Supplier tolerance capability, carrier gaps and curved-board manufacturing.
- Charging coupling/heating through the metal bottom face.
- Seal/IP qualification, weld/adhesive life and retention.
- Skin-contact thermal limits, optics/status-light coupling and human sizing.
- Firmware, IMU driver, sealed-device OTA update/debug and BLE application.
- Physical assembly, regulatory validation and fabricator HDI review.
- Historical documentation discrepancies: two end stops versus a three-stop narrative, incomplete version history, superseded constraint values and PCB-generator net declarations.

**No physical prototype validation has been performed.**

## Repair dependencies

Establish source authority; repair MCU and peripheral symbols/packages/connectivity; reconcile clock/DEC/debug support and power/charging; synchronize schematic and PCB; regenerate affected placement/copper; then route, close ERC/DRC and obtain fabricator review. Resolve M3 adoption through controlled mechanical revision. Physical testing remains required. Routing alone cannot resolve the earlier electrical defects.
