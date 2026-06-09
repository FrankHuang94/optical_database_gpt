# Startup Identity and Funding Audit
> **Last Updated:** 2026-06-09
> **Status:** In Review
> **Tags:** startups, funding, identity-audit, optical-I-O, photonics

## Overview
This file audits the seed list in [11_startups_watchlist.md](11_startups_watchlist.md). It separates active optical-networking companies from photonic-compute companies, adjacent manufacturing/software companies, public companies, acquired companies, and names that cannot be tied to a credible datacenter-optics entity.

Funding totals are based on announced rounds rather than private databases. “Total known funding” is a floor because undisclosed seed, debt, grant, and strategic financing may be omitted. Acquired companies are removed from the active startup cohort but retained for historical tracking.

> ⚠️ Note: Private-company valuations and customer names are often confidential. Do not infer revenue or production from funding size.

## Key Findings / Highlights
- [CONFIRMED] Ayar Labs announced a $155M financing in December 2024, taking publicly reported cumulative funding to roughly $370M [Source: Ayar Labs, 2024].
- [CONFIRMED] Lightmatter announced a $400M Series D in October 2024 at a reported $4.4B valuation [Source: Lightmatter, 2024].
- [CONFIRMED] Celestial AI announced a $250M Series C in March 2025; it should be tracked as an acquisition/M&A subject if the announced Marvell transaction is confirmed in current filings.
- [CONFIRMED] AMD acquired Enosemi in May 2025, so Enosemi belongs in the M&A history rather than the active watchlist.
- [CONFIRMED] Enavate Sciences and DragonWave are category mismatches for an active datacenter-optical startup list.

## Detailed Content
### Active Core Watchlist
| Company | Category | Latest Public Financing | Known Funding Floor | Status | Confidence |
|---|---|---:|---:|---|---|
| Ayar Labs | optical I/O chiplets + external laser | $155M, 2024 | ~$370M | active/private | [HIGH] |
| Lightmatter | photonic interconnect / Passage | $400M Series D, 2024 | >$800M reported across rounds [TO VERIFY exact] | active/private | [HIGH latest round] |
| Ranovus | CPO/NPO optical engines | strategic/venture rounds; exact latest amount not consistently public | [TO VERIFY] | active/private | [MED] |
| Nubis Communications | linear optical engines | $50M-class Series B reported in 2024 | ~$80M+ [TO VERIFY] | active/private | [MED] |
| Avicena | microLED optical interconnect | $65M-class Series B reported in 2025 | ~$100M [TO VERIFY] | active/private | [MED] |
| Xscape Photonics | WDM optical interconnect | $44M Series A reported in 2025 | ~$50M [TO VERIFY] | active/private | [MED] |
| OpenLight | heterogeneous laser-integrated SiPh platform | Series A/strategic backing; amount not consistently disclosed | [TO VERIFY] | active/private | [MED] |
| Quintessent | quantum-dot multi-wavelength lasers | seed/grant funded | [TO VERIFY] | active/private | [MED] |
| Teramount | detachable fiber-to-chip packaging | venture funded | [TO VERIFY] | active/private | [MED] |
| Salience Labs | photonic AI compute | ~$30M Series A reported in 2025 | [TO VERIFY] | active/private; adjacent | [MED] |

### Funding Events Requiring Transaction-Level Tracking
| Company | Event | Date | Investors / Strategic Signal | Database Treatment |
|---|---|---|---|---|
| Ayar Labs | $155M financing | 2024-12 | strategic semiconductor and financial investors | confirmed round; verify cumulative total quarterly |
| Lightmatter | $400M Series D | 2024-10 | large late-stage institutional round | confirmed round and reported valuation |
| Celestial AI | $250M Series C | 2025-03 | AI infrastructure growth financing | move to acquired/pending-acquisition set when legally closed |
| Nubis | Series B | 2024 | Ericsson Ventures and other strategic investors reported | exact amount/source refresh needed |
| Avicena | Series B | 2025 | semiconductor/strategic investors reported | exact close date and total refresh needed |
| Xscape | Series A | 2025 | strategic AI/networking participation reported | exact investor list refresh needed |

### Acquired / No Longer Independent
| Company | Acquirer | Date | Status | Strategic Rationale |
|---|---|---:|---|---|
| Enosemi | AMD | 2025-05-28 | [CONFIRMED] acquired | photonic IC design tools/IP and optical interconnect capability |
| Celestial AI | Marvell | 2025 announcement [TO VERIFY close] | announced transaction | photonic fabric for scale-up/scale-out AI |
| Intel silicon-photonics product business | Jabil | 2023 | [CONFIRMED] transferred | manufacturing/product continuity |
| Advanced Micro Foundry | GlobalFoundries | 2025-11 | [CONFIRMED] acquired | SiPh foundry scale and Singapore capacity |

### Adjacent but Not Core Optical-Network Startups
| Company | Actual Category | Treatment |
|---|---|---|
| Tignis | AI/process-control software for manufacturing | retain in supply-chain software appendix, not optical vendor TAM |
| POET Technologies | public company (NASDAQ/TSXV), optical interposer | move to public emerging-company tracker |
| Salience Labs | photonic compute | track separately from optical interconnect revenue |
| Baya Systems | chiplet fabric/IP, if this was intended by “Bayan Semiconductor” | adjacent electrical chiplet interconnect; confirm intended name |

### Ambiguous or Excluded Names
| Prompt Name | Audit Result | Action |
|---|---|---|
| Bayan Semiconductor | no confidently matched datacenter-photonics company | [UNRESOLVED]; likely name error, possibly Baya Systems |
| Enavate Sciences | life-sciences investment/company identity, not datacenter optics | [DEPRECATED] remove from optical startup cohort |
| Flux Photonics | multiple/unclear identities; no verified target company | [UNRESOLVED] require URL or founder name |
| Mitarum | no verified datacenter-optics entity under this spelling | [UNRESOLVED] require URL or corrected spelling |
| Nexus Photonics | historical/ambiguous identity; no current startup verified | [UNRESOLVED] require legal entity or URL |
| DragonWave | microwave packet-backhaul company with insolvency history | [DEPRECATED] exclude; not optical datacenter networking |

### Diligence Scorecard
| Dimension | Minimum Evidence |
|---|---|
| Legal identity | company registry/name and headquarters |
| Funding | company release or lead-investor release |
| Product | datasheet, conference demonstration, or customer integration |
| Manufacturing | named foundry/OSAT and qualification stage |
| Customer | named agreement, not investor inference |
| IP | assigned patents and university-license terms |
| Status | active site, employees, recent filings/news |

## Data Tables (where applicable)
| Field | Value | Source | Date |
|---|---|---|---|
| Ayar latest disclosed round | $155M | Ayar Labs | 2024-12 |
| Lightmatter Series D | $400M | Lightmatter | 2024-10 |
| Lightmatter reported valuation | $4.4B | company/media reports | 2024-10 |
| Celestial AI Series C | $250M | Celestial AI | 2025-03 |
| Verified category mismatches | Enavate Sciences, DragonWave | identity audit | 2026-06-09 |

## Open Questions / Gaps
- Confirm Celestial AI transaction closing, consideration structure, and employee retention.
- Obtain primary-source releases for Nubis, Avicena, Xscape, Salience, Teramount, and Quintessent round totals.
- Resolve Bayan Semiconductor, Flux Photonics, Mitarum, and Nexus Photonics from user-supplied URLs or legal names.
- Add cash-runway estimates only after financing dates, headcount, and burn assumptions are sourced.
- Move POET into the public-company financial tracker.

## References
- Ayar Labs News | https://ayarlabs.com/news/ | 2026-06-09
- Lightmatter News | https://lightmatter.co/news/ | 2026-06-09
- Celestial AI | https://www.celestial.ai/ | 2026-06-09
- AMD Newsroom | https://www.amd.com/en/newsroom.html | 2026-06-09
- Nubis Communications | https://www.nubis-inc.com/ | 2026-06-09
- Avicena | https://avicena.tech/ | 2026-06-09
- Xscape Photonics | https://www.xscapephotonics.com/ | 2026-06-09
- OpenLight | https://openlightphotonics.com/ | 2026-06-09
