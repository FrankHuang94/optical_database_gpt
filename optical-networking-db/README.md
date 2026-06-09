# Datacenter Optical Networking Knowledge Database
> **Last Updated:** 2026-06-09
> **Status:** Draft
> **Tags:** datacenter-optics, AI-infrastructure, silicon-photonics, transceivers, CPO, market-research

## Overview
This repository is an indexed research database for datacenter optical networking, with emphasis on AI/HPC fabrics, datacenter interconnect (DCI), Ethernet and InfiniBand scale-out networks, silicon photonics, high-speed transceivers, and emerging co-packaged optical I/O. Telecom long-haul is excluded except where coherent technology, component supply, standards, or vendor economics directly affect datacenter deployment.

The initial population is a structured baseline based on public information available primarily through early 2025. It is not investment advice. Financial, market-size, startup-funding, product-roadmap, patent-count, export-control, and post-2024 transaction data require validation against current primary sources before decision use.

> 🔄 Refresh Needed: High Priority — reconcile all 2025-2026 product, financial, standards, funding, and regulatory claims with current filings and official announcements.

## Key Findings / Highlights
- [CONFIRMED] Datacenter optics progressed from 400G volume deployment around 2020 to 800G AI-cluster deployment beginning in 2023, with 1.6T qualification activity expected around 2025-2026 [Source: IEEE 802.3 Ethernet Working Group; vendor announcements, 2023-2025].
- [CONFIRMED] The lane roadmap is moving from 100 Gb/s PAM4 electrical/optical lanes toward 200 Gb/s lanes under IEEE 802.3dj and OIF CEI-224G work [Source: IEEE 802.3dj; OIF, 2024].
- [ESTIMATED] AI scale-out fabrics are the largest near-term incremental demand driver for 800G and 1.6T datacenter transceivers [Source: LightCounting and vendor earnings commentary, 2024; MED confidence].
- [CONFIRMED] Power, thermal density, laser reliability, packaging yield, and serviceability are central constraints in the transition from pluggables to LPO, CPO, and optical I/O [Source: OIF and COBO technical work, 2023-2024].
- [CONFIRMED] Industry structure spans compound-semiconductor lasers, silicon-photonics foundries, DSP/SerDes silicon, module assembly, network systems, and hyperscaler deployment, creating multiple supply bottlenecks and integration points [Source: company filings, 2024].

## Detailed Content
### Quick Access
| Section | File | Status | Last Updated |
|---|---|---|---|
| Master index | README.md | Draft | 2026-06-09 |
| Executive summary | [00](00_executive_summary.md) | Draft | 2026-06-09 |
| Technology overview | [01](01_technology_overview.md) | Draft | 2026-06-09 |
| Technology roadmap | [02](02_tech_roadmap.md) | Draft | 2026-06-09 |
| Standards and MSAs | [03](03_standards_and_msa.md) | Draft | 2026-06-09 |
| Silicon photonics | [04](04_silicon_photonics.md) | Draft | 2026-06-09 |
| Transceiver form factors | [05](05_transceiver_form_factors.md) | Draft | 2026-06-09 |
| Co-packaged optics | [06](06_co_packaged_optics.md) | Draft | 2026-06-09 |
| Coherent vs direct detect | [07](07_coherent_vs_direct_detect.md) | Draft | 2026-06-09 |
| Hyperscalers | [08](08_vendors_hyperscalers.md) | Draft | 2026-06-09 |
| Component vendors | [09](09_vendors_components.md) | Draft | 2026-06-09 |
| Systems vendors | [10](10_vendors_systems.md) | Draft | 2026-06-09 |
| Startups watchlist | [11](11_startups_watchlist.md) | Draft | 2026-06-09 |
| Patents and IP | [12](12_patents_ip_landscape.md) | Draft | 2026-06-09 |
| Research papers | [13](13_key_research_papers.md) | Draft | 2026-06-09 |
| Production and supply chain | [14](14_production_ramp_supply_chain.md) | Draft | 2026-06-09 |
| Competitive landscape | [15](15_competitive_landscape.md) | Draft | 2026-06-09 |
| Market sizing | [16](16_market_sizing.md) | Draft | 2026-06-09 |
| Power and thermal | [17](17_power_and_thermal.md) | Draft | 2026-06-09 |
| AI datacenter architecture | [18](18_AI_datacenter_architecture.md) | Draft | 2026-06-09 |
| Regulation and standards bodies | [19](19_regulatory_and_standards_bodies.md) | Draft | 2026-06-09 |
| Investment and M&A | [20](20_investment_and_ma_tracker.md) | Draft | 2026-06-09 |

### Database Scope
| Included | Excluded unless directly relevant |
|---|---|
| Intra-datacenter links from rack to campus | Consumer optical interfaces |
| AI/HPC scale-up, scale-out, and scale-across | Residential access/PON |
| Ethernet, InfiniBand, RoCE, UEC, DCI | Subsea and long-haul telecom deployment |
| Pluggables, LPO, CPO, optical I/O, OCS | General semiconductor markets |
| Components, systems, hyperscalers, supply chain | Non-optical networking without architectural relevance |

### How to Use This Database
1. Treat `[CONFIRMED]` as supported by a cited primary or strong secondary source, not as permanently current.
2. Treat `[ESTIMATED]` and forecasts as model inputs; preserve assumptions and attach `[HIGH/MED/LOW confidence]`.
3. Treat `[RUMORED]` as unverified and unsuitable for valuation or procurement decisions.
4. Treat `[DEPRECATED]` as historical technology or superseded guidance.
5. Date every statistic by year or quarter and cite claims inline as `[Source: Organization, YYYY-MM-DD]`.
6. Prefer tables for structured comparisons and relative links for related analysis.
7. Use `> ⚠️ Note:` for caveats and `> 🔄 Refresh Needed:` for stale or fast-changing areas.

### Update Workflow
| Step | Requirement |
|---|---|
| Intake | Record source URL, publication date, access date, and source type |
| Validation | Prefer standards bodies, filings, patents, papers, and vendor product pages |
| Classification | Apply status and confidence tags |
| Integration | Update affected tables and cross-referenced sections |
| Review | Check units, periods, currency, definitions, and conflicting estimates |

## Data Tables (where applicable)
| Field | Value | Source | Date |
|---|---|---|---|
| Primary scope | Datacenter optical networking and AI/HPC | Project definition | 2026-06-09 |
| Initial knowledge cutoff | Primarily early 2025 public information | Project brief | 2026-06-09 |
| File count target | 22 Markdown files plus assets directory | Project structure | 2026-06-09 |
| Default evidence hierarchy | Primary sources before secondary research | Editorial convention | 2026-06-09 |
| Forecast convention | Bull/base/bear with explicit confidence | Editorial convention | 2026-06-09 |

## Open Questions / Gaps
- Automate quarterly extraction from SEC filings, earnings transcripts, standards trackers, and patent databases.
- Establish normalized entity IDs, product IDs, units, currencies, and fiscal-calendar mappings.
- Add machine-readable CSV/JSON tables after the Markdown taxonomy stabilizes.
- Validate 2025-2026 startup funding, M&A status, and private-company claims.
- Add archival snapshots so changes in forecasts and product roadmaps are auditable.

## References
- IEEE 802.3 Ethernet Working Group | https://www.ieee802.org/3/ | 2026-06-09
- Optical Internetworking Forum | https://www.oiforum.com/ | 2026-06-09
- Open Compute Project | https://www.opencompute.org/ | 2026-06-09
- Ultra Ethernet Consortium | https://ultraethernet.org/ | 2026-06-09
- U.S. SEC EDGAR | https://www.sec.gov/edgar/search/ | 2026-06-09
