# Key Research Papers
> **Last Updated:** 2026-06-09
> **Status:** Draft
> **Tags:** bibliography, OFC, ECOC, IEEE-JLT, photonics, datacenter-networks

## Overview
This bibliography prioritizes papers and technical reports that explain datacenter optical architecture, integrated photonics, modulation, OCS, energy efficiency, and novel fibers. Conference demonstrations should be separated from peer-reviewed archival results and commercial products.

Titles and links below provide a seed set. Bibliographic metadata and DOI values must be checked against IEEE Xplore, Optica, ACM Digital Library, Crossref, or publisher records before citation in formal research.

> 🔄 Refresh Needed: High Priority — add 2025-2026 OFC, ECOC, ISSCC, Hot Chips, JLT, JSSC, Nature Photonics, and Optica results.

## Key Findings / Highlights
- [CONFIRMED] Miller’s energy-attojoule analysis is foundational for optical interconnect energy limits.
- [CONFIRMED] Google Jupiter publications provide rare production-scale datacenter network evidence.
- [CONFIRMED] SiPh integration literature emphasizes packaging and laser integration alongside device performance.
- [CONFIRMED] OCS research repeatedly finds reconfiguration time and traffic predictability central to utility.
- [ESTIMATED] The most decision-useful papers report full-link energy, BER/FEC, thermal control, and manufacturing assumptions rather than isolated device records.

## Detailed Content
### 1. Silicon Photonics Fundamentals and Integration
| Title | Authors | Year | Venue | Key Finding | DOI/Link |
|---|---|---:|---|---|---|
| Silicon photonics | R. Soref | 2006 | IEEE JSTQE | early field overview and roadmap | https://doi.org/10.1109/JSTQE.2006.883151 |
| Silicon photonics: a review of recent literature | D. Thomson et al. | 2016 | Journal of Optics | broad device/integration review | https://doi.org/10.1088/2040-8978/18/7/073003 |
| Integrated photonics on silicon | D. Dai et al. | 2012 | Laser & Photonics Reviews | integrated waveguide/device survey | [TO VERIFY DOI] |

### 2. Co-Packaged Optics Architecture and Demonstrations
| Title | Authors | Year | Venue | Key Finding | DOI/Link |
|---|---|---:|---|---|---|
| Co-packaged optics: all eyes on high-speed I/O | industry authors | 2022-2024 | OFC tutorials | system drivers and packaging challenges | https://opg.optica.org/conference.cfm?conference=OFC |
| OIF Co-Packaging Framework Implementation Agreement | OIF | 2023 | Industry IA | terminology and framework | https://www.oiforum.com/technical-work/hot-topics/co-packaging/ |
| Silicon photonic switches and transceivers for CPO | multiple | 2020-2024 | JLT/OFC | demonstrations of switch-adjacent engines | [TO CURATE exact papers] |

### 3. High-Speed Modulation: PAM4, PAM6, Coherent
| Title | Authors | Year | Venue | Key Finding | DOI/Link |
|---|---|---:|---|---|---|
| 400ZR Implementation Agreement | OIF | 2020 | Industry IA | interoperable coherent DCI baseline | https://www.oiforum.com/technical-work/hot-topics/400zr-2/ |
| High-speed PAM4 optical interconnect demonstrations | multiple | 2018-2024 | OFC/ECOC/JLT | equalization/FEC enable 100G+ lanes | [TO CURATE] |
| Probabilistic constellation shaping for optical fiber communications | F. Buchali et al. and related authors | 2015-2016 | JLT/ECOC | adaptive spectral-efficiency gains | [TO VERIFY canonical citation] |

### 4. Optical Circuit Switching in Datacenters
| Title | Authors | Year | Venue | Key Finding | DOI/Link |
|---|---|---:|---|---|---|
| Helios: A Hybrid Electrical/Optical Switch Architecture for Modular Data Centers | N. Farrington et al. | 2010 | SIGCOMM | hybrid packet/circuit switching | https://dl.acm.org/doi/10.1145/1851182.1851183 |
| c-Through: Part-time Optics in Data Centers | G. Wang et al. | 2010 | SIGCOMM | traffic-driven optical bypass | https://dl.acm.org/doi/10.1145/1851182.1851192 |
| Jupiter Evolving: Transforming Google’s Datacenter Network via Optical Circuit Switches and Software-Defined Networking | Google authors | 2022 | SIGCOMM | production OCS reconfiguration and evolution | https://research.google/pubs/jupiter-evolving-transforming-googles-datacenter-network-via-optical-circuit-switches-and-software-defined-networking/ |

### 5. Power Efficiency and Low-Power Photonics
| Title | Authors | Year | Venue | Key Finding | DOI/Link |
|---|---|---:|---|---|---|
| Device requirements for optical interconnects to silicon chips | D. A. B. Miller | 2009 | Proceedings of the IEEE | energy and device requirement framework | https://doi.org/10.1109/JPROC.2009.2014298 |
| Attojoule Optoelectronics for Low-Energy Information Processing and Communications | D. A. B. Miller | 2017 | JLT | fundamental energy scaling | https://doi.org/10.1109/JLT.2017.2647779 |
| Energy-efficient optical interconnects | multiple | 2019-2024 | JSSC/ISSCC/JLT | link-level electronic-photonic co-design | [TO CURATE] |

### 6. AI/ML for Network Optimization and Fault Detection
| Title | Authors | Year | Venue | Key Finding | DOI/Link |
|---|---|---:|---|---|---|
| Machine learning for optical network automation | multiple | 2018-2024 | JOCN/JLT | telemetry-driven prediction and control | [TO CURATE systematic review] |
| Deep learning for optical performance monitoring | multiple | 2017-2024 | OFC/JLT | impairment classification from receiver data | [TO CURATE] |

### 7. Hollow-Core Fiber and Novel Fiber Types
| Title | Authors | Year | Venue | Key Finding | DOI/Link |
|---|---|---:|---|---|---|
| Hollow core NANF with low loss in telecom bands | F. Poletti group and collaborators | 2019-2024 | Nature Photonics/OFC | approaching conventional-fiber loss with lower latency/nonlinearity potential | [TO VERIFY exact canonical paper] |
| Hollow-core optical fibre sensors and communications reviews | multiple | 2020-2024 | Nature Reviews/Optica | manufacturing and deployment tradeoffs | [TO CURATE] |

### 8. WDM and Wavelength Management at Scale
| Title | Authors | Year | Venue | Key Finding | DOI/Link |
|---|---|---:|---|---|---|
| Microring-based WDM silicon photonic links | multiple | 2010-2024 | JSSC/JLT/OFC | dense WDM with thermal-control tradeoffs | [TO CURATE] |
| Comb sources for massively parallel optical interconnects | multiple | 2018-2024 | Nature Photonics/OFC | shared multi-wavelength source potential | [TO CURATE] |

### Venue Priority
| Venue | Best Use |
|---|---|
| OFC / ECOC | latest system and component demonstrations |
| ISSCC / IEEE JSSC | electronic-photonic circuit energy and implementation |
| IEEE JLT / JOCN | archival devices, systems, and network analysis |
| Nature Photonics / Optica | high-impact device and integration research |
| Hot Chips | product architecture disclosures |
| SIGCOMM / NSDI | datacenter network architecture and operations |

## Data Tables (where applicable)
| Field | Value | Source | Date |
|---|---|---|---|
| Seed bibliography entries | 18 topic rows | initial curation | 2026-06-09 |
| Highest-priority venue | OFC | field relevance | annual |
| Architecture venue | SIGCOMM | ACM | annual |
| Core archival journal | IEEE JLT | IEEE/Optica | ongoing |
| DOI validation source | Crossref/publisher | editorial workflow | 2026-06-09 |

## Open Questions / Gaps
- Resolve all placeholder citations to exact papers and DOIs.
- Add citation counts and replication/commercialization notes.
- Separate record-setting device results from production-feasible links.
- Add 2025-2026 conference best papers by topic.
- Create BibTeX assets and machine-readable paper tags.

## References
- OFC | https://www.ofcconference.org/ | 2026-06-09
- ECOC | https://www.ecocexhibition.com/ | 2026-06-09
- IEEE Xplore | https://ieeexplore.ieee.org/ | 2026-06-09
- Optica Publishing Group | https://opg.optica.org/ | 2026-06-09
- ACM Digital Library | https://dl.acm.org/ | 2026-06-09
- Crossref | https://www.crossref.org/ | 2026-06-09
