# Patents and IP Landscape
> **Last Updated:** 2026-06-09
> **Status:** In Review
> **Tags:** patents, IP, patent-families, FTO, silicon-photonics, coherent-DSP

## Overview
Optical-networking IP spans device physics, DSP, packaging, thermal control, coupling, laser integration, test, and system control. Raw patent-publication counts are misleading because assignee names change through acquisitions, one invention may have many jurisdictional filings, and claim scope matters more than keyword frequency.

This section includes a reproducible first-pass Google Patents screen and the normalization method required for a legal-quality portfolio analysis. Returned counts are bounded search results with family metadata, not audited INPADOC-family totals or freedom-to-operate conclusions.

> ⚠️ Note: “Coherent” is both a company name and a technical adjective. Counsel should reproduce high-risk searches in a family-normalized professional database and review independent claims, prosecution history, legal status, jurisdiction, and remaining term.

## Key Findings / Highlights
- [CONFIRMED] Intel returned 694 results in the bounded exact-phrase “silicon photonics” assignee screen [Source: Google Patents query, 2026-06-09].
- [CONFIRMED] Cisco returned 113 silicon-photonics, 42 coherent-optical, and 28 co-packaged-optics results; acquired aliases remain incompletely merged.
- [CONFIRMED] Lumentum returned 51 silicon-photonics and 54 coherent-optical results.
- [CONFIRMED] NVIDIA returned seven exact “co-packaged optics” results; recent/unpublished applications and Mellanox aliases may understate the portfolio.
- [ESTIMATED] Highest practical FTO density remains III-V integration, fiber coupling, ring control, coherent DSP/FEC, and optical-engine packaging [MED confidence].

## Detailed Content
### Query Definition v1.0
| Category | Exact Phrase | Filter |
|---|---|---|
| Silicon photonics | `"silicon photonics"` | `assignee=<normalized name>` |
| Coherent optical | `"coherent optical"` | `assignee=<normalized name>` |
| Co-packaged optics | `"co-packaged optics"` | `assignee=<normalized name>` |

```text
https://patents.google.com/xhr/query?url=assignee%3D<ASSIGNEE>%26q%3D<ENCODED_EXACT_PHRASE>&exp=
```

### First-Pass Search Results
| Ultimate Parent Search Name | Silicon Photonics | Coherent Optical | Co-Packaged Optics | Interpretation |
|---|---:|---:|---:|---|
| Intel | 694 | 41 | 32 | broad historic SiPh integration and packaging portfolio |
| Cisco | 113 | 42 | 28 | Acacia/Lightwire/Luxtera aliases not fully merged |
| Broadcom | 2 | 9 | 4 | exact phrases materially undercount SerDes and package claims |
| NVIDIA | 6 | 1 | 7 | emerging CPO set; Mellanox aliases not fully merged |
| Coherent | 12 | 28 | 0 | company-name ambiguity and II-VI/Finisar aliases limit results |
| Lumentum | 51 | 54 | 3 | strong laser, coherent, and SiPh-related set |
| GlobalFoundries | 55 | 5 | 0 | foundry/process portfolio; AMF not fully reflected |

### Acquisition-Aware Parent Map
| Current Parent | Aliases / Acquired Assignees for v2 |
|---|---|
| Cisco | Acacia Communications, Lightwire, Luxtera |
| NVIDIA | Mellanox Technologies and subsidiaries |
| Coherent | II-VI, Finisar, Coherent Inc., assigned Oclaro assets |
| Lumentum | NeoPhotonics, JDS Uniphase/JDSU assets where assigned |
| Marvell | Inphi, Avera Semiconductor |
| GlobalFoundries | Advanced Micro Foundry, assigned IBM Microelectronics assets |
| AMD | Enosemi |

### Why Exact-Phrase Counts Understate Portfolios
| Company | Under-count Mechanism |
|---|---|
| Broadcom | claims may use optical engine, photonic interface, SerDes, package substrate, or near-package terms |
| NVIDIA | Mellanox assignees and recent unpublished applications |
| Coherent | legacy II-VI/Finisar assignees and name ambiguity |
| Cisco | patents may remain assigned to Acacia, Luxtera, or Lightwire entities |
| foundries | process claims may omit the application phrase “silicon photonics” |

### v2 CPC and Keyword Expansion
| Risk Area | CPC / Keyword Direction | Purpose |
|---|---|---|
| Integrated photonics | G02B6/12 and optical-integration subclasses | waveguides and PICs |
| Optical communications | H04B10/* | transmit/receive systems |
| Heterogeneous lasers | III-V, bonded laser, transfer printing, DFB-on-silicon | laser-integration FTO |
| Fiber coupling | grating coupler, edge coupler, fiber attach, FAU | package/coupling FTO |
| Coherent DSP | carrier recovery, polarization demux, equalization, FEC | ZR/ZR+ FTO |
| CPO/NPO | optical engine, near-package, substrate, external laser | terminology expansion |

### Normalization Method
1. Define bounded keywords, CPC classes, claim fields, and priority-date windows.
2. Export simple/INPADOC patent families rather than raw publications.
3. Normalize acquired assignees to current parent while retaining filing-date ownership.
4. Separate active, expired, abandoned, and pending rights by jurisdiction.
5. Score family quality using independent-claim relevance, term, jurisdictions, citations, and product evidence.
6. Manually claim-chart the top active families against a defined product architecture.

### Portfolio Quality Scoring
| Factor | Weight | Measurement |
|---|---:|---|
| Independent-claim relevance | 30% | manual claim chart against target product |
| Active jurisdictions | 20% | active US/EP/CN/JP/KR/TW rights |
| Remaining term | 15% | priority date and term adjustments |
| Product evidence | 15% | assignment, licensing, implementation |
| Forward citations | 10% | normalized by age and field |
| Family breadth | 10% | jurisdictions and continuation coverage |

### FTO Risk Areas
| Area | Why Risk Is Elevated | Mitigation |
|---|---|---|
| III-V-on-silicon lasers | dense incumbent and startup portfolios | product-specific design-around/license review |
| Fiber-to-chip coupling | geometry and alignment claims | claim-chart exact coupler and assembly |
| Ring tuning/control | thermal feedback and calibration IP | review circuits and firmware |
| Coherent DSP/FEC | algorithm and standards overlap | standards/IP counsel review |
| CPO packaging | multi-die, fiber, and laser architecture claims | teardown and package claim mapping |

### Reproducibility Record
| Field | Value |
|---|---|
| Search date | 2026-06-09 |
| Search engine | Google Patents XHR query |
| Result unit | returned result with family metadata; not independently deduplicated INPADOC family |
| Legal status | aggregated metadata only; full status not exported in v1 |
| Assignee handling | one parent string per query; aliases listed separately |
| Known limitation | no CPC expansion or manual false-positive review |

### Open-Source / Shared Ecosystem
| Project | Contribution | IP Caveat |
|---|---|---|
| AIM Photonics PDK | process access and education | PDK license governs use |
| SiEPIC | design automation and education | component/process licenses vary |
| gdsfactory | open-source photonic layout | PDK and IP blocks may be proprietary |
| OpenROAD | electronic design automation | indirect relevance to photonics |

## Data Tables (where applicable)
| Field | Value | Source | Date |
|---|---|---|---|
| Largest SiPh result set | Intel, 694 | Google Patents | 2026-06-09 |
| Largest coherent set in sample | Lumentum, 54 | Google Patents | 2026-06-09 |
| Largest CPO set in sample | Intel, 32 | Google Patents | 2026-06-09 |
| Cisco CPO set | 28 | Google Patents | 2026-06-09 |
| NVIDIA CPO set | 7 | Google Patents | 2026-06-09 |

## Open Questions / Gaps
- Run v2 with aliases, CPC classes, claims fields, and date windows.
- Add Marvell/Inphi, IBM, TSMC, Tower, imec, Ayar, Lightmatter, Ranovus, and university assignees.
- Export and deduplicate results into true patent families.
- Review independent claims for the top 20 active families per risk area.
- Add litigation, IPR, ITC, licensing, expiration, and standards-essential declarations.

## References
- Google Patents | https://patents.google.com/ | 2026-06-09
- USPTO Patent Center | https://patentcenter.uspto.gov/ | 2026-06-09
- WIPO Patentscope | https://patentscope.wipo.int/ | 2026-06-09
- EPO Espacenet | https://worldwide.espacenet.com/ | 2026-06-09
- The Lens | https://www.lens.org/ | 2026-06-09
- gdsfactory | https://gdsfactory.github.io/gdsfactory/ | 2026-06-09