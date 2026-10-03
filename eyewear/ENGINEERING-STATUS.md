---
layout: default
title: "Eyewear — engineering status"
permalink: /eyewear/engineering-status/
device: eyewear
snapshot_date: 2026-10-03
ring: false
---

# Eyewear — engineering status

> **Public snapshot · 2026-10-03.** The private Pocket Brain engineering repository remains the source authority. This curated public summary is not a fabrication release, validated product specification or distribution of engineering source files.

## Release boundary

**Fabrication: NOT READY.** LEFT is routed but incomplete. RIGHT is unrouted and fabrication-blocking. R1–R7 remain OPEN; R8 is VERIFIED_CLOSED only for the documented intentional USB no-connect. R9/EW-E1 remains OPEN / CRITICAL. EW-E2 remains OPEN. Pin 42 connectivity is unresolved.

S24 / v0.14 remains **SOURCE_EXISTS_BUT_NOT_EXPORTED**: a cached source exists, but authoritative exports and sign-off evidence have not been independently recovered. The reported 80° nesting fold has not been independently reproduced. The historical electronics GLB relationship is **NOT_VERIFIABLE**.

## Material status summary

| Area | Status |
|---|---|
| Fabrication | NOT READY |
| Mechanical | S24 / v0.14 report only; authoritative exports and sign-off recovery pending |
| Schematic | Reconciliation and pin 42 connectivity unresolved |
| PCB LEFT | Routed but incomplete |
| PCB RIGHT | Unrouted; fabrication-blocking |
| Routing | R9/EW-E1 OPEN / CRITICAL |
| Electronics placement | EW-E2 OPEN; V2.0.1 source placement does not verify runtime transforms or v0.14 fit |
| Historical model reconciliation | NOT_VERIFIABLE |
| Supplier stack-up / impedance | OPEN |
| RF / power / thermal / fit / sealing | Physical validation OPEN or unverified |

Current-state reconciliation takes precedence over superseded historical statements. The existence of electronics files resolves an earlier evidence-availability gap; it does not resolve correctness or release readiness. Only R8 has the specifically documented verified closure described above.
