---
layout: default
title: "Ring — mechanical architecture"
permalink: /ring/mechanical-architecture/
ring: true
---

# Ring — mechanical architecture

> **Public documentation snapshot**  
> Device: Pocket Brain Ring  
> Source authority: private Pocket Brain engineering repository  
> Public snapshot date: 2026-10-02  
> Engineering state: [current-state.md]({{ '/ring/current-state/' | relative_url }})

This is a curated public summary, not the engineering authority or a fabrication release. Evidence statements below are reported from the private engineering record checked on 2026-10-02; this publication does not independently revalidate hardware. Underlying engineering source retained in private source repository.

## Authority

**FROZEN:** Fusion Engineering Master v0.4, dated 2026-09-27. The private independent FreeCAD report records 178/178 valid solids and zero unexplained hard interferences. This verifies analysed geometry, not physical manufacturing or fit under tolerance.

## Packaging

Ring axis is Fusion Z / web Y. Components occupy complementary circumferential zones: front electronics/antenna, rear battery, lower haptic, bottom-face charging and a side status-light insert. The carrier uses formed/stamped thin sections, battery end stops, compliant support and liner capture features.

The shell comprises a main section and bottom cap with welded/adhesive final closure. Face openings are smaller than the battery envelope, so internals install before closure. Sampled digital assembly paths have supporting reports; those cannot prove the physical assembly process.

## Production board versus M3

| Geometry | Frozen production v0.4 | Separate M3 working geometry |
|---|---|---|
| Board inner/outer radius | 11.720 / 12.270 mm | 11.430 / 11.980 mm |
| Hoop | 150° | approximately 153.72° |
| Radial stackup | 0.550 mm | 0.550 mm |
| Axial width | 5.000 mm | 5.000 mm |
| Production adoption | FROZEN authority | UNRESOLVED — RING-M1 OPEN |

M3 adds capture ledges, carrier notches, re-formed straps and a translated ribbon. It must not be described as incorporated into the frozen production master. A controlled ADOPT / REJECT / SUPERSEDE decision is required.

## Open physical constraints

Battery supplier and swelling behaviour; terminal conductor/insulation and 0.04 mm insulated separation; tight carrier clearances; tolerance capability; weld distortion; adhesive/retention life; seal performance; skin-contact/thermal limits and ring size range remain unresolved. No IP rating or physical process validation is claimed.

See [dimensions]({{ '/ring/dimensions-tolerances/' | relative_url }}) and [open validation]({{ '/ring/open-issues-validation/' | relative_url }}).
