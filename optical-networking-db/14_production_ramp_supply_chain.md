# Production Ramp and Supply Chain
> **Last Updated:** 2026-06-09
> **Status:** In Review
> **Tags:** supply-chain, manufacturing, capacity, yield, lead-time, CHIPS-Act

## Overview
Datacenter optics production links III-V epitaxy and lasers, SiPh and DSP wafers, advanced packaging, optical subassemblies, module assembly/test, switch integration, and hyperscaler qualification. Bottlenecks migrate as a new speed generation ramps.

Public companies disclose revenue, capex, facilities, and selected unit targets but rarely publish optical assembly yield or customer-specific lead time. This section records hard capacity signals, distinguishes nameplate capacity from accepted shipments, and leaves unavailable yield metrics explicitly blank rather than inventing percentages.

> ⚠️ Note: Nameplate capacity, qualified capacity, good-unit output, and customer-accepted shipments are different measures. A product announcement is not a production ramp.

## Key Findings / Highlights
- [CONFIRMED] AAOI targeted 100,000 800G transceivers per month by year-end 2025, with about 35% of production planned in the US [Source: AAOI earnings coverage, 2025-11].
- [CONFIRMED] Fabrinet reported FY2026 Q2 revenue of $1.13B; HPC revenue increased from $15.4M to $85.6M sequentially, with management targeting more than $150M at full ramp for the first program [Source: Fabrinet coverage, 2026-02].
- [CONFIRMED] NVIDIA's 2026 arrangements with Coherent and Lumentum included $2B investments plus purchase and capacity-access provisions [Source: company announcement coverage, 2026-03].
- [CONFIRMED] Meta and Amazon agreements are driving Corning capacity expansion in North Carolina [Source: agreement coverage, 2026].
- [ESTIMATED] Advanced lasers, 200G/lane optical yield/test, and CPO package test/rework are the leading 2026 bottlenecks [MED confidence].

## Detailed Content
### Supply Chain Map
| Layer | Inputs | Representative Players / Regions | Bottleneck |
|---|---|---|---|
| III-V wafer growth | InP/GaAs substrates, epitaxy | Coherent, Lumentum, Sumitomo, Mitsubishi | defect density and epi capacity |
| SiPh foundry | SOI wafers, masks | Intel, GF, TSMC, Tower, imec | PDK maturity, wafer/test capacity |
| DSP/SerDes ASIC | advanced CMOS | TSMC and fabless vendors | leading-node allocation |
| Optical subassembly | PIC, laser, FAU, TIA/driver | Asia/US/Europe suppliers | alignment and known-good die |
| Module assembly | OSA, PCB, firmware, cage | InnoLight, Eoptolink, AAOI, Fabrinet/FIT | automation, calibration, test time |
| System integration | switch, NOS, optics | Arista, Cisco, NVIDIA, ODMs | interoperability and thermals |
| Deployment | fiber plant, qualification | hyperscalers/operators | approval cycles and field operations |

### Disclosed Capacity and Ramp Signals
| Supplier | Capacity / Ramp Signal | Date | Known | Not Disclosed |
|---|---|---:|---|---|
| AAOI | 100k 800G modules/month target; 35% US | 2025 year-end target | module target and geography | achieved output, product mix, yield |
| Fabrinet | HPC revenue $15.4M to $85.6M; >$150M full-ramp target | FY2026 Q1-Q2 | financial ramp of first HPC program | units, customer, optical content, yield |
| Coherent | $2B investment plus purchase/capacity rights | 2026-03 | financed capacity expansion | wafers/month, laser type, allocation |
| Lumentum | $2B investment plus purchase/capacity rights; new fab | 2026-03 | major new laser/optics capacity | location, tools, output date, yield |
| Corning | Meta up to $6B; Amazon multibillion agreement | 2026 | demand and NC expansion | fiber-km, connector units, pricing |
| GlobalFoundries | acquired Advanced Micro Foundry | 2025-11 | Singapore SiPh capability added | consolidated photonics wafer capacity |
| Jabil | acquired Intel SiPh product business | 2023 | product/manufacturing continuity | current module capacity and mix |

### SiPh Capacity
| Platform | Model | Visibility | Key Risk |
|---|---|---|---|
| Intel | captive/integrated R&D and technology | limited public detail | strategy and external access |
| GF Fotonix / AMF | open foundry plus Singapore capability | commercial; aggregate capacity undisclosed | customer ramp and packaging ecosystem |
| TSMC | advanced integration/COUPE roadmap | [TO VERIFY] production scope | allocation and process maturity |
| Tower | open foundry | commercial | scale and qualified design ecosystem |
| imec / CEA-Leti / AIM | R&D, pilot, technology transfer | program-based | transfer to HVM |

### Yield Disclosure Audit
| Layer | Comparable Numerical Yield Public? | Best Available Proxy | Required Metric |
|---|---|---|---|
| III-V epitaxy / laser die | no | gross margin, shortages, capacity investment | epi wafer yield; good die/wafer |
| SiPh wafer | no supplier-comparable set | qualification and MPW maturity | wafer-sort yield by process/PIC area |
| DSP/SerDes | no optical-specific yield | advanced-node supply and margins | known-good die yield |
| Laser/PIC attach | no | ramp delays and assembly capex | first-pass attach yield; rework rate |
| Module calibration/test | no | test-time/capex commentary | first-pass yield; seconds/channel |
| CPO package | no | demonstration and shipment status | package yield; engine rework |
| Field reliability | no comparable set | warranty/RMA commentary | FIT, DPPM, annual failure rate |

### Lead-Time Assessment
| Item | 2026 Assessment | Evidence Quality |
|---|---|---|
| 800G modules | selected suppliers appear demand constrained; allocations likely | MED, earnings/channel evidence |
| 1.6T modules | qualification/early ramp; 200G/lane components dominate schedule | MED, roadmap evidence |
| advanced lasers | strategic agreements imply scarcity | HIGH inference from disclosed investments |
| SiPh foundry | expanding through GF/AMF and other programs | MED; numerical capacity unavailable |
| fiber/connectivity | hyperscaler agreements driving US expansion | HIGH, contractual evidence |
| test equipment | transition supports demand; exact lead time undisclosed | LOW/MED |

### Ramp Stage Definitions
| Stage | Required Evidence |
|---|---|
| Engineering sample | functional device; no production commitment |
| Customer sample | delivered for customer evaluation |
| Qualification | environmental, reliability, interoperability tests underway/passed |
| Low-volume manufacturing | repeatable line and customer-accepted shipments |
| HVM | stable yield, automated test, sustained accepted output and revenue |
| Constrained HVM | repeatable HVM exists but qualified demand exceeds supply |

### Technology Ramp Timeline
| Technology | Pilot | Low Volume | HVM Assessment | Key Bottleneck |
|---|---|---|---|---|
| 800G DR4/DR8 | 2022-2023 | 2023 | 2024-2026 | laser/PIC yield and test |
| 800G SR8 | 2022-2023 | 2023-2024 | 2024-2026 | VCSEL bandwidth/reliability |
| LPO 800G | 2023-2024 | 2024-2026E | [TO VERIFY] | host channel and interoperability |
| CPO 51.2T | 2022-2024 demos | limited customer deliveries | HVM volume undisclosed | package yield/serviceability |
| 1.6T DR8 | 2024-2025 samples | 2025-2026E | 2026-2027E | 200G/lane ecosystem |
| CPO 102.4T | 2024-2026 announcements/demos | 2026-2027E | 2027+ [LOW confidence] | engine, ELS, package/test |

### Supplier Data Request
| Metric | Unit | Frequency |
|---|---|---|
| Nameplate capacity | units/month or wafers/month | quarterly |
| Qualified capacity | customer-approved units/month | quarterly |
| Good-unit output | accepted units/month | monthly |
| First-pass yield | % | monthly |
| Rework recovery | % | monthly |
| Cycle time | days from wafer start to shipment | monthly |
| Quoted lead time | weeks by SKU | monthly |
| On-time delivery | % | monthly |
| Field failure | DPPM or FIT | quarterly |

### Geographic Concentration and Policy
| Region | Concentration | Risk |
|---|---|---|
| Taiwan | advanced CMOS, packaging, emerging SiPh | geopolitics and allocation |
| China | module assembly and optical suppliers | export controls, tariffs, customer restrictions |
| US | fabless DSP, SiPh IP, compound-semiconductor assets | cost and specialized capacity |
| Japan | lasers, materials, precision components | supplier concentration |
| Southeast Asia | contract manufacturing | logistics and geographic concentration |
| Europe | research institutes and equipment | HVM technology transfer |

US CHIPS programs may support domestic packaging, SiPh, and compound semiconductors, but award-specific photonics capacity must be verified. Export-control details are maintained in [19_regulatory_and_standards_bodies.md](19_regulatory_and_standards_bodies.md).

## Data Tables (where applicable)
| Field | Value | Source | Date |
|---|---|---|---|
| AAOI 800G target | 100k modules/month | AAOI coverage | 2025 year-end |
| AAOI US production target | ~35% | AAOI coverage | 2025 |
| Fabrinet FY26 Q2 revenue | $1.13B | Fabrinet | 2026-02 |
| Fabrinet FY26 Q2 HPC revenue | $85.6M | Fabrinet | 2026-02 |
| NVIDIA supplier investments | $2B each to Coherent and Lumentum | company coverage | 2026-03 |

## Open Questions / Gaps
- Confirm whether AAOI achieved 100k/month and identify DR4/DR8/2xFR4 mix.
- Obtain Coherent/Lumentum fab locations, tool schedules, and qualified output.
- Quantify GF/AMF, TSMC, Intel, and Tower photonics wafer capacity.
- Obtain first-pass yield, rework, cycle time, and field failure under NDA.
- Build a monthly lead-time survey across lasers, DSPs, PICs, modules, connectors, and test equipment.

## References
- AAOI capacity coverage | https://www.investors.com/news/technology/applied-optoelectronics-stock-aaoi-applied-optoelectronics-earnings-q32025/ | 2026-06-09
- Fabrinet ramp coverage | https://www.investors.com/research/the-new-america/fabrinet-stock-fn/ | 2026-06-09
- NVIDIA supplier agreements | https://www.wsj.com/tech/ai/nvidia-to-invest-2-billion-in-both-lumentum-and-coherent-b047f619 | 2026-06-09
- Meta-Corning agreement | https://www.wsj.com/tech/meta-enters-up-to-6-billion-data-center-fiber-optic-cable-deal-with-corning-4a085f73 | 2026-06-09
- Amazon-Corning agreement | https://www.wsj.com/tech/amazon-enters-agreement-with-corning-for-optical-fiber-for-data-centers-352c7fa7 | 2026-06-09
- GlobalFoundries Fotonix | https://gf.com/technology-platforms/fotonix/ | 2026-06-09
- AIM Photonics | https://www.aimphotonics.com/ | 2026-06-09