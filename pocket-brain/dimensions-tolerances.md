---
layout: default
title: "Pocket Brain — dimensions and tolerances"
permalink: /pocket-brain/dimensions-tolerances/
device: pocket-brain
snapshot_date: 2026-10-04
---

# Pocket Brain — dimensions and tolerances

> **Public documentation snapshot**  
> Device: Pocket Brain  
> Source authority: private Pocket Brain engineering repository  
> Public snapshot date: 2026-10-04  
> Engineering evidence checked: 2026-10-03

This is not the fabrication or engineering authority. Raw engineering source remains private. Underlying engineering source retained in private source repository. Values below are nominal/model-derived, not manufacturing tolerances.

| Measure | Value | Boundary |
|---|---|---|
| Frozen Fusion v0.3 solid envelope (width × height × depth) | 65.0 × 105.0 × 22.085 mm | Reproduced nominal geometry. Not a tolerance-controlled drawing. |
| Concept battery envelope | 54.5 × 72.0 × 5.2 mm | Frozen envelope, not a supplier-qualified cell specification. |
| Concept battery closed-mesh volume | 20,156.512 mm³ | Model measurement, not measured pack energy. |
| Concept battery bounding volume | Approximately 20,404.8 mm³ | Bounding-box volume; not the usable cell volume. |
| Fusion-to-Blender maximum conversion delta | 0.003 mm | Reported presentation-conversion result, not a physical tolerance. |

Historical concept envelope/detail measurements have different version scopes. Do not replace the current Fusion envelope with older detailed-depth figures or mix them into a manufacturing specification.

Supplier tolerances, production variation, press-fit forces, bond specification and physical stack-up qualification remain **OPEN**. Tiny geometric search margins from historical trials are not qualified manufacturing clearances. Nominal fit alone does not establish process capability.

See [mechanical architecture]({{ '/pocket-brain/mechanical-architecture/' | relative_url }}) and [open issues]({{ '/pocket-brain/open-issues-validation/' | relative_url }}).
