# Production Ramp and Supply Chain
> **Last Updated:** 2026-06-09
> **Status:** Draft
> **Tags:** supply-chain, manufacturing, capacity, CHIPS-Act, export-controls

## Overview
Datacenter optics production links III-V epitaxy and lasers, silicon-photonics and DSP wafers, advanced packaging, optical sub-assemblies, module assembly/test, switch integration, and hyperscaler qualification. Bottlenecks can migrate between layers as a new speed generation ramps.

A product announcement is not a production ramp. Pilot builds establish function, low-volume manufacturing establishes repeatability, and HVM requires yield, automated test, qualified second sources, field reliability, and customer acceptance.

> 🔄 Refresh Needed: High Priority — replace 2025-era lead-time and capacity assumptions with supplier disclosures and channel checks.

## Key Findings / Highlights
- [CONFIRMED] Advanced DSP/SerDes production is concentrated at leading foundries, especially TSMC.
- [CONFIRMED] III-V laser/EML capacity uses specialized InP/GaAs epitaxy and fabrication distinct from silicon CMOS.
- [CONFIRMED] China and Southeast Asia are important module-assembly regions; Fabrinet has major Thailand operations.
- [ESTIMATED] 200G/lane optical yield and test capacity are key constraints for the 1.6T ramp [MED confidence].
- [CONFIRMED] Export controls and entity restrictions can affect advanced chips, equipment, customers, and design collaboration; applicability is product/end-user specific.

## Detailed Content
### Supply Chain Map
| Layer | Inputs | Representative Players / Regions | Bottleneck |
|---|---|---|---|
| III-V wafer growth | InP/GaAs substrates, epitaxy | Coherent, Lumentum, Sumitomo, Mitsubishi | defect density, epi capacity |
| SiPh foundry | SOI wafers, masks | Intel, GF, TSMC, Tower, imec | PDK maturity, wafer/test capacity |
| DSP/SerDes ASIC | advanced CMOS | TSMC plus fabless vendors | leading-node allocation |
| Optical sub-assembly | PIC, laser, FAU, TIA/driver | Asia/US/Europe suppliers | alignment and known-good die |
| Module assembly | OSA, PCB, cage, firmware | InnoLight, Eoptolink, AAOI, Fabrinet/FIT | automation, calibration, test time |
| System integration | switch, NOS, optics | Arista, Cisco, NVIDIA, ODMs | interoperability and thermals |
| Deployment | fiber plant, qualification | hyperscalers/operators | approval cycles and field operations |

### SiPh Capacity
| Platform | Model | Capacity Visibility | Key Risk |
|---|---|---|---|
| Intel | captive/integrated | limited public detail | strategy and external access |
| GF Fotonix | open foundry | commercial | customer ramp and packaging ecosystem |
| TSMC | advanced integration/COUPE roadmap | [TO VERIFY] | capacity allocation and maturity |
| Tower | open foundry | commercial | scale and qualified design ecosystem |
| imec/CEA-Leti/AIM | R&D/pilot/transfer | program based | transfer to HVM |

### Contract Manufacturing
| Company | Main Role | Geography | Optical Relevance |
|---|---|---|---|
| Fabrinet | precision optical/electromechanical manufacturing | Thailand | high |
| Foxconn Interconnect Technology | connectors/modules/assembly | China/Asia/global | high [TO VERIFY mix] |
| Benchmark Electronics | complex electronics manufacturing | global | selective optical/system programs |
| module vendors/ODMs | vertically integrated module production | China/Asia | high |

### Ramp Timeline
| Technology | Pilot Production | Low Volume | HVM | Key Bottleneck |
|---|---|---|---|---|
| 800G-DR4/DR8 | 2022-2023 | 2023 | 2024-2025 | laser/PIC yield, test |
| 800G-SR8 | 2022-2023 | 2023-2024 | 2024-2025 | VCSEL bandwidth/reliability |
| LPO 800G | 2023-2024 | 2024-2025E | [TO VERIFY] | host channel and interoperability |
| CPO 51.2T | 2022-2024 demos | limited pilots | [TO VERIFY] | package yield/serviceability |
| 1.6T-DR8 | 2024-2025 samples | 2025-2026E | 2026-2027E | 200G/lane ecosystem |
| CPO 102.4T | 2024-2026 demos | 2026-2027E | 2027+ | optical engine/ELS/package |

> ⚠️ Note: Timeline ranges are synthesis estimates, not supplier commitments. Update at SKU and customer-qualification level.

### Geographic Concentration
| Region | Concentration | Risk |
|---|---|---|
| Taiwan | advanced CMOS, packaging, emerging SiPh | geopolitics, capacity allocation |
| China | module assembly and optical suppliers | export controls, tariffs, customer restrictions |
| US | fabless DSP, SiPh IP, compound-semiconductor assets | higher cost, limited specialized capacity |
| Japan | lasers, materials, precision components | supplier concentration |
| Southeast Asia | contract manufacturing | logistics, labor, geographic concentration |
| Europe | R&D, equipment, photonics institutes | scale-up transfer |

### Policy Effects
- US CHIPS Act programs may support domestic advanced packaging, silicon photonics, and compound semiconductors, but award-specific capacity must be verified.
- AIM Photonics supports domestic process access, packaging, test, education, and prototyping.
- BIS rules can restrict exports based on classification, destination, end user, and end use; “optical module” alone is not a sufficient conclusion.
- Entity List impacts are company-specific and change over time [See: [19_regulatory_and_standards_bodies.md](19_regulatory_and_standards_bodies.md)].

## Data Tables (where applicable)
| Field | Value | Source | Date |
|---|---|---|---|
| Leading DSP foundry concentration | TSMC-heavy | supplier disclosures | 2024 |
| US shared SiPh ecosystem | AIM Photonics | AIM | active 2024 |
| Major optical CM location | Thailand | Fabrinet filings | 2024 |
| 800G ramp | AI-led HVM expansion | vendor commentary | 2024 |
| 1.6T bottleneck | 200G/lane yield/test [ESTIMATED] | industry synthesis | 2025E |

## Open Questions / Gaps
- Collect wafer starts, tool capacity, yields, lead times, and utilization by layer.
- Map country of origin and alternate source for each critical component.
- Track customer qualification dates separately from vendor HVM claims.
- Add current ECCNs, Entity List parties, and license requirements with counsel.
- Quantify CHIPS Act awards tied directly to photonics capacity.

## References
- US CHIPS for America | https://www.nist.gov/chips | 2026-06-09
- AIM Photonics | https://www.aimphotonics.com/ | 2026-06-09
- BIS Entity List | https://www.bis.gov/regulations/ear/744-supp-4 | 2026-06-09
- Fabrinet filings | https://investor.fabrinet.com/ | 2026-06-09
- GlobalFoundries Fotonix | https://gf.com/technology-platforms/fotonix/ | 2026-06-09
