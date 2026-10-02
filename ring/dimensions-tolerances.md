# Ring — dimensions and tolerances

> **Public documentation snapshot**  
> Device: Pocket Brain Ring  
> Source authority: private Pocket Brain engineering repository  
> Public snapshot date: 2026-10-02  
> Engineering state: [current-state.md](current-state.md)

This is a curated public summary, not the engineering authority or a fabrication release. Evidence statements below are reported from the private engineering record checked on 2026-10-02; this publication does not independently revalidate hardware. Underlying engineering source retained in private source repository.

Numbers are reported geometry or explicitly labelled targets. They are not released manufacturing tolerances or proof of supplier capability.

| Feature | Value | Qualification |
|---|---|---|
| Outer diameter | 28.6 mm nominal / 28.66 mm modelled | VERIFIED geometry; ±0.05 mm is an unconfirmed target |
| Bore | 21.05 mm modelled | VERIFIED geometry; ±0.05 mm target; single size only |
| Axial width | 8.90 mm | VERIFIED geometry; ±0.05 mm target |
| Shell wall | 0.90–1.05 mm nominal | ENGINEERING ASSUMPTION; ±0.08 mm target |
| Frozen production board | radii 11.720/12.270 mm; 150° | Fusion v0.4 authority |
| Separate M3 board | radii 11.430/11.980 mm; approximately 153.72° | Working implementation; adoption OPEN |
| Board stackup / axial width | 0.550 / 5.000 mm | Geometry; laminate/supplier specification not established |
| Battery envelope | 195.7 mm³ | VERIFIED geometric envelope, not an orderable cell/capacity |
| Battery swelling pocket | 0.376 mm nominal | Geometric allowance against 0.30 mm requirement; swelling not physically validated |
| Terminal separation | 0.04 mm insulated | Tight geometric provision; manufacturing/insulation risk OPEN |
| PCB–carrier wall | 0.02 mm role-level / 0.12 mm wall-local | Different measurement scopes; tolerance risk remains |
| M3 board–liner clearance | 0.108 mm | Working-geometry result, not adopted production geometry |
| M3 worst-case occupied height | 0.926 mm allowance vs 0.90 mm requirement | Datum/tolerance analysis, not supplier capability proof |
| Gasket compression | 25% nominal (20–30% target) | Geometry/design intent; sealing NOT PERFORMED |

Mass, battery capacity/runtime, RF impedance, physical thermal limits, supplier capability, IP rating and ring size range are not established. Geometric clearance results do not close electrical, RF or manufacturing issues.

See [mechanical architecture](mechanical-architecture.md) for authority separation.
