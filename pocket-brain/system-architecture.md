---
layout: default
title: "Pocket Brain — system architecture"
permalink: /pocket-brain/system-architecture/
device: pocket-brain
snapshot_date: 2026-10-04
---

# Pocket Brain — system architecture

> **Public documentation snapshot**  
> Device: Pocket Brain  
> Source authority: private Pocket Brain engineering repository  
> Public snapshot date: 2026-10-04  
> Engineering evidence checked: 2026-10-03

This is not the fabrication or engineering authority. Raw engineering source remains private. Underlying engineering source retained in private source repository.

| System | Intended role | Qualification |
|---|---|---|
| Enclosure / structure | Caps, frame, board carrier, battery support and retention | Frozen nominal geometry; physical/manufacturing qualification open. |
| Compute / memory / storage | Local compute and data continuity | Stage 6 architecture and part selection defined; no implemented board. |
| Battery / power | Energy storage, charge management and system rails | Envelope and requirements defined; cell and performance unqualified. |
| USB / pogo I/O | Data, charging and service interfaces | Architecture defined; electrical and mating validation open. |
| RF | Wireless companion module and antenna/feed provision | Architecture defined; RF performance unvalidated. |
| Thermal | Compute-to-spreader/enclosure path and battery isolation | Nominal provision only; heat rejection and cell temperature unvalidated. |
| Status / service | Status indication and reset/service provisions | Interface implementation and product decisions remain open. |

## Component mapping

The web model has **37 mapped semantic components**. Labels group presentation geometry; they are not a verified bill of electronic parts or proof of soldered connectivity. A semantic component may contain multiple CAD solids. Category grouping does not replace mechanical ownership or electrical nets.

The model's memory/storage proxies must not be treated as the selected hardware population. Stage 6 defines the electrical selections separately; no real PCB implementation exists yet.

See [electrical architecture]({{ '/pocket-brain/electrical-architecture/' | relative_url }}) for the implementation boundary and [device dossier]({{ '/pocket-brain/device-dossier/' | relative_url }}) for the authority split.
