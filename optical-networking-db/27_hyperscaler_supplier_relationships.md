# Hyperscaler Supplier Relationships
> **Last Updated:** 2026-06-09
> **Status:** In Review
> **Tags:** hyperscalers, suppliers, Corning, Coherent, Lumentum, evidence-map

## Overview
This file upgrades [08_vendors_hyperscalers.md](08_vendors_hyperscalers.md) from inferred strategy to an evidence-ranked relationship map. Optical procurement is usually confidential, so relationships are classified as contractual, named product adoption, company-identified customer, executive testimonial, or analyst inference.

The strongest 2026 disclosures are in fiber/connectivity and laser capacity: Meta and Amazon signed large Corning agreements, while NVIDIA committed capital and purchases to Coherent and Lumentum. Finished-transceiver allocations remain much less transparent.

> ⚠️ Note: An investment, testimonial, interoperability demo, or customer list does not prove current production revenue for a specific optical SKU.

## Key Findings / Highlights
- [CONFIRMED] Meta signed a multiyear Corning agreement worth up to $6B for US datacenter fiber, cable, and connectivity through 2030 [Source: Meta/Corning agreement reported 2026].
- [CONFIRMED] Amazon signed a multibillion-dollar Corning fiber/connectivity agreement announced June 8, 2026 [Source: Amazon/Corning announcement coverage, 2026-06-08].
- [CONFIRMED] NVIDIA committed $2B each to Coherent and Lumentum and entered multibillion-dollar nonexclusive purchase arrangements with capacity-access rights [Source: company announcements reported 2026-03].
- [CONFIRMED] NVIDIA named TACC, Oak Ridge, CoreWeave, and Lambda as prospective Quantum-X Photonics adopters [Source: NVIDIA SC25 disclosures].
- [ESTIMATED] Public evidence is strongest upstream because fiber and laser capacity require long-term commitments; module awards are more frequently confidential [HIGH confidence].

## Detailed Content
### Evidence Scale
| Grade | Evidence Type | Meaning |
|---|---|---|
| A | signed agreement with value/capacity or official named adoption | direct relationship confirmed |
| B | supplier/customer identified by company filing or official release | relationship confirmed, economics may be unknown |
| C | executive testimonial, qualification, or interoperability work | engagement signal, not purchase proof |
| D | analyst/channel inference | hypothesis only |

### Relationship Matrix
| Buyer / Platform | Supplier | Layer | Evidence | Grade | Date / Term |
|---|---|---|---|---|---|
| Meta | Corning | fiber, cable, connectivity hardware | up to $6B multiyear US datacenter agreement | A | announced 2026; through 2030 |
| Amazon | Corning | fiber, cable, connectivity | multibillion-dollar agreement; NC capacity expansion and 1,000 jobs | A | announced 2026-06-08 |
| NVIDIA | Coherent | advanced lasers and optical-networking product families | $2B investment plus multibillion-dollar purchase commitment/capacity rights | A | announced 2026-03 |
| NVIDIA | Lumentum | advanced laser systems/optics | $2B investment plus multibillion-dollar purchase commitment/capacity rights; new fab planned | A | announced 2026-03 |
| NVIDIA Quantum-X | TACC | CPO system adoption | named adopter | A/B | SC25; deployment timing 2026+ |
| NVIDIA Quantum-X | Oak Ridge National Laboratory | CPO system adoption | named adopter | A/B | SC25 |
| NVIDIA Quantum-X | CoreWeave | CPO system adoption | named adopter | A/B | SC25 |
| NVIDIA Quantum-X | Lambda | CPO system adoption | named adopter | A/B | SC25 |
| Amazon / Microsoft / Oracle | AAOI | optical modules | named as customers in secondary financial coverage; exact current SKU/volume confidential | B/C | 2025-2026 |
| ByteDance | Broadcom | CPO ecosystem | public executive testimonial for Broadcom CPO direction | C | 2024 |
| Google | Broadcom | custom accelerator/network silicon | long-running custom-silicon relationship; optical supplier scope not established | B for silicon; D for optics | ongoing |

### Hyperscaler Coverage
| Hyperscaler | Confirmed Optical Relationship | Unresolved Supplier Layers |
|---|---|---|
| Meta | Corning fiber/connectivity | 800G/1.6T modules, lasers, DSPs, CPO engines |
| Amazon AWS | Corning fiber/connectivity; AAOI relationship reported | allocation by module speed/reach and coherent DCI |
| Microsoft Azure | AAOI relationship reported | module allocation, coherent DSP, CPO partners |
| Google | internal network/OCS and custom-silicon disclosures | merchant transceivers, lasers, PICs, CPO |
| NVIDIA / AI cloud ecosystem | Coherent and Lumentum capacity; named Quantum-X adopters | optical-engine packaging and foundry allocation |
| ByteDance | Broadcom CPO public support | volume/order status and module vendors |
| Alibaba/Baidu | no high-confidence current public supplier map | domestic/global split under export controls |

### Corning Capacity Signals
| Agreement | Manufacturing Effect | Strategic Meaning |
|---|---|---|
| Meta, up to $6B | Meta expected as main customer at expanded Hickory, NC operation; workforce increase reported | long-duration US fiber/connectivity demand |
| Amazon, multibillion-dollar | North Carolina expansion and ~1,000 jobs | second major hyperscaler capacity commitment |
| NVIDIA, $500M investment reported | dedicated/expanded AI-fiber capacity | ties fiber supply to accelerated systems |

### NVIDIA Laser/Optics Capacity Signals
| Supplier | Capital | Purchase Commitment | Capacity Right | Facility Signal |
|---|---:|---|---|---|
| Coherent | $2B NVIDIA investment | multibillion-dollar, nonexclusive | future-product/capacity access | US manufacturing/R&D expansion |
| Lumentum | $2B NVIDIA investment | multibillion-dollar, nonexclusive | future-product/capacity access | new fabrication facility announced |

### What Remains Inference
- A hyperscaler investor in an optical startup is not automatically a production customer.
- A supplier's “cloud customer” disclosure does not identify the customer unless explicitly named.
- System-vendor optics may be sourced through ODMs or contract manufacturers, obscuring the end buyer.
- Direct laser/PIC sourcing can bypass the finished-module vendor and produce double-counting.
- Qualification can precede volume revenue by multiple quarters.

## Data Tables (where applicable)
| Field | Value | Source | Date |
|---|---|---|---|
| Meta-Corning maximum agreement | up to $6B | company/WSJ coverage | 2026 |
| Amazon-Corning agreement | multibillion-dollar | company/WSJ coverage | 2026-06-08 |
| NVIDIA-Coherent investment | $2B | company/WSJ coverage | 2026-03 |
| NVIDIA-Lumentum investment | $2B | company/WSJ coverage | 2026-03 |
| Named Quantum-X adopters | TACC, ORNL, CoreWeave, Lambda | NVIDIA SC25 | 2025 |

## Open Questions / Gaps
- Obtain official contract duration and minimum purchase schedules where public.
- Map module SKU/reach allocations by hyperscaler without relying on rumor.
- Separate direct component sourcing from ODM/module-vendor revenue.
- Add China hyperscaler relationships from filings and official tenders.
- Track whether NVIDIA's capacity rights constrain supply available to other buyers.

## References
- Meta-Corning coverage | https://www.wsj.com/tech/meta-enters-up-to-6-billion-data-center-fiber-optic-cable-deal-with-corning-4a085f73 | 2026-06-09
- Amazon-Corning coverage | https://www.wsj.com/tech/amazon-enters-agreement-with-corning-for-optical-fiber-for-data-centers-352c7fa7 | 2026-06-09
- NVIDIA-Coherent/Lumentum coverage | https://www.wsj.com/tech/ai/nvidia-to-invest-2-billion-in-both-lumentum-and-coherent-b047f619 | 2026-06-09
- NVIDIA Quantum-X adoption coverage | https://www.itpro.com/infrastructure/nvidia-announces-new-supercomputers-and-an-open-model-family-for-science-at-sc-2025 | 2026-06-09
- Broadcom Bailly coverage | https://www.investors.com/news/technology/broadcom-stock-avgo-bailly-cpo-ethernet-switch-ai/ | 2026-06-09
