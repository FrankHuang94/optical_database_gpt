# Datacenter Optical Networking Knowledge Database
> **Last Updated:** 2026-06-09
> **Status:** In Review
> **Tags:** datacenter-optics, AI-infrastructure, silicon-photonics, transceivers, CPO, market-research

## Overview
This repository is an indexed research database for datacenter optical networking, with emphasis on AI/HPC fabrics, datacenter interconnect (DCI), Ethernet and InfiniBand scale-out networks, silicon photonics, high-speed transceivers, and emerging co-packaged optical I/O. Telecom long-haul is excluded except where coherent technology, component supply, standards, or vendor economics directly affect datacenter deployment.

Files `00`-`20` provide the thematic baseline. Files `21`-`30` are dated 2026 evidence refreshes addressing product status, standards, valuations, forecasts, startups, patents, hyperscaler relationships, manufacturing, power, M&A, papers, and regulation. Use the dated refresh file when it conflicts with an older baseline, while preserving the older file as historical context.

> ⚠️ Note: This database is research, not investment, legal, export-control, patent, or procurement advice. Market values and regulatory status can change immediately.

## Key Findings / Highlights
- [CONFIRMED] IEEE P802.3dj reached Draft 3.0 Standards Association ballot in 2026; it is not yet a final standard [Source: IEEE 802.3dj, 2026-06-04].
- [CONFIRMED] OIF published 800ZR, 800LR, CMIS 5.4, and additional EEI/ELSFP agreements while opening 1600ZR, NPO, compute-optics, and 448G work [Source: OIF, accessed 2026-06-09].
- [CONFIRMED] Named CPO products now include Broadcom Bailly and NVIDIA Quantum-X/Spectrum-X Photonics, but independent HVM power/reliability data remain limited.
- [CONFIRMED] 2026 capacity agreements connect NVIDIA with Coherent and Lumentum, and hyperscalers Meta/Amazon with Corning.
- [ESTIMATED] AI scale-out, optical scale-up, and fiber/connectivity demand are shifting value toward lasers, packaging, foundry capacity, and system co-design [MED confidence].

## Detailed Content
### Quick Access
| Section | File | Status | Last Updated |
|---|---|---|---|
| Master index | README.md | In Review | 2026-06-09 |
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

### 2026 Evidence Refresh
| Gap Addressed | File | Status |
|---|---|---|
| Product and CPO announcements | [21](21_2026_product_and_cpo_tracker.md) | In Review |
| IEEE/OIF project status | [22](22_2026_ieee_oif_status.md) | In Review |
| Company financials and valuations | [23](23_2026_financials_and_valuations.md) | In Review |
| Market forecast reconciliation | [24](24_market_forecast_reconciliation.md) | In Review |
| Startup identity and funding | [25](25_startup_identity_and_funding_audit.md) | In Review |
| Patent-family searches | [26](26_patent_family_search_2026.md) | In Review |
| Hyperscaler-supplier relationships | [27](27_hyperscaler_supplier_relationships.md) | In Review |
| Capacity, yield, and lead times | [28](28_capacity_yield_and_lead_times.md) | In Review |
| Full-system power | [29](29_full_system_power_benchmarks.md) | In Review |
| M&A, papers, and export controls | [30](30_2026_ma_papers_and_export_controls.md) | In Review |

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
7. Use dated refresh files as current overlays; do not silently rewrite history.
8. Use `> ⚠️ Note:` for caveats and `> 🔄 Refresh Needed:` for stale or fast-changing areas.

### Update Workflow
| Step | Requirement |
|---|---|
| Intake | Record source URL, publication date, access date, and source type |
| Validation | Prefer standards bodies, filings, patents, papers, and vendor product pages |
| Classification | Apply status and confidence tags |
| Integration | Add a dated refresh record and update cross-references |
| Review | Check units, periods, currency, definitions, and conflicting estimates |
| Preservation | Do not overwrite prior forecasts or snapshots without retaining the old value |

### Refresh with Codex
Reconnect Codex to this repository for each refresh and use a pull request so proposed changes can be reviewed before merging into `main`.

```text
Connect to:
https://github.com/FrankHuang94/optical_database_gpt

Refresh optical-networking-db using information current through [DATE].

1. Read the existing files first.
2. Verify every "Refresh Needed" and "TO VERIFY" item.
3. Prioritize primary sources.
4. Preserve historical data and add new dated rows.
5. Update citations, status tags, and Last Updated dates.
6. Do not overwrite estimates without explaining the change.
7. Summarize changed files, resolved gaps, and remaining gaps.
8. Commit changes to a new branch and open a pull request.
```

Recommended cadence:

| Frequency | Sections / Events |
|---|---|
| Monthly | `21`, `22`, `25`, `27`, `28`, `30` |
| Quarterly | `23`, `24`, `26`, `29` and relevant baseline files |
| After OFC and ECOC | `02`-`07`, `13`, `21`, `22`, `29`, `30` |
| Annually | `01` fundamentals and glossary |

## Data Tables (where applicable)
| Field | Value | Source | Date |
|---|---|---|---|
| Primary scope | Datacenter optical networking and AI/HPC | Project definition | 2026-06-09 |
| Thematic baseline | files 00-20 | Repository | 2026-06-09 |
| Dated evidence refresh | files 21-30 | Repository | 2026-06-09 |
| Markdown file count | 32 including README | Repository audit | 2026-06-09 |
| Forecast convention | Bull/base/bear with explicit confidence | Editorial convention | 2026-06-09 |

## Open Questions / Gaps
- Acquire licensed LightCounting/Omdia/Dell'Oro/Cignal source tables and preserve license-compliant derived data.
- Obtain independent CPO full-system power, yield, and field-reliability measurements.
- Complete alias/CPC patent searches and legal claim review.
- Resolve ambiguous startup names with legal entities or URLs.
- Automate quarterly SEC, standards, patent, restricted-party, pricing, and transaction feeds.

## References
- IEEE 802.3 Ethernet Working Group | https://www.ieee802.org/3/ | 2026-06-09
- Optical Internetworking Forum | https://www.oiforum.com/ | 2026-06-09
- Open Compute Project | https://www.opencompute.org/ | 2026-06-09
- Ultra Ethernet Consortium | https://ultraethernet.org/ | 2026-06-09
- U.S. SEC EDGAR | https://www.sec.gov/edgar/search/ | 2026-06-09
