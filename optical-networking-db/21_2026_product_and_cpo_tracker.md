# 2026 Product and CPO Tracker
> **Last Updated:** 2026-06-09
> **Status:** In Review
> **Tags:** CPO, silicon-photonics, products, NVIDIA, Broadcom, Marvell, 2026-refresh

## Overview
This file separates announced products, demonstrated hardware, customer sampling, and production deployment. It supplements [06_co_packaged_optics.md](06_co_packaged_optics.md) and should be used as the dated source of truth for 2025-2026 product status.

The central change since the initial database build is that CPO has moved from framework work and demonstrations to named switch platforms, disclosed customers, purchase commitments, and capacity investments. Production timing remains architecture-specific: Broadcom disclosed customer shipments for a 51.2T CPO switch, while NVIDIA's 102.4T and 409.6T photonics systems remain 2026 rollout programs.

> ⚠️ Note: Performance figures below are supplier claims unless explicitly labeled independently measured. “Announced” is not equivalent to generally available or high-volume production.

## Key Findings / Highlights
- [CONFIRMED] Broadcom's 51.2 Tb/s Bailly system combines a Tomahawk 5 switch ASIC with eight 6.4 Tb/s silicon-photonics engines; Broadcom stated in March 2024 that it had delivered systems to several customers [Source: Broadcom announcement reported by IBD, 2024-03-14].
- [CONFIRMED] NVIDIA announced Quantum-X Photonics and Spectrum-X Photonics switch families in March 2025, with 2026 rollout timing subsequently described for both InfiniBand and Ethernet [Source: NVIDIA GTC/Hot Chips disclosures, 2025].
- [CONFIRMED] NVIDIA's Spectrum SN6810 target is 128x800G / 102.4 Tb/s; SN6800 is 512x800G / 409.6 Tb/s; Quantum-X targets 144x800G / 115.2 Tb/s [Source: NVIDIA product disclosures, 2025-2026].
- [CONFIRMED] OIF has expanded CPO-adjacent standardization into 12.8T/6.4T near-package optics and compute-optics interfaces [Source: OIF Current Work, accessed 2026-06-09].
- [ESTIMATED] 2026 is an early-system-adoption year for CPO rather than broad replacement of 800G/1.6T pluggables [MED confidence].

## Detailed Content
### Product Status Matrix
| Vendor | Product / Program | Capacity | Architecture | Public Status | Timing | Evidence Quality |
|---|---|---:|---|---|---|---|
| Broadcom | Bailly + Tomahawk 5 | 51.2 Tb/s | 8 x 6.4T co-packaged optical engines | [CONFIRMED] delivered to several customers | disclosed 2024 | company announcement; customer identities mostly undisclosed |
| Broadcom | Tomahawk 6 generation | 102.4 Tb/s class | pluggable/CPO ecosystem options | [CONFIRMED] product generation; exact CPO configurations vary | 2025-2026 | official product roadmap; SKU-level validation required |
| NVIDIA | Quantum-X Photonics | 115.2 Tb/s; 144x800G | liquid-cooled InfiniBand CPO switch | [CONFIRMED] announced; adopter names disclosed at SC25 | 2026 rollout | official platform claims; deployment validation pending |
| NVIDIA | Spectrum SN6810 | 102.4 Tb/s; 128x800G | liquid-cooled Ethernet CPO switch | [CONFIRMED] announced | 2H 2026 target | official roadmap |
| NVIDIA | Spectrum SN6800 | 409.6 Tb/s; 512x800G | multi-switch/system-scale photonics platform | [CONFIRMED] announced | 2H 2026 target | official roadmap; topology boundary must be checked |
| Marvell | 1.6T PAM4 DSP / Ara-class portfolio | 1.6 Tb/s module | advanced-node DSP for pluggables | [CONFIRMED] merchant product roadmap | 2025-2026 | official product releases; volume by customer undisclosed |
| Marvell | custom XPU CPO platform | multi-terabit optical scale-out | CPO integrated into custom accelerator designs | [CONFIRMED] available for custom design engagement | announced 2025 | company disclosure; no named HVM deployment |
| Intel/Jabil | former Intel silicon-photonics product business | 100G-800G-class portfolio | pluggable SiPh manufacturing | [CONFIRMED] transferred to Jabil in 2023 | ongoing | ownership corrected; Intel remains an R&D/foundry actor |
| Ayar Labs | TeraPHY + SuperNova | multi-Tb/s optical I/O | in-package WDM chiplet + external laser | [CONFIRMED] demonstrations/partner programs | qualification stage | no public HVM customer volume |
| Ranovus | Odin / ORON | multi-Tb/s engines | CPO/NPO optical engines | [CONFIRMED] demonstrations and partner programs | pre-HVM | deployment quantities undisclosed |

### NVIDIA Claim Boundary
| Metric | Pluggable Baseline Claimed | CPO Claimed | Status |
|---|---:|---:|---|
| Per-port power | ~30 W | ~9 W | [CONFIRMED vendor claim], not independent measurement |
| Electrical channel loss | ~22 dB | ~4 dB | [CONFIRMED vendor design comparison] |
| Power efficiency | 1.0x | 3.5x | [CONFIRMED vendor claim] |
| Signal integrity | 1.0x | 64x improvement | definition requires source-slide review |
| Resiliency | 1.0x | 10x improvement | modeled component-count claim |
| Deployment time | baseline | ~30% faster | modeled operational claim |

### Adoption Evidence
| Organization | Platform / Supplier | Disclosure | Interpretation |
|---|---|---|---|
| TACC | NVIDIA Quantum-X Photonics | named prospective adopter at SC25 | credible early deployment signal |
| Oak Ridge National Laboratory | NVIDIA Quantum-X Photonics | named prospective adopter | HPC validation pathway |
| CoreWeave | NVIDIA Quantum-X Photonics | named prospective adopter | cloud AI deployment signal |
| Lambda | NVIDIA Quantum-X Photonics | named prospective adopter | cloud AI deployment signal |
| ByteDance | Broadcom CPO | executive testimonial on CPO need | support signal, not proof of awarded volume |
| undisclosed customers | Broadcom Bailly | Broadcom said several customer deliveries | shipment evidence without quantity |

### Readiness Gate
| Gate | Bailly 51.2T | NVIDIA 102.4T+ | Optical I/O Chiplets |
|---|---|---|---|
| Named silicon | yes | yes | yes |
| Named system SKU | yes | yes | generally no complete switch SKU |
| Customer shipment | limited disclosure | prospective/early | partner samples |
| Independent watts/Tb test | no public dataset found | no public dataset found | no public dataset found |
| Field failure data | undisclosed | undisclosed | undisclosed |
| HVM volume | undisclosed | not yet established | not established publicly |

## Data Tables (where applicable)
| Field | Value | Source | Date |
|---|---|---|---|
| Bailly optical engines | 8 x 6.4 Tb/s | Broadcom | 2024-03 |
| NVIDIA Quantum-X ports | 144 x 800G | NVIDIA | 2025-2026 roadmap |
| NVIDIA SN6810 ports | 128 x 800G | NVIDIA | 2025-2026 roadmap |
| NVIDIA SN6800 ports | 512 x 800G system | NVIDIA | 2025-2026 roadmap |
| OIF NPO project | 12.8T and 6.4T modules | OIF | active 2026 |

## Open Questions / Gaps
- Obtain generally-available dates, shipment units, pricing, and field-reliability data for each CPO SKU.
- Clarify whether SN6800's 409.6T figure represents a single chassis/system versus a single switching ASIC.
- Verify Tomahawk 6 CPO package options and named customers.
- Add Marvell SKU-level power and customer qualification status.
- Add independent lab measurements for switch-level watts/Tb and BER margin.

## References
- NVIDIA Networking | https://www.nvidia.com/en-us/networking/ | 2026-06-09
- NVIDIA GTC 2025 photonics coverage | https://www.techradar.com/pro/nvidia-is-planning-post-copper-1-6tbps-network-tech-to-connect-millions-of-gpus-as-it-unveils-photonics-networking-gear-at-gtc-2025 | 2026-06-09
- NVIDIA Hot Chips roadmap coverage | https://www.tomshardware.com/networking/nvidia-outlines-plans-for-using-light-for-communication-between-ai-gpus-by-2026-silicon-photonics-and-co-packaged-optics-may-become-mandatory-for-next-gen-ai-data-centers | 2026-06-09
- Broadcom Bailly coverage | https://www.investors.com/news/technology/broadcom-stock-avgo-bailly-cpo-ethernet-switch-ai/ | 2026-06-09
- OIF Current Work | https://www.oiforum.com/technical-work/current-work/ | 2026-06-09
