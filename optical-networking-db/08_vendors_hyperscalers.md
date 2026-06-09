# Hyperscaler Optical Strategies
> **Last Updated:** 2026-06-09
> **Status:** Draft
> **Tags:** hyperscalers, cloud, custom-silicon, OCS, SONiC

## Overview
Hyperscalers shape optical demand through network topology, switch/NIC design, qualification rules, deployment cadence, and direct sourcing. Their public disclosures reveal broad direction but rarely complete supplier allocation, internal PIC work, or CPO schedules.

Vertical integration is strongest in switch/NIC software, telemetry, topology, and custom compute silicon. Optical-module and PIC design involvement varies by company and can include specifications, reference designs, co-design, direct component sourcing, or internal research rather than full manufacturing.

> 🔄 Refresh Needed: High Priority — reconcile internal program names, suppliers, and 2025-2026 deployments with current engineering publications and procurement disclosures.

## Key Findings / Highlights
- [CONFIRMED] Google’s Jupiter fabric and optical circuit switching research demonstrate long-running topology and OCS integration [Source: Google research/SIGCOMM, 2015-2022].
- [CONFIRMED] Meta has contributed FBOSS, Voyager, Cassini, and networking specifications through open ecosystems [Source: Meta/OCP, 2016-2024].
- [CONFIRMED] Microsoft originated SONiC and uses disaggregated networking broadly in Azure [Source: Microsoft, 2016-2024].
- [CONFIRMED] AWS designs Trainium/Inferentia and Nitro-related infrastructure; detailed optical and custom-SerDes ownership is less public.
- [ESTIMATED] Hyperscaler qualification scale and dual-sourcing requirements are major determinants of module vendor share and margins [HIGH confidence].

## Detailed Content
### Hyperscaler Matrix
| Hyperscaler | Internal Network Program | Optical Strategy | Key Suppliers | Custom Silicon | CPO Plans | Public Disclosures |
|---|---|---|---|---|---|---|
| Google | Jupiter; Apollo/Orion OCS references [verify naming] | custom topology, OCS, high-radix fabrics, DCI | not fully disclosed | TPU, NIC/network silicon programs | internal research/signals; [TO VERIFY] | SIGCOMM papers, cloud engineering |
| Meta | FBOSS, Minipack, Voyager, Cassini | open systems, 400G/ZR, OCP specifications | diversified; not fully disclosed | MTIA and network co-design | OCP/industry participation; [TO VERIFY] | Engineering blog, OCP |
| Microsoft | Azure DCI, SONiC | disaggregation, coherent DCI, custom systems | not fully disclosed | Maia/Cobalt and networking silicon work | research/partnership signals; [TO VERIFY] | Azure blog, research papers |
| Amazon AWS | Nitro, EFA, Trainium/Inferentia clusters | tightly integrated cloud fabric | not fully disclosed | extensive custom compute/NIC silicon | [TO VERIFY] | re:Invent and product docs |
| ByteDance | AI/cloud fabrics | high-volume 400G/800G sourcing [ESTIMATED] | China/global suppliers | limited public detail | [TO VERIFY] | sparse |
| Alibaba Cloud | HPN/cloud network; Hanguang/AI silicon | domestic and global optical ecosystem | Accelink/InnoLight ecosystem possible [RUMORED] | custom cloud/AI silicon | [TO VERIFY] | technical papers |
| Baidu | AI cloud and Kunlun clusters | high-bandwidth AI fabrics | not fully disclosed | Kunlun AI silicon | [TO VERIFY] | product/engineering material |

### Google Case Study
| Program | Function | Optical Relevance |
|---|---|---|
| Jupiter | warehouse-scale Clos fabric | repeated bandwidth generations and custom control |
| OCS deployments | reconfigurable optical circuits | bypass/reconfigure electrical switching paths |
| TPU pods | accelerator clusters | drives scale-out and scale-across traffic |
| Aquila | [TO VERIFY exact public program] | prompt-supplied custom NIC reference requires primary source |

### Meta Case Study
| Program | Contribution | Status |
|---|---|---|
| FBOSS | switch software | active/open-source ecosystem |
| Voyager | open packet-optical transport | historical OCP platform |
| Cassini | open modular packet/optical transponder | OCP/TIP ecosystem |
| 400G coherent | DCI and open line systems | public deployment direction; quantities [TO VERIFY] |

### Open Networking Implications
| Technology | Role | Optical Impact |
|---|---|---|
| SONiC | network OS disaggregation | broadens switch ODM ecosystem and module qualification |
| OpenConfig | vendor-neutral telemetry/config | consistent optical telemetry and automation |
| SAI | switch abstraction | separates NOS from ASIC SDK |
| OpenROAD | open physical-design flow | indirect; may lower custom-silicon barriers |
| CMIS | pluggable management | standardized module telemetry/control |

### Vertical Integration Levels
1. Architecture and traffic engineering.
2. NOS, telemetry, and automated operations.
3. Custom NIC/DPU and switch co-design.
4. Module specification and direct sourcing.
5. DSP/PIC design or joint development.
6. Manufacturing, generally retained by foundry/OSAT/module partners.

## Data Tables (where applicable)
| Field | Value | Source | Date |
|---|---|---|---|
| Google Jupiter publication | warehouse-scale fabric | Google/SIGCOMM | 2015 |
| Microsoft SONiC release | open network OS | Microsoft | 2016 |
| Meta Voyager | open packet optical | Meta/OCP | 2016 |
| Meta Cassini | modular transponder | TIP/OCP | 2019 |
| Google OCS paper | production optical circuit switching | Google/SIGCOMM | 2022 |

## Open Questions / Gaps
- Verify Google Orion/Aquila naming and scope.
- Identify disclosed module, laser, DSP, and switch suppliers by hyperscaler.
- Separate internal optical R&D from production deployment.
- Quantify custom PIC/DSP ownership and tape-outs.
- Track China hyperscaler procurement under export controls.

## References
- Google Research Publications | https://research.google/pubs/ | 2026-06-09
- Meta Engineering | https://engineering.fb.com/ | 2026-06-09
- Open Compute Project | https://www.opencompute.org/ | 2026-06-09
- SONiC | https://sonic-net.github.io/SONiC/ | 2026-06-09
- AWS Architecture | https://aws.amazon.com/architecture/ | 2026-06-09
- OpenConfig | https://www.openconfig.net/ | 2026-06-09
