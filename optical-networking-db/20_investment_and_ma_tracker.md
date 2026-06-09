# Investment and M&A Tracker
> **Last Updated:** 2026-06-09
> **Status:** Draft
> **Tags:** investment, valuation, M-and-A, venture-funding, catalysts

## Overview
This tracker links operating indicators to valuation, financing, and strategic transactions. Optical names differ materially in fiscal calendars and business mix, so market capitalization and multiples must use same-day prices and standardized LTM financials.

The table is intentionally not populated with stale “current” market values. Historical transaction and funding baselines are included, while live market data, short interest, and catalyst dates are queued for automated refresh [See: [11_startups_watchlist.md](11_startups_watchlist.md)].

> 🔄 Refresh Needed: High Priority — ingest same-day prices, debt/cash, LTM filings, short interest, earnings calendars, and deal status.

## Key Findings / Highlights
- [CONFIRMED] Strategic acquisitions have concentrated coherent DSP, PAM4 DSP, lasers, and network systems.
- [CONFIRMED] AI optical exposure is often estimated because public segments include telecom, industrial, and consumer products.
- [ESTIMATED] Revenue growth without gross-margin and customer-concentration analysis is an incomplete investment signal [HIGH confidence].
- [CONFIRMED] OFC and ECOC are recurring product-announcement catalysts.
- [ESTIMATED] CPO startups are plausible strategic targets, but timing depends on customer qualification and IP ownership.

## Detailed Content
### Public Company Financial Tracker
| Company | Ticker | Market Cap | EV | Revenue LTM ($M) | YoY Growth % | EV/Revenue | Gross Margin % | DC Optical Revenue % | Next Catalyst |
|---|---|---:|---:|---:|---:|---:|---:|---:|---|
| Coherent | COHR | [LIVE DATA] | [LIVE DATA] | [TO UPDATE] | [TO UPDATE] | formula | [TO UPDATE] | 25-40% [ESTIMATED] | earnings / 800G-1.6T mix |
| Lumentum | LITE | [LIVE DATA] | [LIVE DATA] | [TO UPDATE] | [TO UPDATE] | formula | [TO UPDATE] | 20-35% [ESTIMATED] | cloud laser ramp |
| Applied Optoelectronics | AAOI | [LIVE DATA] | [LIVE DATA] | [TO UPDATE] | [TO UPDATE] | formula | [TO UPDATE] | 50-75% [ESTIMATED] | 800G qualification |
| Fabrinet | FN | [LIVE DATA] | [LIVE DATA] | [TO UPDATE] | [TO UPDATE] | formula | [TO UPDATE] | 50-70% [ESTIMATED] | datacom mix/capacity |
| Marvell | MRVL | [LIVE DATA] | [LIVE DATA] | [TO UPDATE] | [TO UPDATE] | formula | [TO UPDATE] | 10-20% direct [ESTIMATED] | custom AI / optical DSP |
| Arista | ANET | [LIVE DATA] | [LIVE DATA] | [TO UPDATE] | [TO UPDATE] | formula | [TO UPDATE] | indirect/high DC | AI Ethernet revenue |
| Ciena | CIEN | [LIVE DATA] | [LIVE DATA] | [TO UPDATE] | [TO UPDATE] | formula | [TO UPDATE] | DCI subset | cloud/coherent orders |
| Cisco | CSCO | [LIVE DATA] | [LIVE DATA] | [TO UPDATE] | [TO UPDATE] | formula | [TO UPDATE] | low consolidated | AI backlog / Acacia |
| Nokia | NOK | [LIVE DATA] | [LIVE DATA] | [TO UPDATE] | [TO UPDATE] | formula | [TO UPDATE] | DCI subset | Infinera integration |
| Viavi | VIAV | [LIVE DATA] | [LIVE DATA] | [TO UPDATE] | [TO UPDATE] | formula | [TO UPDATE] | indirect | 1.6T test cycle |

### Recent / Strategic M&A
| Date | Acquirer | Target | Deal Value | EV/Revenue | Strategic Rationale | Status |
|---|---|---|---:|---:|---|---|
| 2024-06 | Nokia | Infinera | ~$2.3B EV | [TO CALCULATE] | optical scale, DSP/PIC portfolio | announced; [TO VERIFY current] |
| 2024-01 | HPE | Juniper | ~$14B equity | [TO CALCULATE] | networking and AI systems | announced; [TO VERIFY current] |
| 2022-07 | II-VI | Coherent | ~$5.7B | [TO CALCULATE] | vertical optical integration | closed |
| 2021-04 | Cisco | Acacia | ~$4.5B | [TO CALCULATE] | coherent DSP/modules | closed |
| 2021-04 | Marvell | Inphi | ~$10B | [TO CALCULATE] | cloud interconnect silicon | closed |
| 2020-04 | NVIDIA | Mellanox | $6.9B | [TO CALCULATE] | AI/HPC networking | closed |

### Venture Funding Tracker
| Company | Stage | Amount ($M) | Date | Lead Investor | Valuation ($M) |
|---|---|---:|---|---|---:|
| Ayar Labs | growth | 155 [TO VERIFY round] | 2024 | Advent/Light Street-led [TO VERIFY] | undisclosed |
| Lightmatter | growth | 400 [TO VERIFY round/extension] | 2024 | T. Rowe Price-related lead [TO VERIFY] | [TO VERIFY] |
| Celestial AI | growth | 175 [TO VERIFY round] | 2024 | US Innovative Technology Fund [TO VERIFY] | undisclosed |
| Nubis Communications | venture | [TO VERIFY] | 2023-2024 | [TO VERIFY] | undisclosed |
| Avicena | venture | [TO VERIFY] | 2023-2024 | [TO VERIFY] | undisclosed |
| Xscape Photonics | seed/Series A | [TO VERIFY] | 2022-2024 | [TO VERIFY] | undisclosed |

> ⚠️ Note: Funding “amount” may refer to a latest round, not total funding. Validate against company press releases and financing documents.

### Investor Theses
| Thesis | Bull Case | Bear Case |
|---|---|---|
| Bandwidth density | optics moves closer to compute | electrical reach improves enough |
| Power efficiency | CPO/LPO reduce I/O energy | savings lost to lasers/cooling/yield |
| AI unit growth | more accelerators and links | capex digestion / utilization limits |
| 1.6T cycle | content and ASP uplift | rapid price erosion and delays |
| Consolidation | scarce IP gains strategic premium | integration and customer conflict |

### Short Interest Tracker
| Company | Short Interest % Float | Days to Cover | As-of Date | Source |
|---|---:|---:|---|---|
| COHR | [LIVE DATA] | [LIVE DATA] | [TO UPDATE] | exchange/FINRA |
| LITE | [LIVE DATA] | [LIVE DATA] | [TO UPDATE] | exchange/FINRA |
| AAOI | [LIVE DATA] | [LIVE DATA] | [TO UPDATE] | exchange/FINRA |
| FN | [LIVE DATA] | [LIVE DATA] | [TO UPDATE] | exchange/FINRA |

### Catalyst Calendar
| Date | Company / Event | Catalyst Type | Bull Case | Bear Case |
|---|---|---|---|---|
| March annually | OFC | products/standards | 1.6T/CPO design wins | demos remain pre-volume |
| September/October annually | ECOC | research/products | 200G/lane progress | reliability/yield delays |
| Quarterly | public-company earnings | financial | AI optics beats estimates | customer digestion/margin pressure |
| IEEE meeting calendar | 802.3dj votes | standards | stable 1.6T ecosystem | schedule/objective changes |
| Vendor launch cycles | switch/optics launches | product | 102.4T adoption | thermal or supply constraints |

### Refresh Formulas
- `Enterprise Value = Market Cap + Debt + Preferred + Minority Interest - Cash`.
- `EV/Revenue = Enterprise Value / standardized LTM revenue`.
- Use diluted share count and same-day FX.
- Treat announced backlog consistently; do not mix orders, revenue, and design wins.
- Preserve historical snapshots rather than overwriting prior estimates.

## Data Tables (where applicable)
| Field | Value | Source | Date |
|---|---|---|---|
| Largest tracked strategic deal | HPE/Juniper ~$14B announced | HPE | 2024 |
| Largest optics-silicon deal | Marvell/Inphi ~$10B | Marvell | 2020 announced |
| Coherent consolidation | Cisco/Acacia; Nokia/Infinera | company announcements | 2021/2024 |
| Required price frequency | daily for live valuation | methodology | 2026-06-09 |
| Required financial frequency | quarterly | methodology | 2026-06-09 |

## Open Questions / Gaps
- Populate live market, EV, LTM, margin, and short-interest data.
- Verify M&A close/status and calculate announcement-date multiples.
- Confirm venture round amounts, leads, totals, and valuations.
- Build earnings and standards calendar feeds.
- Backtest optical KPIs against revenue and stock performance.

## References
- SEC EDGAR | https://www.sec.gov/edgar/search/ | 2026-06-09
- FINRA Short Interest | https://www.finra.org/finra-data/browse-catalog/equity-short-interest/data | 2026-06-09
- OFC | https://www.ofcconference.org/ | 2026-06-09
- ECOC | https://www.ecocexhibition.com/ | 2026-06-09
- Company investor-relations sites | URLs listed in vendor files | 2026-06-09
