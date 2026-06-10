# 2026 Financials and Valuations
> **Last Updated:** 2026-06-09
> **Status:** In Review
> **Tags:** financials, valuation, public-companies, LTM, market-cap, 2026-refresh

## Overview
This snapshot adds same-day market values and standardized trailing financials for the primary public optical/networking comparables. It supplements [09_vendors_components.md](09_vendors_components.md), [10_vendors_systems.md](10_vendors_systems.md), and [20_investment_and_ma_tracker.md](20_investment_and_ma_tracker.md).

Market values are a June 9, 2026 snapshot and will become stale immediately. LTM revenue and margins use S&P Global Market Intelligence data displayed by StockAnalysis; they should be reconciled to the latest 10-Q/10-K before use in a model. Optical exposure is not comparable across companies and is kept separate from valuation.

> ⚠️ Note: Several optical equities experienced exceptional 2025-2026 appreciation. High EV/revenue ratios in this table are a market snapshot, not a normalized-cycle valuation recommendation.

## Key Findings / Highlights
- [CONFIRMED] Coherent's LTM revenue was approximately $6.60B with 37.0% gross margin; June 9, 2026 EV was approximately $70.64B [Source: S&P Global Market Intelligence via StockAnalysis, 2026-06-09].
- [CONFIRMED] Lumentum's LTM revenue was approximately $2.49B with 40.8% gross margin; EV was approximately $64.07B [Source: same].
- [CONFIRMED] Marvell's LTM revenue was approximately $8.72B with 51.5% gross margin; EV was approximately $229.98B [Source: same].
- [CONFIRMED] Fabrinet's LTM revenue reached approximately $4.24B, but its manufacturing model produced a much lower 12.0% gross margin than IP/system vendors [Source: same].
- [ESTIMATED] Pure-play optical exposure commands a large 2026 valuation premium, but revenue concentration and capacity execution make comparisons highly cycle-sensitive [HIGH confidence].

## Detailed Content
### Public Company Snapshot
| Company | Ticker | Price ($) | Market Cap ($B) | EV ($B) | LTM Revenue ($B) | EV/Revenue | Gross Margin | Net Cash / (Debt) ($B) | Snapshot Quality |
|---|---|---:|---:|---:|---:|---:|---:|---:|---|
| Coherent | COHR | 355.94 | 69.64 | 70.64 | 6.60 | 10.70x | 36.99% | (1.00) | [CONFIRMED] direct page values |
| Lumentum | LITE | 821.76 | 63.93 | 64.07 | 2.49 | 25.75x | 40.84% | (0.14) | [CONFIRMED] direct page values |
| Applied Optoelectronics | AAOI | 162.88 | ~13.1 | ~12.9 | 0.507 | ~25.4x | 29.64% | 0.159 | [ESTIMATED] market cap from price x shares; financials confirmed |
| Fabrinet | FN | ~586 | ~21.0 | ~20.1 | 4.24 | ~4.7x | 12.04% | 0.941 | [ESTIMATED] market cap from price x shares; financials confirmed |
| Marvell | MRVL | 266.88 | 233.47 | 229.98 | 8.72 | 26.38x | 51.50% | (1.43) | [CONFIRMED] direct page values |
| Arista Networks | ANET | 152.16 | 191.60 | 179.25 | 9.71 | 18.46x | 63.54% | 12.35 | [CONFIRMED] direct page values |
| Ciena | CIEN | 439.34 | ~62.4 | ~62.6 | 5.57 | ~11.2x | 43.05% | (0.18) | [ESTIMATED] market cap; financials confirmed |
| Cisco | CSCO | ~120.36 | ~474.7 | ~491.1 | 60.75 | ~8.1x | 64.30% | (16.36) | [ESTIMATED] market cap; financials confirmed |
| Nokia | NOK | 13.85 | 77.62 | 74.83 | 23.06 | 3.25x | 45.36% | 2.89 | [CONFIRMED] ADR-based direct page values |
| Viavi | VIAV | 46.03 intraday | 11.28 | 11.82 | 1.37 | 8.65x | 60.36% | (0.64) | [CONFIRMED] direct page values |

### Profitability and Cash Flow
| Company | Operating Margin | LTM Net Income ($M) | LTM FCF ($M) | Interpretation |
|---|---:|---:|---:|---|
| Coherent | 12.08% | 401 | (538) | growth/capacity investment and working-capital effects require review |
| Lumentum | 10.22% | 439 | 114 | improving mix; high valuation embeds major growth |
| AAOI | -11.57% | (43) | (449) | capacity ramp and execution risk remain material |
| Fabrinet | 9.86% | 421 | 46 | high-volume manufacturing, low margin, capital-intensive ramp |
| Marvell | 16.41% | 2,530 | 1,670 | high-margin silicon platform with AI/custom concentration |
| Arista | 42.79% | 3,720 | 5,280 | software/system economics and net-cash balance sheet |
| Ciena | 11.20% | 438 | 833 | transport cycle and cloud/DCI mix |
| Cisco | 23.71% | 11,960 | 11,790 | optical exposure diluted by broad portfolio |
| Nokia | 8.44% | 918 | 1,580 | broad telecom exposure; Infinera integration |
| Viavi | 8.98% | (55) | 46 | test-cycle exposure and acquisition/debt effects |

### Exposure Classification
| Class | Companies | Use in Comparable Analysis |
|---|---|---|
| Optical component/module | COHR, LITE, AAOI | closest demand sensitivity; different product mix |
| Optical manufacturing | FN | volume/capacity proxy, structurally lower gross margin |
| Optical/DSP silicon | MRVL | AI/custom silicon dominates consolidated valuation |
| Network systems | ANET, CSCO | optical pull-through but not merchant-optics economics |
| Coherent transport | CIEN, NOK | DCI plus telecom cycle |
| Test | VIAV | enabling capital-equipment/test proxy |

### Refresh Method
1. Use the same market close for price and diluted share count.
2. Reconcile cash, debt, minority interest, and convertibles from the latest filing.
3. Use GAAP LTM revenue and gross margin; place adjusted metrics in separate columns.
4. Preserve this dated snapshot rather than overwriting it.
5. Do not compare EV/revenue without optical exposure, growth, margin, and capital intensity.

## Data Tables (where applicable)
| Field | Value | Source | Date |
|---|---|---|---|
| Valuation snapshot | US market close | StockAnalysis/S&P Global MI | 2026-06-09 |
| Highest direct EV/revenue | Marvell ~26.4x; Lumentum ~25.8x | snapshot | 2026-06-09 |
| Lowest direct EV/revenue | Nokia ~3.25x | snapshot | 2026-06-09 |
| Highest gross margin | Cisco 64.3%; Arista 63.5% | LTM | 2026-06-09 |
| Optical manufacturing gross margin | Fabrinet 12.0% | LTM | 2026-06-09 |

## Open Questions / Gaps
- Reconcile estimated market caps for AAOI, FN, CIEN, and CSCO to official closing share counts.
- Add YoY revenue growth and optical-specific revenue bridges from each latest filing.
- Normalize stock-based compensation, restructuring, and acquisition accounting.
- Add China-listed InnoLight/Eoptolink/Accelink/Huagong Tech using consistent FX and accounting.
- Automate monthly snapshots rather than replacing the June 2026 baseline.

## References
- COHR Statistics | https://stockanalysis.com/stocks/cohr/statistics/ | 2026-06-09
- LITE Statistics | https://stockanalysis.com/stocks/lite/statistics/ | 2026-06-09
- AAOI Statistics | https://stockanalysis.com/stocks/aaoi/statistics/ | 2026-06-09
- FN Statistics | https://stockanalysis.com/stocks/fn/statistics/ | 2026-06-09
- MRVL Statistics | https://stockanalysis.com/stocks/mrvl/statistics/ | 2026-06-09
- ANET Statistics | https://stockanalysis.com/stocks/anet/statistics/ | 2026-06-09
- CIEN Statistics | https://stockanalysis.com/stocks/cien/statistics/ | 2026-06-09
- CSCO Statistics | https://stockanalysis.com/stocks/csco/statistics/ | 2026-06-09
- NOK Statistics | https://stockanalysis.com/stocks/nok/statistics/ | 2026-06-09
- VIAV Statistics | https://stockanalysis.com/stocks/viav/statistics/ | 2026-06-09
