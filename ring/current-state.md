# Ring — current engineering snapshot

> **Public documentation snapshot**  
> Device: Pocket Brain Ring  
> Source authority: private Pocket Brain engineering repository  
> Public snapshot date: 2026-10-02  
> Engineering state: [current-state.md](current-state.md)

This is a curated public summary, not the engineering authority or a fabrication release. Evidence statements below are reported from the private engineering record checked on 2026-10-02; this publication does not independently revalidate hardware. Underlying engineering source retained in private source repository.

## Current state

| Area | State | Evidence boundary |
|---|---|---|
| Mechanical | PARTIALLY_VERIFIED | Frozen Fusion v0.4 geometry is reported valid; M3 remains separate and unadopted (RING-M1). |
| Presentation | VERIFIED | 42/42 semantic mapping in the v0.4.1 web assembly; presentation only. |
| Schematic | RECONCILIATION_REQUIRED | RING-E1–E8 open; E1, E2 and E8 critical. Historical pin-map and electrical-gate validation claims withdrawn. |
| PCB | PLACEMENT_PRESENT_CONNECTIVITY_UNRESOLVED | 32 footprint blocks, 174 pads: 127 netted / 47 without nets; 33 unconnected items. |
| Routing | NOT CLOSED | KC-C5 manual-routing handoff; failed first-pass copper retained; no accepted routed board or fabrication release. |
| RF | INCOMPLETE_UNVALIDATED | Matching, antenna, reference clock, impedance and body/metal-shell testing unresolved. |
| Power | INCOMPLETE_WITH_CORRECTNESS_ISSUES | SYS/BAT unresolved; receiver/rectifier missing; supplier, protection and capacity/runtime not defined. |
| Fabrication | NOT READY | Schematic/PCB association, routing and fabricator/HDI confirmations open. |
| Physical validation | NOT PERFORMED | No physical prototype; no RF, thermal, IP, battery or hardware assembly validation. |

## Governing corrections

- Frozen Fusion v0.4 board geometry: radii 11.720/12.270 mm, 0.550 mm radial stackup, 5.000 mm axial width, 150° hoop.
- M3 working geometry: radii 11.430/11.980 mm, 0.290 mm inward displacement, approximately 153.72° hoop. It is not adopted into the frozen production master.
- Synthesized-netlist self-consistency did not validate hardware connectivity. The netlist is not a native KiCad export.
- Fresh ERC report: 3 errors + 14 warnings. DRC observations: 769 violations in the reconciliation run and 770 in the same-day audit, plus 33 unconnected items and 86 parity issues. These are point-in-time observations, not one invariant count.
- Parity findings: 32 extra / 31 duplicate / 23 missing footprints; all 23 physical schematic references lacked footprint assignments.
- Actual 0.20/0.10 mm vias meet the encoded project minima; fabricator capability remains unconfirmed.
- Battery capacity, runtime, physical materials, supplier capability and IP rating are not established.
- NFC is SPECULATIVE and excluded from the frozen function set; BLE implementation is not validated.

## Presentation versus engineering

The web model has 42 semantic meshes, 50 nodes including 8 ownership groups, 92,434 triangles, 14 exported materials and one Explode animation. Its verified mapping does not certify electronics, manufacturing, materials or physical performance. The saved Blender master has 13 material datablocks; an earlier 17-material candidate count is historical.

Historical presentation findings RING-EV1/EV2 and copy finding RING-RF2 remain OPEN in the private audit register. Website changes do not formally close those engineering records or establish detailed electronics placement.

See [open issues](open-issues-validation.md) and [evidence boundaries](sources-evidence.md).
