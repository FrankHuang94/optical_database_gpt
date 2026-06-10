# Market Forecast Reconciliation
> **Last Updated:** 2026-06-09
> **Status:** In Review
> **Tags:** market-sizing, forecasts, LightCounting, Dell-Oro, Omdia, TAM

## Overview
This file addresses the mismatch between market forecasts by separating addressable-market scope, forecast object, units, and publication vintage. It supplements [16_market_sizing.md](16_market_sizing.md), whose initial ranges should be treated as scenario placeholders.

Licensed LightCounting, Dell'Oro, Omdia, Cignal AI, and IDTechEx tables were not available in the repository. The reconciliation therefore uses public statements and defines the exact fields required when licensed data is added. It does not reverse-engineer paywalled numbers from press coverage.

> ⚠️ Note: A $90B “optical TAM,” a datacenter-transceiver revenue forecast, AI back-end switch sales, and global datacenter capex are different markets and must never be added together.

## Key Findings / Highlights
- [CONFIRMED] Dell'Oro reported Ethernet represented roughly two-thirds of AI back-end network switch sales in 1Q 2026 [Source: Dell'Oro, 2026-06-02].
- [CONFIRMED] Dell'Oro's published roadmap expectation places majority AI back-end ports at 800G in 2026, 1.6T in 2027, and 3.2T in 2029 [Source: Dell'Oro commentary cited in ITPro, 2025].
- [CONFIRMED] Omdia forecast global datacenter investment approaching $1.6T by 2030 and more than $600B of 2026 deployment by leading technology enterprises [Source: Omdia, 2026-05-28].
- [CONFIRMED] Lumentum management presented a broad optical TAM reaching approximately $90B by 2030, implying about 40% CAGR from 2025 [Source: Lumentum OFC investor briefing reported by IBD, 2026-03-19].
- [ESTIMATED] Finished datacenter transceivers remain a materially smaller subset than the $90B broad optical-content TAM [HIGH confidence].

## Detailed Content
### Forecast Evidence Register
| Source | Metric | Base / Forecast | Scope | Public Value | Confidence |
|---|---|---|---|---:|---|
| Dell'Oro | AI back-end switch sales by protocol | 1Q 2026 actual | Ethernet + InfiniBand switches | Ethernet ~two-thirds | [HIGH] public release |
| Dell'Oro | dominant port speed | 2026/2027/2029 forecast | AI back-end network switch ports | 800G / 1.6T / 3.2T | [MED] public summary |
| Omdia | global datacenter investment | 2030 forecast | facilities + infrastructure; broader than networking | ~$1.6T | [MED] public release; definition needed |
| Omdia | leading technology-enterprise deployment | 2026 forecast | AI infrastructure investment | >$600B | [MED] public release |
| Lumentum | optical TAM | 2030 management TAM | broad photonics/optical opportunity | ~$90B; ~40% 2025-30 CAGR | [MED] company-defined TAM |
| LightCounting | Ethernet transceiver units/revenue | licensed | finished modules by speed/reach | [LICENSED DATA REQUIRED] | unavailable |
| Cignal AI/Omdia | coherent pluggables | licensed | ZR/ZR+/transport | [LICENSED DATA REQUIRED] | unavailable |
| IDTechEx | SiPh/CPO | licensed | components/platforms | [LICENSED DATA REQUIRED] | unavailable |

### Scope Hierarchy
| Level | Included | Excluded / Overlap Warning |
|---|---|---|
| Global datacenter investment | buildings, power, cooling, compute, network | not an optics TAM |
| Networking systems | switches, routers, NICs, optical transport | contains optics but mostly system value |
| Optical interconnect TAM | lasers, PICs, DSPs, modules, fiber/connectivity | components can be counted inside modules |
| Finished transceivers | pluggable and embedded optical modules | excludes external fiber and host systems |
| Datacenter transceivers | Ethernet/InfiniBand/DCI subset | define whether coherent DCI and AOCs are included |
| CPO/optical I/O | engines, chiplets, lasers, packages | may displace rather than add to pluggables |

### Reconciled Scenario Frame
| Segment | 2026 Direction | 2030 Treatment | Evidence Rule |
|---|---|---|---|
| 800G datacenter pluggables | volume growth; dominant AI port speed | matures and faces ASP erosion | unit x ASP model required |
| 1.6T pluggables | qualification/early ramp | major replacement generation | align with 102.4T switch shipments |
| 3.2T | standards/R&D | early deployment around 2029 is plausible | no near-term revenue in base case without product evidence |
| CPO/NPO | early systems and design wins | scenario-sensitive adoption | model substitution against pluggables |
| Coherent 800ZR/1600ZR | 800ZR ecosystem build | DCI growth and 1.6T transition | separate modules from line systems |
| Fiber/connectivity | capacity expansion | benefits from port/fiber-count growth | do not count within module ASP |

### Database Base/Bull/Bear Rules
| Scenario | 2026-2030 Assumption | Required Trigger |
|---|---|---|
| Bear | aggressive ASP erosion; delayed 1.6T/CPO | AI capex digestion or qualification delays |
| Base | 800G volume, 1.6T broad ramp from 2027, limited CPO | Dell'Oro speed sequence and vendor shipments |
| Bull | high optical endpoints per accelerator; CPO adds content | 100K+ accelerator deployments and disclosed HVM capacity |

### Licensed Data Intake Template
| Required Field | Example |
|---|---|
| Report/source | LightCounting Ethernet Optics |
| Publication vintage | 2H 2026 |
| Geography | worldwide |
| Product boundary | modules only; excludes AOC |
| Datacom/telecom split | explicit |
| Actual/estimate years | 2025A / 2026E-2031E |
| Units and revenue | units, ASP, $M |
| Speed/reach/form factor | 400G DR4, 800G DR8, etc. |
| Revision history | prior forecast and delta |

## Data Tables (where applicable)
| Field | Value | Source | Date |
|---|---|---|---|
| Ethernet share of AI back-end switch sales | ~two-thirds | Dell'Oro | 1Q 2026 |
| Majority speed sequence | 800G / 1.6T / 3.2T | Dell'Oro | 2026 / 2027 / 2029E |
| Global datacenter investment | approaches $1.6T | Omdia | 2030E |
| 2026 leading-enterprise investment | >$600B | Omdia | 2026E |
| Broad optical TAM | ~$90B | Lumentum management | 2030E |

## Open Questions / Gaps
- Purchase/import licensed transceiver unit and revenue tables.
- Resolve whether Lumentum's $90B TAM includes switching silicon, fiber, packaging, and compute optics.
- Build speed/reach unit x ASP forecasts with actual 2025A and 2026 quarterly data.
- Reconcile CPO as substitution versus incremental optical content.
- Archive every forecast vintage to measure forecast error.

## References
- Dell'Oro News Room | https://www.delloro.com/news/ | 2026-06-09
- Dell'Oro speed roadmap coverage | https://www.itpro.com/infrastructure/networking/why-networking-is-just-as-important-as-compute-in-ai-data-centers | 2026-06-09
- Omdia Newsroom | https://omdia.tech.informa.com/pr | 2026-06-09
- Lumentum OFC TAM coverage | https://www.investors.com/news/technology/lumentum-stock-lite-ofc-nvidia-gtc-optical-demand/ | 2026-06-09
- LightCounting | https://www.lightcounting.com/ | 2026-06-09
