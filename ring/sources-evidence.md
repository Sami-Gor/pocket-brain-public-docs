# Ring — public sources and evidence

> **Public documentation snapshot**  
> Device: Pocket Brain Ring  
> Source authority: private Pocket Brain engineering repository  
> Public snapshot date: 2026-10-02  
> Engineering state: [current-state.md](current-state.md)

This is a curated public summary, not the engineering authority or a fabrication release. Evidence statements below are reported from the private engineering record checked on 2026-10-02; this publication does not independently revalidate hardware. Underlying engineering source retained in private source repository.

This index describes evidence held privately; it does not provide public access to raw engineering files. **Underlying engineering source retained in private source repository.** No CAD, PCB, schematic, Blender, GLB, supplier records or raw audit exports are included in this public documentation repository.

| Evidence category | Status | What it supports / limits |
|---|---|---|
| Mechanical production authority | FROZEN | Fusion v0.4 freeze, 2026-09-27; production geometry authority |
| Independent mechanical geometry report | VERIFIED / REPORT ONLY | Reported 178/178 solids and zero unexplained interferences; not physical manufacturing verification |
| M3 alternate geometry | OPEN | Separate working implementation; production adoption unresolved |
| Main presentation model | VERIFIED | v0.4.1 assembly semantic/geometric presentation contract only |
| Component mapping | VERIFIED | 42/42 web semantic identities; distinct from engineering body/component counts |
| Electronics design record | OPEN | KiCad v0.1; pin-map/connectivity reconciliation required; earlier validation claims withdrawn |
| PCB placement/routing | OPEN / NOT READY | Placement present; KC-C5 human manual-routing handoff; connectivity/routing not closed |
| ERC/DRC reports | REPORT ONLY | Dated measurements; failures and parity issues remain; no fabrication approval |
| RF and power validation | OPEN / NOT PERFORMED | Antenna, matching, clock, battery, receiver and protection unresolved |
| NFC | SPECULATIVE | Excluded from the frozen function set |
| Physical prototype testing | NOT PERFORMED | No RF, thermal, IP, battery or hardware assembly validation |
| Source/provenance index | REPORT ONLY | Private index reports 59 entries; electronics-placement/export provenance gaps remain |
| Fabrication release | NOT READY | No accepted routed board or fabricator approval |

## Presentation identity

The private current-state record identifies main presentation v0.4.1 as 3,292,328 bytes with SHA-256:

`c3ee5d09d7f9c365fba933c9e3ca76f242355a0f91522d38ad94fc84828fb437`

Reported metrics: 42 meshes, 50 nodes, 8 ownership groups, 92,434 triangles, 14 exported materials and one Explode animation. These are presentation facts, not functional electronics evidence. Raw models are not distributed here.

## Public reading links

- [Current state](current-state.md)
- [Device dossier](device-dossier.md)
- [Mechanical architecture](mechanical-architecture.md)
- [Electrical architecture](electrical-architecture.md)
- [Dimensions and tolerances](dimensions-tolerances.md)
- [Engineering status](engineering-status.md)
- [Open issues and validation](open-issues-validation.md)
- [Sources and evidence](sources-evidence.md)
