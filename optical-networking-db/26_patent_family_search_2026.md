# Patent Family Search 2026
> **Last Updated:** 2026-06-09
> **Status:** In Review
> **Tags:** patents, Google-Patents, patent-families, assignee-normalization, FTO

## Overview
This file converts [12_patents_ip_landscape.md](12_patents_ip_landscape.md) from a qualitative placeholder into a reproducible search screen. The search used Google Patents' assignee filter and exact-phrase categories, then recorded the returned family-clustered result count and family status metadata.

These are search-result counts, not audited legal portfolio counts. Assignee spelling, translations, acquisitions, title/abstract wording, continuations, and false positives affect the result. The output is suitable for competitive screening and query refinement, not freedom-to-operate conclusions.

> ⚠️ Note: “Coherent” is both a company name and a technical adjective. The assignee filter reduces but may not eliminate ambiguity. Counsel should reproduce high-risk searches in Lens, Derwent, PatSnap, Orbit, or an equivalent family-normalized database.

## Key Findings / Highlights
- [CONFIRMED] Intel produced the largest bounded “silicon photonics” result set in this screen: 694 results [Source: Google Patents query, 2026-06-09].
- [CONFIRMED] Cisco/Acacia was strong across silicon photonics, coherent optics, and CPO phrase searches: 113, 42, and 28 results respectively.
- [CONFIRMED] Lumentum returned 51 silicon-photonics and 54 coherent-optical results, consistent with its integrated laser/coherent portfolio.
- [CONFIRMED] NVIDIA's exact “co-packaged optics” result set was small but emerging at seven results; keyword counts understate broader package/interconnect claims.
- [ESTIMATED] The highest practical FTO density remains fiber coupling, III-V integration, ring control, DSP/carrier recovery, and optical-engine packaging [MED confidence].

## Detailed Content
### Query Definition v1.0
| Category | Exact Phrase | Google Patents Filter |
|---|---|---|
| Silicon photonics | `"silicon photonics"` | `assignee=<normalized name>` |
| Coherent optical | `"coherent optical"` | `assignee=<normalized name>` |
| Co-packaged optics | `"co-packaged optics"` | `assignee=<normalized name>` |

URL pattern:

```text
https://patents.google.com/xhr/query?url=assignee%3D<ASSIGNEE>%26q%3D<ENCODED_EXACT_PHRASE>&exp=
```

### Search Results
| Ultimate Parent Search Name | Silicon Photonics | Coherent Optical | Co-Packaged Optics | Interpretation |
|---|---:|---:|---:|---|
| Intel | 694 | 41 | 32 | broad historic SiPh integration and packaging portfolio |
| Cisco | 113 | 42 | 28 | includes Acacia/Lightwire-related technology but alias merge is incomplete |
| Broadcom | 2 | 9 | 4 | exact phrases substantially undercount SerDes/package claims |
| NVIDIA | 6 | 1 | 7 | growing CPO footprint; Mellanox aliases not fully merged |
| Coherent | 12 | 28 | 0 | exact company-name ambiguity and former II-VI aliases limit result |
| Lumentum | 51 | 54 | 3 | strong laser, coherent, and SiPh-related set |
| GlobalFoundries | 55 | 5 | 0 | foundry/process portfolio; AMF acquisition not yet fully reflected |

### Acquisition-Aware Parent Map
| Current Parent | Aliases / Acquired Assignees to Add in v2 |
|---|---|
| Cisco | Acacia Communications, Lightwire, Luxtera |
| NVIDIA | Mellanox Technologies, Mellanox Technologies Denmark |
| Coherent | II-VI, Finisar, Oclaro assets where assigned, Coherent Inc. |
| Lumentum | NeoPhotonics, JDS Uniphase/JDSU assets where assigned |
| Marvell [not yet queried] | Inphi, Avera Semiconductor |
| GlobalFoundries | Advanced Micro Foundry, IBM Microelectronics-assigned assets |
| AMD [not yet queried] | Enosemi |

### Why Exact-Phrase Counts Understate Portfolios
| Company | Under-count Mechanism |
|---|---|
| Broadcom | claims use optical engine, photonic interface, SerDes, package substrate, or near-package terminology |
| NVIDIA | Mellanox assignee names and recent unpublished applications |
| Coherent | legacy II-VI/Finisar assignees and “coherent” name ambiguity |
| Cisco | patents may remain assigned to Acacia/Luxtera/Lightwire legal entities |
| foundries | process claims may omit application phrase “silicon photonics” |

### v2 CPC/Keyword Expansion
| Risk Area | CPC / Keyword Direction | Purpose |
|---|---|---|
| Integrated photonics | G02B6/12, H01L optical integration subclasses | capture waveguides/PICs |
| Optical communications | H04B10/* | capture transmit/receive systems |
| Heterogeneous lasers | III-V, bonded laser, transfer printing, DFB-on-silicon | laser integration FTO |
| Fiber coupling | grating coupler, edge coupler, fiber attach, FAU | package/coupling FTO |
| Coherent DSP | carrier recovery, polarization demultiplexing, equalization, FEC | ZR/ZR+ FTO |
| CPO/NPO | optical engine, near-package, package substrate, external laser | terminology expansion |

### Portfolio Quality Scoring
| Factor | Weight | Measurement |
|---|---:|---|
| Active jurisdictions | 20% | US/EP/CN/JP/KR/TW active status |
| Remaining term | 15% | priority date and term adjustments |
| Independent-claim relevance | 30% | manual claim chart against target architecture |
| Forward citations | 10% | normalized by age/field |
| Family breadth | 10% | jurisdiction and continuation coverage |
| Product evidence | 15% | assignment/licensing and implementation evidence |

### Reproducibility Record
| Field | Value |
|---|---|
| Search date | 2026-06-09 |
| Search engine | Google Patents XHR query |
| Result unit | returned search result with family metadata; not independently deduplicated INPADOC family |
| Legal-status handling | family metadata exposes aggregated country status; full status not exported in v1 |
| Assignee handling | one current-parent string per query; aliases listed separately |
| Known limitation | no CPC expansion and no manual false-positive review |

## Data Tables (where applicable)
| Field | Value | Source | Date |
|---|---|---|---|
| Largest SiPh result set | Intel, 694 | Google Patents | 2026-06-09 |
| Largest coherent result set in sample | Lumentum, 54 | Google Patents | 2026-06-09 |
| Largest CPO result set in sample | Intel, 32 | Google Patents | 2026-06-09 |
| Cisco CPO result set | 28 | Google Patents | 2026-06-09 |
| NVIDIA CPO result set | 7 | Google Patents | 2026-06-09 |

## Open Questions / Gaps
- Run v2 with aliases, CPC classes, title/abstract/claims fields, and priority-date windows.
- Add Marvell/Inphi, IBM, TSMC, Tower, imec, Ayar Labs, Lightmatter, Ranovus, and university assignees.
- Export all results and deduplicate to INPADOC/simple families.
- Manually review independent claims for the top 20 active families per risk area.
- Add litigation, IPR, ITC, licensing, expiration, and standards-essential declarations.

## References
- Google Patents | https://patents.google.com/ | 2026-06-09
- USPTO Patent Center | https://patentcenter.uspto.gov/ | 2026-06-09
- WIPO Patentscope | https://patentscope.wipo.int/ | 2026-06-09
- EPO Espacenet | https://worldwide.espacenet.com/ | 2026-06-09
- The Lens | https://www.lens.org/ | 2026-06-09
