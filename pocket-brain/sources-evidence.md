---
layout: default
title: "Pocket Brain — sources and evidence"
permalink: /pocket-brain/sources-evidence/
device: pocket-brain
snapshot_date: 2026-10-04
---

# Pocket Brain — sources and evidence

> **Public documentation snapshot**  
> Device: Pocket Brain  
> Source authority: private Pocket Brain engineering repository  
> Public snapshot date: 2026-10-04  
> Engineering evidence checked: 2026-10-03

This is not the fabrication or engineering authority. Raw engineering source remains private. Underlying engineering source retained in private source repository. This is a **REPORT ONLY** evidence summary, not a new independent audit or a download of raw engineering records.

## Evidence boundaries

| Category | Reported state | Scope |
|---|---|---|
| Mechanical authority | FROZEN / nominal VERIFIED | Fusion v0.3 geometry/retention/closure only; fabrication NOT READY. |
| Presentation model | VERIFIED | Blender v1.0 conversion, not mechanical authority. |
| Component mapping | VERIFIED | 37 semantic identities in CAD-derived web v1.0; not a verified electronic BOM. |
| Electrical architecture | DEFINED / implementation OPEN | Stage 6 selection package; no schematic/PCB/netlist/routing. |
| Battery / power | Requirements defined / qualification OPEN | No supplier-qualified cell, real capacity or real runtime. |
| RF / thermal / charging | UNVALIDATED | Architecture/provision does not establish performance or safety. |
| Physical validation | NOT PERFORMED | No qualified functioning physical prototype established. |
| Open engineering issues | OPEN | Sourcing, electrical fit, manufacturing, interfaces and hardware tests. |
| Missing historical files | NOT_VERIFIABLE from absent files | Seven historical Stage-5 machine-readable files remain missing; no retroactive reconstruction. |

The private reconciled current-state document and its machine-readable record govern over older dossier/phase claims. This snapshot omits private source paths, raw ledgers, internal tool instructions, rejected checkpoint history and source downloads. It does not imply those records are publicly accessible.

## Presentation identity

The reported CAD-derived web v1.0 asset is 1,557,280 bytes, with 37 meshes, 16 materials and one Explode clip. Its SHA-256 is:

`b1e7e9411686faf64d6bd320285a3b9d95df14beee5e7825d932edf4fe37f237`

The private record reports a live hash check on 2026-10-03. Publishing this page does not perform a new deployment or live-hash verification.

## Battery methodology

### Model-derived measurement

The conceptual battery mesh is 54.5 × 72.0 × 5.2 mm, with a closed-mesh volume of 20,156.512 mm³ (20.156512 cm³). This is measured model geometry, **not measured hardware capacity**.

### Assumptions

- Usable-volume factor: 90%, leaving approximately 18.140861 cm³.
- Cell energy-density cases: 464, 700 and 935 Wh/L from the dated research model.
- Discharge utilisation: 90%.
- Aggregate conversion efficiency: 90%.
- Loads of 5, 10 and 15 W are sensitivity inputs, not measured device consumption.

The volume allowance models packaging, tabs, protection, insulation, swelling/assembly space and unusable edges. It is not a supplier-qualified pack specification. The density cases do not establish a cell fitting this envelope or current procurement availability.

### Calculated estimates

Nominal model energy = mesh volume in litres × usable-volume factor × assumed cell energy density. Usable model energy = nominal model energy × discharge utilisation × conversion efficiency. Runtime estimate = usable model energy ÷ assumed average load.

| Density case | Nominal model energy | Usable model energy | 5 W | 10 W | 15 W |
|---|---|---|---|---|---|
| 464 Wh/L | 8.417 Wh | 6.818 Wh | 1.364 h | 0.682 h | 0.455 h |
| 700 Wh/L | 12.699 Wh | 10.286 Wh | 2.057 h | 1.029 h | 0.686 h |
| 935 Wh/L | 16.962 Wh | 13.739 Wh | 2.748 h | 1.374 h | 0.916 h |

### Not verified

Supplier cell, actual pack capacity, runtime, discharge capability, cycle life, charging safety, thermal performance and certification are **not verified**. The research conclusion “feasible with constraints” is not fabrication approval or a product runtime specification. Stage 6 requirements are design targets, not qualified cell performance.

### Research references

The underlying research model was reviewed on 2026-08-30; it is retained as a dated calculation methodology, not refreshed procurement advice.

- [Grepow ultra-thin pouch cells](https://www.grepow.com/shaped-battery/ultra-thin-battery.html) — manufacturer data used for the 464 Wh/L case.
- [ATL products](https://www.atlbattery.com/en/product.html) — manufacturer data used for the 700 Wh/L case.
- [Enovix AI-1 testing announcement](https://ir.enovix.com/news-releases/news-release-details/independent-testing-confirms-enovix-ai-1tm-achieves-935-whl) — source used for the 935 Wh/L case; qualification/scaling caveats remain.
- [Amprius SiCore announcement](https://amprius.com/amprius-launches-sicore-450-wh-kg-high-energy-cell-with-near-term-mass-production-capability-to-scale/) — contextual advanced-density evidence, not proof of an envelope-matched cell.
- [Cell-to-system packing analysis](https://doi.org/10.3390/wevj11040077) — contextual research on packing losses; not a device-specific 90% allowance validation.

See [current state]({{ '/pocket-brain/current-state/' | relative_url }}) and [open validation]({{ '/pocket-brain/open-issues-validation/' | relative_url }}).
