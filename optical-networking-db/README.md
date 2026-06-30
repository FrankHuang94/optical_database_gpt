# Datacenter Optical Networking Knowledge Database
> **Last Updated:** 2026-06-30
> **Status:** In Review
> **Tags:** datacenter-optics, AI-infrastructure, silicon-photonics, transceivers, CPO, market-research

## Overview
This repository is an indexed research database for datacenter optical networking, emphasizing AI/HPC fabrics, datacenter interconnect, Ethernet and InfiniBand scale-out, silicon photonics, high-speed transceivers, and co-packaged optical I/O. Telecom long-haul is excluded unless coherent technology, component supply, standards, or vendor economics directly affect datacenter deployment.

The database uses a canonical topic structure: files `00` through `20` are the only numbered sections. New evidence must be integrated into the relevant existing section. For example, CPO product updates belong in `06_co_packaged_optics.md`; they must not be placed in a new dated supplement. Git history and pull requests provide the historical audit trail.

> ⚠️ Note: This database is research, not investment, legal, export-control, patent, or procurement advice. Market values, product status, standards, and regulations can change immediately.

## Key Findings / Highlights
- [CONFIRMED] IEEE P802.3dj reached Draft 3.0 Standards Association ballot in 2026; detailed status is in [03_standards_and_msa.md](03_standards_and_msa.md).
- [CONFIRMED] Named CPO platforms and rollout evidence are maintained only in [06_co_packaged_optics.md](06_co_packaged_optics.md).
- [CONFIRMED] Current supplier, capacity, power, funding, patent, market, financial, transaction, paper, and regulatory evidence is consolidated into its canonical topic file.
- [CONFIRMED] Duplicate dated refresh files are prohibited by the database conventions.
- [ESTIMATED] AI scale-out, optical scale-up, fiber, laser, packaging, and foundry constraints remain the major strategic themes [MED confidence].

## Detailed Content
### Quick Access
| Section | File | Status | Last Updated |
|---|---|---|---|
| Master index | README.md | In Review | 2026-06-30 |
| Executive summary | [00](00_executive_summary.md) | Draft | 2026-06-30 |
| Technology overview | [01](01_technology_overview.md) | Draft | 2026-06-30 |
| Technology roadmap | [02](02_tech_roadmap.md) | Draft | 2026-06-30 |
| Standards and MSAs | [03](03_standards_and_msa.md) | In Review | 2026-06-30 |
| Silicon photonics | [04](04_silicon_photonics.md) | Draft | 2026-06-30 |
| Transceiver form factors | [05](05_transceiver_form_factors.md) | Draft | 2026-06-30 |
| Co-packaged optics | [06](06_co_packaged_optics.md) | In Review | 2026-06-30 |
| Coherent vs direct detect | [07](07_coherent_vs_direct_detect.md) | Draft | 2026-06-30 |
| Hyperscalers and supplier relationships | [08](08_vendors_hyperscalers.md) | In Review | 2026-06-30 |
| Component vendors | [09](09_vendors_components.md) | Draft | 2026-06-30 |
| Systems vendors | [10](10_vendors_systems.md) | Draft | 2026-06-30 |
| Startups watchlist | [11](11_startups_watchlist.md) | In Review | 2026-06-30 |
| Patents and IP | [12](12_patents_ip_landscape.md) | In Review | 2026-06-30 |
| Research papers | [13](13_key_research_papers.md) | In Review | 2026-06-30 |
| Production and supply chain | [14](14_production_ramp_supply_chain.md) | In Review | 2026-06-30 |
| Competitive landscape | [15](15_competitive_landscape.md) | Draft | 2026-06-30 |
| Market sizing | [16](16_market_sizing.md) | In Review | 2026-06-30 |
| Power and thermal | [17](17_power_and_thermal.md) | In Review | 2026-06-30 |
| AI datacenter architecture | [18](18_AI_datacenter_architecture.md) | Draft | 2026-06-30 |
| Regulation and standards bodies | [19](19_regulatory_and_standards_bodies.md) | In Review | 2026-06-30 |
| Investment and M&A | [20](20_investment_and_ma_tracker.md) | In Review | 2026-06-30 |

### Visual Navigation
Every numbered section now includes a `Visual Guide` with one or more GitHub-rendered Mermaid diagrams. These diagrams are self-authored summaries of the section logic, so they can be versioned like text and updated alongside the evidence tables.

| Visual Theme | Sections |
|---|---|
| System roadmap and link basics | [00](00_executive_summary.md), [01](01_technology_overview.md), [02](02_tech_roadmap.md) |
| Standards, silicon photonics, form factors, CPO, coherent | [03](03_standards_and_msa.md), [04](04_silicon_photonics.md), [05](05_transceiver_form_factors.md), [06](06_co_packaged_optics.md), [07](07_coherent_vs_direct_detect.md) |
| Buyer/vendor ecosystem | [08](08_vendors_hyperscalers.md), [09](09_vendors_components.md), [10](10_vendors_systems.md), [11](11_startups_watchlist.md), [15](15_competitive_landscape.md) |
| Evidence, supply chain, and operations | [12](12_patents_ip_landscape.md), [13](13_key_research_papers.md), [14](14_production_ramp_supply_chain.md), [17](17_power_and_thermal.md), [19](19_regulatory_and_standards_bodies.md) |
| Market and architecture model | [16](16_market_sizing.md), [18](18_AI_datacenter_architecture.md), [20](20_investment_and_ma_tracker.md) |

### Official Visual Source Register
Vendor diagrams, product photos, investor-presentation figures, and architecture graphics should be linked to official pages rather than copied into the repository unless reuse rights are clear. The links below are starting points for reader-friendly visuals and future refresh work.

| Organization | Official Visual / Content Source | Best-Fit Sections |
|---|---|---|
| Lumentum | Datacom and laser product pages: https://www.lumentum.com/en/products | [09](09_vendors_components.md), [14](14_production_ramp_supply_chain.md), [17](17_power_and_thermal.md) |
| Coherent | Networking and transceiver portfolio: https://www.coherent.com/networking | [04](04_silicon_photonics.md), [05](05_transceiver_form_factors.md), [09](09_vendors_components.md) |
| Ciena | WaveLogic and coherent networking pages: https://www.ciena.com/products/wavelogic | [07](07_coherent_vs_direct_detect.md), [10](10_vendors_systems.md), [18](18_AI_datacenter_architecture.md) |
| Marvell | Optical DSP and PAM4 connectivity pages: https://www.marvell.com/products/networking/optical-dsp.html | [02](02_tech_roadmap.md), [07](07_coherent_vs_direct_detect.md), [09](09_vendors_components.md) |
| Broadcom | Tomahawk / StrataXGS switch silicon pages: https://www.broadcom.com/products/ethernet-connectivity/switching/strataxgs | [02](02_tech_roadmap.md), [06](06_co_packaged_optics.md), [18](18_AI_datacenter_architecture.md) |
| NVIDIA | Spectrum-X Ethernet platform pages: https://www.nvidia.com/en-us/networking/ethernet/spectrum-x/ | [08](08_vendors_hyperscalers.md), [10](10_vendors_systems.md), [18](18_AI_datacenter_architecture.md) |
| InnoLight | Optical module product pages: https://www.innolight.com/en | [05](05_transceiver_form_factors.md), [09](09_vendors_components.md), [14](14_production_ramp_supply_chain.md) |
| Arista | 800G and cloud networking solution pages: https://www.arista.com/en/solutions/800g | [08](08_vendors_hyperscalers.md), [10](10_vendors_systems.md), [15](15_competitive_landscape.md) |
| Cisco | Silicon One and Acacia/coherent networking pages: https://www.cisco.com/site/us/en/products/networking/silicon-one/index.html | [07](07_coherent_vs_direct_detect.md), [10](10_vendors_systems.md), [15](15_competitive_landscape.md) |
| Nokia | Photonic Service Engine pages: https://www.nokia.com/networks/ip-networks/photonic-service-engine/ | [07](07_coherent_vs_direct_detect.md), [10](10_vendors_systems.md), [20](20_investment_and_ma_tracker.md) |
| OIF | CEI and coherent implementation-agreement pages: https://www.oiforum.com/technical-work/ | [03](03_standards_and_msa.md), [07](07_coherent_vs_direct_detect.md) |
| Ethernet Alliance | Ethernet roadmap: https://ethernetalliance.org/technology/roadmap/ | [02](02_tech_roadmap.md), [03](03_standards_and_msa.md) |

### Database Scope
| Included | Excluded unless directly relevant |
|---|---|
| Intra-datacenter links from rack to campus | consumer optical interfaces |
| AI/HPC scale-up, scale-out, and scale-across | residential access/PON |
| Ethernet, InfiniBand, RoCE, UEC, DCI | subsea and long-haul deployment |
| Pluggables, LPO, CPO, optical I/O, OCS | general semiconductor markets |
| Components, systems, hyperscalers, supply chain | non-optical networking without architectural relevance |

### Canonical Ownership
| Topic | Canonical File |
|---|---|
| product generation and lane roadmap | `02_tech_roadmap.md` |
| IEEE, OIF, MSA technical status | `03_standards_and_msa.md` |
| CPO products, adoption, readiness | `06_co_packaged_optics.md` |
| hyperscaler strategy and supplier relationships | `08_vendors_hyperscalers.md` |
| private companies, funding, identity | `11_startups_watchlist.md` |
| patents, family searches, FTO risk | `12_patents_ip_landscape.md` |
| papers and technical literature | `13_key_research_papers.md` |
| capacity, yield, lead time, supply chain | `14_production_ramp_supply_chain.md` |
| TAM and forecast reconciliation | `16_market_sizing.md` |
| module, system, and facility power | `17_power_and_thermal.md` |
| regulatory bodies and export controls | `19_regulatory_and_standards_bodies.md` |
| public financials, valuations, funding, M&A | `20_investment_and_ma_tracker.md` |

### How to Use This Database
1. Treat `[CONFIRMED]` as supported by a cited primary or strong secondary source, not as permanently current.
2. Treat `[ESTIMATED]` and forecasts as model inputs; preserve assumptions and attach `[HIGH/MED/LOW confidence]`.
3. Treat `[RUMORED]` as unverified and unsuitable for valuation or procurement decisions.
4. Treat `[DEPRECATED]` as historical technology, company, or superseded guidance.
5. Date every statistic and cite claims inline as `[Source: Organization, YYYY-MM-DD]`.
6. Prefer tables for structured comparisons and relative links for related analysis.
7. Update the existing canonical file; do not create dated numbered supplements.
8. Preserve history through Git commits and pull requests, not duplicate topic files.
9. Use `> ⚠️ Note:` for caveats and `> 🔄 Refresh Needed:` only for genuinely stale areas.

### Update Workflow
| Step | Requirement |
|---|---|
| Intake | record source URL, publication date, access date, and source type |
| Validation | prefer standards bodies, filings, patents, papers, and official product pages |
| Classification | apply status and confidence tags |
| Ownership | map each item to exactly one canonical file |
| Integration | update the relevant table/subsection in place |
| Cross-reference | link to related sections without duplicating detailed content |
| Review | check units, periods, currencies, definitions, and conflicting estimates |
| Preservation | retain prior values in Git history or dated rows where comparison is useful |

### Refresh with Codex
Reconnect Codex to this repository for each refresh and use a new branch and pull request.

```text
Connect to:
https://github.com/FrankHuang94/optical_database_gpt

Refresh optical-networking-db using information current through [DATE].

1. Read README.md and all affected canonical files first.
2. Verify every "Refresh Needed" and "TO VERIFY" item relevant to the update.
3. Prioritize primary sources: standards bodies, filings, official product pages,
   patents, and peer-reviewed papers.
4. Integrate each update into its existing canonical section (00-20).
5. Do not create new numbered refresh/supplement files.
6. Keep one detailed source of truth per topic; use cross-links instead of duplication.
7. Preserve prior values through Git history or dated comparison rows.
8. Update citations, status tags, confidence labels, and Last Updated dates.
9. Do not overwrite an estimate without explaining the changed source or assumption.
10. Validate relative links and confirm the database still contains only sections 00-20.
11. Summarize changed files, resolved gaps, and remaining evidence limitations.
12. Commit to a new branch and open a pull request for review.
```

### Recommended Cadence
| Frequency | Sections / Events |
|---|---|
| Monthly | `03`, `06`, `08`, `11`, `14`, `19`, `20` |
| Quarterly | `09`, `10`, `12`, `15`, `16`, `17`, `20` |
| After OFC and ECOC | `02`-`07`, `13`, `14`, `17` |
| Annually | `00`, `01`, `04`, `05`, `07`, `18` |

## Data Tables (where applicable)
| Field | Value | Source | Date |
|---|---|---|---|
| Primary scope | datacenter optical networking and AI/HPC | project definition | 2026-06-09 |
| Canonical numbered sections | 00-20 | repository convention | 2026-06-09 |
| Markdown count | 22 including README | repository target | 2026-06-09 |
| History mechanism | Git commits and pull requests | repository convention | 2026-06-09 |
| Forecast convention | bull/base/bear with explicit confidence | editorial convention | 2026-06-09 |

## Open Questions / Gaps
- Acquire licensed LightCounting/Omdia/Dell'Oro/Cignal source tables.
- Obtain independent CPO full-system power, yield, and reliability data.
- Complete alias/CPC patent-family searches and legal claim review.
- Resolve ambiguous startup identities with legal entities or URLs.
- Automate quarterly filings, standards, patents, restricted parties, pricing, and transactions.

## References
- IEEE 802.3 Ethernet Working Group | https://www.ieee802.org/3/ | 2026-06-09
- Optical Internetworking Forum | https://www.oiforum.com/ | 2026-06-09
- Open Compute Project | https://www.opencompute.org/ | 2026-06-09
- Ultra Ethernet Consortium | https://ultraethernet.org/ | 2026-06-09
- U.S. SEC EDGAR | https://www.sec.gov/edgar/search/ | 2026-06-09
