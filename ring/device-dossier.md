# Ring — curated device dossier

> **Public documentation snapshot**  
> Device: Pocket Brain Ring  
> Source authority: private Pocket Brain engineering repository  
> Public snapshot date: 2026-10-02  
> Engineering state: [current-state.md](current-state.md)

This is a curated public summary, not the engineering authority or a fabrication release. Evidence statements below are reported from the private engineering record checked on 2026-10-02; this publication does not independently revalidate hardware. Underlying engineering source retained in private source repository.

## Purpose and functions

Finger-worn interaction accessory intended to combine BLE communication, MCU processing, IMU motion sensing, haptics, status indication, battery voltage monitoring, inductive charging, power regulation and firmware/debug access. These are requirements/design intent, not verified operating functions.

PPG, ECG, skin temperature, SpO₂, NFC payments, Wi-Fi and cellular functions are not confirmed in the frozen function set. There is no display, audio subsystem, camera, hinge or external finished-product connector.

## Physical architecture

Nominal outer diameter 28.6 mm (modelled 28.66 mm), bore 21.05 mm and axial width 8.9 mm. A two-piece shell encloses a liner, formed carrier, rigid-flex board, battery and haptic envelopes, charging coil, antenna provision, status light and retention/sealing features.

The digital assembly exposes 42 semantic components and 8 ownership groups. The Fusion record accounts for 11 components with 60 occurrence bodies plus a root reference body. These are different representation scopes, not interchangeable inventories.

Internal parts install before final welded/adhesive closure. No field-serviceable access is established. Materials and tolerances remain candidates/targets, not supplier-validated specifications.

## Engineering boundaries

Fusion v0.4 is the frozen mechanical authority. M3 remains an alternate working geometry with adoption unresolved. KiCad v0.1 is at KC-C5 manual-routing handoff with schematic reconciliation and connectivity unresolved. Detailed electronics placement inside the Ring is not verified. No firmware programme or functioning physical prototype is established by this snapshot.

**Fabrication NOT READY; physical validation NOT PERFORMED.**

- [Current state](current-state.md)
- [Device dossier](device-dossier.md)
- [Mechanical architecture](mechanical-architecture.md)
- [Electrical architecture](electrical-architecture.md)
- [Dimensions and tolerances](dimensions-tolerances.md)
- [Engineering status](engineering-status.md)
- [Open issues and validation](open-issues-validation.md)
- [Sources and evidence](sources-evidence.md)
