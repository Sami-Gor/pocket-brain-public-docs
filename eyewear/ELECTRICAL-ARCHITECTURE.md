---
layout: default
title: "Eyewear — electrical architecture"
permalink: /eyewear/electrical-architecture/
device: eyewear
snapshot_date: 2026-10-03
ring: false
---

# Eyewear — electrical architecture

> **Public snapshot · 2026-10-03.** The private Pocket Brain engineering repository remains the source authority. This curated public summary is not a fabrication release, validated product specification or distribution of engineering source files.

## Existing design evidence

A schematic and two PCB design records exist. The documented BOM has 69 data rows; this is not a verified assembled-unit count. A generated release package or successful file/hash check does not establish DRC-clean routing, manufacture readiness or electrical function.

| Board | Current evidence | Release boundary |
|---|---|---|
| LEFT | Six copper layers; routed but incomplete | Electrical and manufacturing issues remain open |
| RIGHT | Four copper layers; 39 placed footprints; 0 tracks, 0 vias, 0 zones | Unrouted; fabrication-blocking |

Logical copper-layer reconciliation does not establish supplier-approved physical stack-up or impedance. Pin 42 remains **PIN42_CONNECTIVITY_UNRESOLVED**; a prior documentation-only assertion was withdrawn.

## Power, sensors and RF

The concept uses protected cell arrangements; it must not be interpreted as evidence of a validated raw parallel-cell connection. Capacity, chemistry, charging safety and runtime require verification. Modelled sensors and acoustic parts are design intent, not tested function. RF tuning, impedance, body-loading and performance testing remain open.

## Release boundary

**Fabrication: NOT READY.** LEFT is routed but incomplete. RIGHT is unrouted and fabrication-blocking. R1–R7 remain OPEN; R8 is VERIFIED_CLOSED only for the documented intentional USB no-connect. R9/EW-E1 remains OPEN / CRITICAL. EW-E2 remains OPEN. Pin 42 connectivity is unresolved.

S24 / v0.14 remains **SOURCE_EXISTS_BUT_NOT_EXPORTED**: a cached source exists, but authoritative exports and sign-off evidence have not been independently recovered. The reported 80° nesting fold has not been independently reproduced. The historical electronics GLB relationship is **NOT_VERIFIABLE**.
