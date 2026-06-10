# Key Research Papers
> **Last Updated:** 2026-06-09
> **Status:** In Review
> **Tags:** bibliography, OFC, ECOC, IEEE-JLT, photonics, datacenter-networks

## Overview
This bibliography prioritizes work explaining datacenter optical architecture, integrated photonics, modulation, OCS, power efficiency, and novel fibers. Conference demonstrations, preprints, peer-reviewed archival papers, standards documents, and commercial products are kept distinct.

The 2025-2026 additions include 225-Gbaud PAM4/TFLN transmission, coherent CPO concepts, cross-layer optical chiplet optimization, and AI-fabric networking results. Preprints remain labeled as such until a final venue is verified.

> ⚠️ Note: arXiv papers are not necessarily peer reviewed. Verify authors, final venue, DOI, and revisions before formal citation.

## Key Findings / Highlights
- [CONFIRMED] Miller’s energy analyses remain foundational for optical-interconnect device and link requirements.
- [CONFIRMED] Google Jupiter publications provide rare production-scale OCS evidence.
- [CONFIRMED] A 2025 result reported net 3.2 Tb/s, 225-Gbaud PAM4 O-band IM/DD transmission using CMOS 3 nm SerDes and thin-film lithium-niobate modulators [Source: arXiv:2503.24147].
- [CONFIRMED] 2025-2026 preprints increasingly analyze coherent CPO and cross-layer optical chiplet/topology design.
- [ESTIMATED] Decision-useful research reports full-link energy, BER/FEC, thermal control, manufacturing assumptions, and failure behavior rather than isolated device records [HIGH confidence].

## Detailed Content
### 1. Silicon Photonics Fundamentals and Integration
| Title | Authors | Year | Venue | Key Finding | DOI/Link |
|---|---|---:|---|---|---|
| Silicon photonics | R. Soref | 2006 | IEEE JSTQE | early field overview and roadmap | https://doi.org/10.1109/JSTQE.2006.883151 |
| Silicon photonics: a review of recent literature | D. Thomson et al. | 2016 | Journal of Optics | broad device/integration review | https://doi.org/10.1088/2040-8978/18/7/073003 |
| Integrated photonics on silicon | D. Dai et al. | 2012 | Laser & Photonics Reviews | integrated waveguide/device survey | [TO VERIFY DOI] |
| 3D optoelectronics and co-packaged optics: when solving the wrong problems stalls deployment | Yi, Wilkerson | 2026 | arXiv perspective | argues that serviceability, standards, packaging, and thermals determine deployment | https://arxiv.org/abs/2603.21313 |

### 2. Co-Packaged Optics Architecture and Demonstrations
| Title | Authors | Year | Venue / Type | Key Finding | DOI/Link |
|---|---|---:|---|---|---|
| OIF Co-Packaging Framework Implementation Agreement | OIF | 2023 | Industry IA | CPO terminology and framework | https://www.oiforum.com/technical-work/hot-topics/co-packaging/ |
| C2PO: Coherent Co-packaged Optics using offset-QAM-16 for Beyond PAM-4 Optical I/O | Sturm et al. | 2025 | arXiv | modeled compact coherent CPO transmitter toward 400G/channel | https://arxiv.org/abs/2506.12160 |
| Silicon photonic switches and transceivers for CPO | multiple | 2020-2025 | JLT/OFC | switch-adjacent engine demonstrations | [TO CURATE exact papers] |

### 3. High-Speed Modulation: PAM4, PAM6, Coherent
| Title | Authors | Year | Venue / Type | Key Finding | DOI/Link |
|---|---|---:|---|---|---|
| 400ZR Implementation Agreement | OIF | 2020 | Industry IA | interoperable coherent DCI baseline | https://www.oiforum.com/technical-work/hot-topics/400zr-2/ |
| Net 3.2 Tbps 225 Gbaud PAM4 O-Band IM/DD 2 km Transmission Using FR8 and DR8 with a CMOS 3 nm SerDes and TFLN Modulators | St-Arnault et al. | 2025 | arXiv/OFC-era result | 3.2T/4.2T-class aggregate IM/DD demonstration | https://arxiv.org/abs/2503.24147 |
| Probabilistic constellation shaping for optical fiber communications | Buchali et al. and related work | 2015-2016 | JLT/ECOC | adaptive spectral-efficiency gains | [TO VERIFY canonical citation] |

### 4. Optical Circuit Switching in Datacenters
| Title | Authors | Year | Venue | Key Finding | DOI/Link |
|---|---|---:|---|---|---|
| Helios: A Hybrid Electrical/Optical Switch Architecture for Modular Data Centers | Farrington et al. | 2010 | SIGCOMM | hybrid packet/circuit switching | https://dl.acm.org/doi/10.1145/1851182.1851183 |
| c-Through: Part-time Optics in Data Centers | Wang et al. | 2010 | SIGCOMM | traffic-driven optical bypass | https://dl.acm.org/doi/10.1145/1851182.1851192 |
| Jupiter Evolving: Transforming Google’s Datacenter Network via Optical Circuit Switches and Software-Defined Networking | Google authors | 2022 | SIGCOMM | production OCS reconfiguration and evolution | https://research.google/pubs/jupiter-evolving-transforming-googles-datacenter-network-via-optical-circuit-switches-and-software-defined-networking/ |

### 5. Power Efficiency and Low-Power Photonics
| Title | Authors | Year | Venue | Key Finding | DOI/Link |
|---|---|---:|---|---|---|
| Device requirements for optical interconnects to silicon chips | D. A. B. Miller | 2009 | Proceedings of the IEEE | device and energy requirements | https://doi.org/10.1109/JPROC.2009.2014298 |
| Attojoule Optoelectronics for Low-Energy Information Processing and Communications | D. A. B. Miller | 2017 | JLT | fundamental energy scaling | https://doi.org/10.1109/JLT.2017.2647779 |
| Energy-efficient optical interconnects | multiple | 2019-2025 | JSSC/ISSCC/JLT | electronic-photonic link co-design | [TO CURATE] |

### 6. AI Fabrics and Cross-Layer Optimization
| Title | Authors | Year | Venue / Type | Key Finding | DOI/Link |
|---|---|---:|---|---|---|
| High-speed Networking for Giga-Scale AI Factories | Khashab et al. | 2026 | arXiv; vendor authors | Spectrum-X evaluation reports high line-rate utilization and failure behavior | https://arxiv.org/abs/2605.21187 |
| ChipLight: Cross-Layer Optimization of Chiplet Design with Optical Interconnects for LLM Training | Bai et al. | 2026 | arXiv | co-optimizes chiplets, parallelism, and optical topology | https://arxiv.org/abs/2604.18909 |
| Machine learning for optical network automation | multiple | 2018-2025 | JOCN/JLT | telemetry-driven prediction and control | [TO CURATE systematic review] |

### 7. Hollow-Core Fiber and Novel Fiber Types
| Title | Authors | Year | Venue | Key Finding | DOI/Link |
|---|---|---:|---|---|---|
| Hollow-core NANF low-loss communications work | Poletti group and collaborators | 2019-2025 | Nature Photonics/OFC | lower latency/nonlinearity potential; manufacturing remains limiting | [TO VERIFY canonical paper] |
| Hollow-core fiber reviews | multiple | 2020-2025 | Nature/Optica reviews | deployment and manufacturing tradeoffs | [TO CURATE] |

### 8. WDM and Wavelength Management at Scale
| Title | Authors | Year | Venue | Key Finding | DOI/Link |
|---|---|---:|---|---|---|
| Microring-based WDM silicon-photonic links | multiple | 2010-2025 | JSSC/JLT/OFC | dense WDM with thermal-control tradeoffs | [TO CURATE] |
| Comb sources for parallel optical interconnects | multiple | 2018-2025 | Nature Photonics/OFC | shared multi-wavelength source potential | [TO CURATE] |

### Evidence Classification
| Type | Treatment |
|---|---|
| peer-reviewed archival paper | preferred technical evidence; still check conditions and replication |
| conference paper/postdeadline result | current performance evidence; manufacturing generalization limited |
| preprint | retain with explicit non-peer-reviewed status |
| standards/IA | interoperability/specification evidence, not measured product performance |
| vendor-authored evaluation | useful system evidence; disclose conflict and methodology limits |

### Venue Priority
| Venue | Best Use |
|---|---|
| OFC / ECOC | latest component and system demonstrations |
| ISSCC / IEEE JSSC | circuit energy and implementation |
| IEEE JLT / JOCN | archival devices, systems, and networking |
| Nature Photonics / Optica | high-impact device and integration work |
| Hot Chips | product architecture disclosures |
| SIGCOMM / NSDI | datacenter network architecture and operations |

## Data Tables (where applicable)
| Field | Value | Source | Date |
|---|---|---|---|
| New 225-Gbaud PAM4 result | arXiv:2503.24147 | arXiv | 2025 |
| Coherent CPO concept | arXiv:2506.12160 | arXiv | 2025 |
| CPO deployment perspective | arXiv:2603.21313 | arXiv | 2026 |
| AI networking evaluation | arXiv:2605.21187 | arXiv | 2026 |
| Optical chiplet optimization | arXiv:2604.18909 | arXiv | 2026 |

## Open Questions / Gaps
- Replace preprints with final OFC/ECOC/JLT versions where published.
- Resolve placeholder rows to exact papers and DOIs.
- Add citation, replication, commercialization, and conflict-of-interest notes.
- Separate device records from production-feasible link results.
- Create BibTeX and machine-readable topic tags in `assets/`.

## References
- OFC | https://www.ofcconference.org/ | 2026-06-09
- ECOC | https://www.ecocexhibition.com/ | 2026-06-09
- IEEE Xplore | https://ieeexplore.ieee.org/ | 2026-06-09
- Optica Publishing Group | https://opg.optica.org/ | 2026-06-09
- ACM Digital Library | https://dl.acm.org/ | 2026-06-09
- Crossref | https://www.crossref.org/ | 2026-06-09
- arXiv links listed in tables | URLs above | 2026-06-09