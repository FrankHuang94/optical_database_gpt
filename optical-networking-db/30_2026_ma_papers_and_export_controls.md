# 2026 M&A, Papers, and Export Controls
> **Last Updated:** 2026-06-09
> **Status:** In Review
> **Tags:** M-and-A, research-papers, export-controls, BIS, 2026-refresh

## Overview
This file updates three fast-moving evidence sets: transaction status, new technical literature, and US export-control policy. It supplements [13_key_research_papers.md](13_key_research_papers.md), [19_regulatory_and_standards_bodies.md](19_regulatory_and_standards_bodies.md), and [20_investment_and_ma_tracker.md](20_investment_and_ma_tracker.md).

The principal correction is that HPE/Juniper and Nokia/Infinera are no longer pending transactions. The photonics M&A focus has shifted toward optical design software, SiPh foundry capacity, and optical scale-up fabrics.

> ⚠️ Note: Export-control requirements are legal, product-specific, and rapidly changing. This database is an issue tracker, not legal advice or an export-classification determination.

## Key Findings / Highlights
- [CONFIRMED] HPE completed its approximately $14B acquisition of Juniper Networks on July 2, 2025 after a US DOJ settlement [Source: HPE/DOJ transaction disclosures, 2025].
- [CONFIRMED] Nokia completed its approximately $2.3B Infinera acquisition in February 2025 [Source: Nokia transaction disclosures, 2025].
- [CONFIRMED] AMD acquired photonic-design company Enosemi on May 28, 2025 [Source: AMD, 2025].
- [CONFIRMED] GlobalFoundries acquired Advanced Micro Foundry in November 2025, adding Singapore SiPh foundry capacity [Source: GlobalFoundries, 2025-11-17].
- [CONFIRMED] The US rescinded the January 2025 AI Diffusion Rule before implementation and retained/modified separate advanced-computing and semiconductor controls [Source: BIS policy announcement, 2025-05].

## Detailed Content
### Transaction Status
| Date | Acquirer / Investor | Target | Value | Current Status | Optical Rationale |
|---|---|---|---:|---|---|
| 2025-02 | Nokia | Infinera | ~$2.3B EV announced | [CONFIRMED] completed | combines PSE/ICE coherent DSP, PIC, line-system portfolios |
| 2025-05-28 | AMD | Enosemi | undisclosed | [CONFIRMED] completed | photonic IC design tools/IP and optical-interconnect expertise |
| 2025-07-02 | HPE | Juniper Networks | ~$14B equity | [CONFIRMED] completed after DOJ settlement | AI/datacenter networking, Mist, switching/routing |
| 2025-11-17 | GlobalFoundries | Advanced Micro Foundry | undisclosed | [CONFIRMED] completed/announced acquisition | SiPh foundry scale in Singapore |
| 2025-12 [TO VERIFY] | Marvell | Celestial AI | ~$3B-class reported consideration [TO VERIFY] | announced; close status requires filing check | Photonic Fabric scale-up/scale-out IP |
| 2026-03 | NVIDIA | Coherent | $2B equity investment | [CONFIRMED] strategic investment, not acquisition | laser/optical capacity and product access |
| 2026-03 | NVIDIA | Lumentum | $2B equity investment | [CONFIRMED] strategic investment, not acquisition | laser capacity, new fab, future optics |

### HPE / Juniper Remedy Context
| Remedy | Purpose | Database Relevance |
|---|---|---|
| divest HPE Instant On wireless business | preserve WLAN competition | transaction condition, not optical-specific |
| license Juniper Mist AI source code | preserve innovation/competition | affects software/network integration |
| HPE Juniper Networking organization | combines portfolios | update systems-vendor ownership and ticker mapping |

### 2025-2026 Research Additions
| Title | Authors | Year | Venue / Type | Key Finding | Link |
|---|---|---:|---|---|---|
| Net 3.2 Tbps 225 Gbaud PAM4 O-Band IM/DD 2 km Transmission Using FR8 and DR8 with a CMOS 3 nm SerDes and TFLN Modulators | St-Arnault et al. | 2025 | arXiv/OFC-era result | demonstrated 3.2T/4.2T-class aggregate IM/DD with 225 Gbaud PAM4 and TFLN | https://arxiv.org/abs/2503.24147 |
| C2PO: Coherent Co-packaged Optics using offset-QAM-16 for Beyond PAM-4 Optical I/O | Sturm et al. | 2025 | arXiv | modeled compact coherent CPO transmitter path toward 400G/channel | https://arxiv.org/abs/2506.12160 |
| 3D optoelectronics and co-packaged optics: when solving the wrong problems stalls deployment | Yi, Wilkerson | 2026 | arXiv perspective | argues serviceability, standards, packaging, and thermals determine adoption | https://arxiv.org/abs/2603.21313 |
| High-speed Networking for Giga-Scale AI Factories | Khashab et al. | 2026 | arXiv / NVIDIA authors | Spectrum-X production evaluation reports 98% line rate and failure behavior | https://arxiv.org/abs/2605.21187 |
| ChipLight: Cross-Layer Optimization of Chiplet Design with Optical Interconnects for LLM Training | Bai et al. | 2026 | arXiv | co-optimizes chiplets, parallelism, and optical topology | https://arxiv.org/abs/2604.18909 |

> ⚠️ Note: arXiv entries may not be peer reviewed. Preserve venue and review status when importing citations.

### Export-Control Timeline
| Date | Action | Current Interpretation |
|---|---|---|
| 2022-10 onward | advanced-computing, supercomputer, and semiconductor-manufacturing controls | foundational PRC restrictions remain relevant |
| 2024-12 | additional semiconductor-manufacturing controls and Entity List changes | tightened equipment/technology restrictions |
| 2025-01 | AI Diffusion Rule issued | [DEPRECATED] as operative framework; later rescinded |
| 2025-04 | NVIDIA H20 and related China-oriented accelerators subjected to license requirements | direct AI-chip impact; optics affected indirectly through customer/system demand |
| 2025-05 | BIS announced rescission of AI Diffusion Rule and future replacement approach | country-tier diffusion framework did not take effect as planned |
| 2025-05 to 2025-07 | temporary EDA/software export restrictions and subsequent relaxation reported | demonstrates policy volatility for design ecosystem |
| 2026 | licensing policy continues to evolve by chip, destination, parent/end user, and end use | legal review required for every transaction |

### Optical-Supply-Chain Exposure
| Item | Potential Control Hook | Action |
|---|---|---|
| advanced DSP/SerDes | ECCN/performance thresholds and advanced-computing rules | classify SKU and destination |
| foundry tapeout/design data | technology/software export and deemed-export rules | screen access and personnel |
| high-end test equipment | CCL classification/end use | classify equipment and support |
| module shipment | module classification plus incorporated controlled chips | do not assume optics are uncontrolled |
| China customer/affiliate | Entity List, Military End User, ownership/affiliate guidance | screen ultimate parent and beneficial owner |
| cloud access | advanced-computing end-use/location rules | review service and remote-access controls |

### Compliance Dataset
| Required Field | Example |
|---|---|
| legal entity and aliases | supplier/customer/parent |
| ownership | direct and indirect percentages |
| restricted-list screening | Entity List, SDN, MEU and relevant lists |
| ECCN/HTS | product-level classification |
| destination/end use | fab, cloud, military, research |
| license exception/status | citation and expiration |
| rule effective date | preserve historical decisions |
| counsel approval | reviewer/date/document |

## Data Tables (where applicable)
| Field | Value | Source | Date |
|---|---|---|---|
| HPE/Juniper status | completed | HPE/DOJ | 2025-07-02 |
| Nokia/Infinera status | completed | Nokia | 2025-02 |
| AMD/Enosemi status | completed | AMD | 2025-05-28 |
| GF/AMF status | acquired | GlobalFoundries | 2025-11-17 |
| AI Diffusion Rule | rescinded before implementation | BIS | 2025-05 |

## Open Questions / Gaps
- Verify Marvell/Celestial AI signed value, regulatory status, and closing date from current filings.
- Add announcement-date revenue multiples for all transactions.
- Replace arXiv citations with final OFC/ECOC/JLT versions where published.
- Maintain a versioned BIS/Federal Register rules table and entity-screening export.
- Obtain legal review for product ECCNs and China subsidiary/affiliate treatment.

## References
- HPE Investor Relations | https://investors.hpe.com/ | 2026-06-09
- Nokia Investor Relations | https://www.nokia.com/about-us/investors/ | 2026-06-09
- AMD Newsroom | https://www.amd.com/en/newsroom.html | 2026-06-09
- GlobalFoundries Newsroom | https://gf.com/gf-press-release/ | 2026-06-09
- BIS | https://www.bis.gov/ | 2026-06-09
- Federal Register | https://www.federalregister.gov/agencies/industry-and-security-bureau | 2026-06-09
- Research links listed in paper table | URLs above | 2026-06-09
