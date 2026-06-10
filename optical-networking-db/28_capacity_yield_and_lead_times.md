# Capacity, Yield, and Lead Times
> **Last Updated:** 2026-06-09
> **Status:** In Review
> **Tags:** capacity, yield, lead-time, manufacturing, 800G, 1.6T

## Overview
This file adds disclosed production-capacity and ramp evidence to [14_production_ramp_supply_chain.md](14_production_ramp_supply_chain.md). Public companies disclose revenue, capex, facilities, and selected unit targets, but rarely publish optical assembly yield or customer-specific lead time.

The correct conclusion is not to invent yield percentages. The database records hard capacity signals, identifies where yield is implicit in financial performance, and defines the supplier questionnaire needed to close the remaining gaps.

> ⚠️ Note: Nameplate capacity, qualified capacity, good-unit output, and customer-accepted shipments are different measures.

## Key Findings / Highlights
- [CONFIRMED] AAOI targeted 100,000 800G transceivers per month by year-end 2025, with approximately 35% of production planned in the United States [Source: AAOI earnings coverage, 2025-11].
- [CONFIRMED] Fabrinet reported FY2026 Q2 revenue of $1.13B; HPC revenue increased from $15.4M to $85.6M sequentially, with management targeting more than $150M when the first program is fully ramped [Source: Fabrinet earnings coverage, 2026-02].
- [CONFIRMED] NVIDIA's 2026 agreements provide Coherent and Lumentum with $2B each plus multibillion-dollar purchase commitments and capacity-access rights [Source: company announcements, 2026-03].
- [CONFIRMED] Lumentum said it would build a new fabrication facility to support the NVIDIA relationship [Source: Lumentum/NVIDIA announcement coverage, 2026-03].
- [CONFIRMED] Meta and Amazon agreements are driving Corning capacity expansion in North Carolina [Source: company agreement coverage, 2026].

## Detailed Content
### Disclosed Capacity Signals
| Supplier | Capacity / Ramp Signal | Date | What Is Known | What Is Not Known |
|---|---|---:|---|---|
| AAOI | 100k 800G modules/month target; 35% US | 2025 year-end target | module-rate target and geography | achieved good-unit output, product mix, yield |
| Fabrinet | HPC revenue $15.4M to $85.6M; >$150M full-ramp target | FY2026 Q1-Q2 | financial ramp of first HPC program | units, customer, optical content, yield |
| Coherent | $2B investment + purchase/capacity rights | 2026-03 | financed US capacity expansion | exact wafers/month, laser type, allocation |
| Lumentum | $2B investment + purchase/capacity rights; new fab | 2026-03 | major new laser/optics capacity | fab location, tool plan, output date, yield |
| Corning | Meta up to $6B; Amazon multibillion agreement | 2026 | fiber/cable/connectivity demand and NC expansion | fiber-km, connector units, pricing |
| GlobalFoundries | acquired Advanced Micro Foundry | 2025-11 | added Singapore SiPh foundry capability | consolidated photonics wafer capacity |
| Jabil | acquired Intel SiPh product business | 2023 | product/manufacturing continuity | current module capacity and customer mix |

### Yield Disclosure Audit
| Layer | Public Numerical Yield Found? | Best Available Proxy | Required Metric |
|---|---|---|---|
| III-V epitaxy / laser die | no | gross margin, capacity investments, shortages | epi wafer yield; good laser die/wafer |
| SiPh wafer | no supplier-comparable set | foundry qualification and MPW maturity | wafer sort yield by PIC area/process |
| DSP/SerDes | no optical-specific yield | advanced-node supply and product margin | known-good die yield |
| Laser/PIC attach | no | module ramp delays and assembly capex | first-pass attach yield and rework rate |
| Module calibration/test | no | test-time/capex commentary | first-pass yield, calibration seconds/channel |
| CPO package | no | demonstration/customer shipment status | package yield, engine replacement/rework |
| Field reliability | no comparable set | warranty reserve/RMA commentary | FIT, DPPM, annualized failure rate |

### Lead-Time Evidence
| Item | 2026 Assessment | Evidence Quality |
|---|---|---|
| 800G modules | demand-constrained at selected suppliers; customer allocations likely | [MED] earnings/channel evidence |
| 1.6T modules | qualification and early ramp; lead time dominated by 200G/lane components | [MED] roadmap evidence |
| advanced lasers | capacity commitments imply strategic scarcity | [HIGH inference] from NVIDIA investments |
| SiPh foundry | expanding through GF/AMF and new programs | [MED] capacity numbers undisclosed |
| fiber/connectivity | hyperscaler contracts driving US expansion | [HIGH] contract evidence |
| test equipment | generation transition drives demand; exact lead times undisclosed | [LOW/MED] |

### Ramp Stage Definitions
| Stage | Required Evidence |
|---|---|
| Engineering sample | functional device; no production commitment |
| Customer sample | delivered to named/unnamed customer for evaluation |
| Qualification | environmental, reliability, interoperability test underway/passed |
| Low-volume manufacturing | repeatable line with customer-accepted shipments |
| HVM | sustained good-unit output, stable yield, automated test, multiple quarters revenue |
| Constrained HVM | HVM process exists but demand exceeds qualified supply |

### Supplier Data Request
| Metric | Unit | Reporting Frequency |
|---|---|---|
| Nameplate capacity | units/month or wafers/month | quarterly |
| Qualified capacity | customer-approved units/month | quarterly |
| Good-unit output | shipped accepted units/month | monthly |
| First-pass yield | % | monthly |
| Rework recovery | % | monthly |
| Cycle time | days from wafer start to shipment | monthly |
| Quoted lead time | weeks by SKU | monthly |
| On-time delivery | % | monthly |
| RMA / field failure | DPPM or FIT | quarterly |

### Bottleneck Ranking
| 2026 Rank | Bottleneck | Rationale |
|---:|---|---|
| 1 | advanced laser capacity | direct strategic investments and capacity rights |
| 2 | 200G/lane optical yield/test | 1.6T qualification dependency |
| 3 | CPO package/test/rework | no public HVM yield evidence |
| 4 | fiber/connectivity manufacturing | multiple multibillion hyperscaler commitments |
| 5 | leading-node DSP/SerDes allocation | shared with broader AI/custom silicon demand |

## Data Tables (where applicable)
| Field | Value | Source | Date |
|---|---|---|---|
| AAOI 800G capacity target | 100k modules/month | AAOI earnings coverage | 2025 year-end |
| AAOI US production target | ~35% | AAOI earnings coverage | 2025 |
| Fabrinet FY26 Q2 revenue | $1.13B | Fabrinet | 2026-02 |
| Fabrinet HPC revenue | $85.6M in FY26 Q2 | Fabrinet | 2026-02 |
| NVIDIA supplier investments | $2B each, COHR and LITE | NVIDIA/company announcements | 2026-03 |

## Open Questions / Gaps
- Confirm whether AAOI achieved its 100k/month target and identify the mix of DR4/DR8/2xFR4.
- Obtain Coherent/Lumentum fab locations, tool-install schedules, and qualified output.
- Quantify GF/AMF and TSMC photonics wafer capacity.
- Obtain first-pass yield, rework, cycle-time, and field-failure metrics under NDA.
- Build a monthly lead-time survey across lasers, DSPs, PICs, modules, connectors, and test gear.

## References
- AAOI capacity coverage | https://www.investors.com/news/technology/applied-optoelectronics-stock-aaoi-applied-optoelectronics-earnings-q32025/ | 2026-06-09
- Fabrinet ramp coverage | https://www.investors.com/research/the-new-america/fabrinet-stock-fn/ | 2026-06-09
- NVIDIA supplier agreements | https://www.wsj.com/tech/ai/nvidia-to-invest-2-billion-in-both-lumentum-and-coherent-b047f619 | 2026-06-09
- Meta-Corning agreement | https://www.wsj.com/tech/meta-enters-up-to-6-billion-data-center-fiber-optic-cable-deal-with-corning-4a085f73 | 2026-06-09
- Amazon-Corning agreement | https://www.wsj.com/tech/amazon-enters-agreement-with-corning-for-optical-fiber-for-data-centers-352c7fa7 | 2026-06-09
