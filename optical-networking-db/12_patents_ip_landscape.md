# Patents and IP Landscape
> **Last Updated:** 2026-06-09
> **Status:** Draft
> **Tags:** patents, IP, FTO, silicon-photonics, coherent-DSP

## Overview
Optical-networking IP spans device physics, circuit design, DSP algorithms, packaging, thermal tuning, fiber coupling, laser integration, test, and control. Raw patent counts are misleading because assignee names change through acquisition, one invention may create many jurisdictional filings, and claim scope matters more than document count.

This file defines a normalized search framework and identifies likely leaders. It does not provide legal advice or a freedom-to-operate (FTO) opinion; an FTO assessment requires claim charts, prosecution history, jurisdiction, expiration, and product-specific counsel.

> 🔄 Refresh Needed: High Priority — run reproducible Lens/Google Patents/USPTO queries and normalize patent families by ultimate parent.

## Key Findings / Highlights
- [CONFIRMED] Intel has a long silicon-photonics patent history covering waveguides, modulators, coupling, and integration.
- [CONFIRMED] Cisco’s Acacia acquisition consolidated significant coherent DSP and module IP.
- [CONFIRMED] Broadcom holds extensive SerDes, switch ASIC, and high-speed I/O portfolios relevant to CPO.
- [CONFIRMED] Coherent/II-VI and Lumentum portfolios cover III-V lasers, modulators, materials, and packaging.
- [ESTIMATED] Highest FTO risk concentrates at heterogeneous laser integration, low-loss coupling/alignment, ring control, coherent DSP/FEC, and package-level optical interfaces.

## Detailed Content
### Indicative Holder Matrix
| Company / Parent | SiPh Patents | Coherent DSP Patents | Transceiver / Packaging Patents | Filing Trend (YoY) |
|---|---:|---:|---:|---|
| Intel | [TO QUERY] high | [TO QUERY] medium | [TO QUERY] high | [TO QUERY] |
| Cisco / Acacia | high | high | high | [TO QUERY] |
| Broadcom | high | medium | high | [TO QUERY] |
| NVIDIA / Mellanox | medium-growing | low-medium | medium-growing | [TO QUERY] likely rising |
| Coherent / II-VI | medium-high | medium | high | [TO QUERY] |
| Lumentum / NeoPhotonics assets | medium | medium | high | [TO QUERY] |
| IBM | high historical | medium | medium | [TO QUERY] |
| GlobalFoundries | medium-growing | low | medium | [TO QUERY] |
| imec / university ecosystem | high publications/patents | low | medium | [TO QUERY] |

> ⚠️ Note: Counts are intentionally blank until family-level queries are run. Filling them with keyword-result totals would create false precision.

### Patent Families to Track
| Owner | Theme | Example Search Concepts | Strategic Relevance |
|---|---|---|---|
| Intel | SiPh waveguides/modulators/coupling | silicon photonic, grating coupler, hybrid laser | transceiver/CPO implementation |
| Cisco/Acacia | coherent DSP/modulation | carrier recovery, polarization, probabilistic shaping | ZR/ZR+ performance |
| Broadcom | SerDes/CPO interfaces | high-speed equalization, optical engine package | switch-to-optics integration |
| NVIDIA/Mellanox | optical switch/package | co-packaged optical switch, photonic interconnect | AI networking |
| Coherent/Lumentum | III-V lasers/modulators | EML, DFB, quantum dot, InP integration | light source supply |
| Startups | optical I/O/packaging | WDM chiplet, detachable coupler, microLED link | acquisition/FTO diligence |

### Search and Normalization Method
1. Define CPC classes and bounded keyword queries.
2. Export INPADOC/simple patent families, not raw publications.
3. Normalize acquired assignees to ultimate parent while preserving filing-date ownership.
4. Separate active, expired, abandoned, and pending rights.
5. Score family quality by forward citations, jurisdiction coverage, claim breadth, and remaining term.
6. Manually review independent claims for high-risk architecture features.

### Litigation and Licensing Baseline
| Matter | Parties / Area | Status |
|---|---|---|
| Optical component patent disputes | Finisar/II-VI/Lumentum and industry peers historically | [TO RESEARCH case-level] |
| Coherent DSP licensing | standards-essential and proprietary implementations | [TO RESEARCH] |
| SiPh foundry/IP licensing | PDK and platform agreements | often confidential |
| ITC import cases | optical modules/components | [TO RESEARCH docket-level] |

### FTO Risk Areas
| Area | Why Risk Is Elevated | Mitigation |
|---|---|---|
| III-V-on-silicon lasers | dense legacy and startup portfolios | design-around + license review |
| Fiber-to-chip coupling | geometry and alignment claims | claim chart specific coupler |
| Ring tuning/control | thermal feedback and calibration IP | firmware/circuit review |
| Coherent DSP/FEC | algorithm and standards overlap | standards/IP counsel |
| CPO packaging | multi-die/fiber/laser architecture claims | package teardown and claim mapping |

### Open-Source / Shared Ecosystem
| Project | Contribution | IP Caveat |
|---|---|---|
| AIM Photonics PDK | process design access and education | PDK license governs use |
| SiEPIC | design automation and education | component/process licenses vary |
| gdsfactory | open-source photonic layout tooling | PDK/IP blocks may be proprietary |
| OpenROAD | electronic design automation | indirect to photonics |

## Data Tables (where applicable)
| Field | Value | Source | Date |
|---|---|---|---|
| Count unit | normalized patent family | database methodology | 2026-06-09 |
| Primary US source | USPTO Patent Center | USPTO | current |
| International source | WIPO Patentscope | WIPO | current |
| Legal status requirement | active/pending/expired/abandoned | FTO methodology | 2026-06-09 |
| Highest-risk categories | laser integration, coupling, DSP, CPO packaging | preliminary analysis | 2026-06-09 |

## Open Questions / Gaps
- Execute and publish reproducible query strings and CPC filters.
- Build acquisition-aware assignee mapping.
- Add litigation docket numbers, outcomes, and licensing terms where public.
- Identify standards-essential declarations relevant to Ethernet/coherent optics.
- Commission product-specific FTO review before commercial use.

## References
- USPTO Patent Center | https://patentcenter.uspto.gov/ | 2026-06-09
- Google Patents | https://patents.google.com/ | 2026-06-09
- WIPO Patentscope | https://patentscope.wipo.int/ | 2026-06-09
- The Lens | https://www.lens.org/ | 2026-06-09
- EPO Espacenet | https://worldwide.espacenet.com/ | 2026-06-09
- gdsfactory | https://gdsfactory.github.io/gdsfactory/ | 2026-06-09
