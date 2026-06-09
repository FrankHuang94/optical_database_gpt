# Regulatory and Standards Bodies
> **Last Updated:** 2026-06-09
> **Status:** Draft
> **Tags:** IEEE, OIF, ETSI, ITU-T, OCP, UEC, export-controls

## Overview
Standards bodies coordinate interoperable Ethernet, electrical I/O, coherent optics, management, and network architecture. Regulatory policy affects trade, advanced-semiconductor access, cybersecurity, energy use, and domestic manufacturing. Technical and legal status can change independently.

This tracker is informational, not legal advice. Export-control classification depends on product specifications, destination, end user, and end use; Entity List presence does not by itself describe every permitted or prohibited transaction.

> 🔄 Refresh Needed: High Priority — update standards milestones, consortium membership, BIS rules, Entity List entries, and CHIPS awards.

## Key Findings / Highlights
- [CONFIRMED] IEEE 802.3df delivered 800GbE; 802.3dj addresses 200G/lane and 1.6TbE objectives.
- [CONFIRMED] OIF coordinates CEI electrical interfaces, coherent ZR, CMIS, CPO, and external-laser work.
- [CONFIRMED] OCP publishes open hardware/software designs including networking systems and SAI-related work.
- [CONFIRMED] UEC targets Ethernet improvements for AI/HPC.
- [CONFIRMED] US export controls and CHIPS incentives can affect the same supply chain in opposite directions: restricting selected transfers while subsidizing domestic capacity.

## Detailed Content
### IEEE 802.3 Tracker
| Group | Topic | Speed Target | Status | Expected Completion |
|---|---|---:|---|---|
| 802.3bs | 200/400GbE | 400G | complete | 2017 |
| 802.3cd | 50/100/200GbE | 200G | complete | 2018 |
| 802.3ck | 100G electrical lanes | 100G/lane | complete | 2022 |
| 802.3df | 800GbE | 800G | complete | 2024 |
| 802.3dj | 200G/lane Ethernet | up to 1.6T | active at baseline | [TO VERIFY] |

### OIF Tracker
| Project | Description | Status | Members / Ecosystem |
|---|---|---|---|
| CEI-112G | common electrical interfaces | IAs published | semiconductor/system vendors |
| CEI-224G | next electrical generation | active [TO VERIFY] | broad ecosystem |
| 400ZR | interoperable coherent DCI | deployed | module/DSP/system vendors |
| 800ZR | next coherent rate | active [TO VERIFY] | coherent ecosystem |
| CMIS | pluggable management | active revisions | host/module vendors |
| CPO / ELSFP | co-packaging and external lasers | framework/projects active | switch/optics vendors |

### Other Standards Organizations
| Body | Relevant Group | Datacenter Optical Role |
|---|---|---|
| ITU-T | SG15 | optical transport, interfaces, fiber |
| ETSI | ISG NFV, MEC, sustainability groups | network architecture/energy context |
| IETF | routing, congestion, YANG/telemetry | protocols above optical PHY |
| OCP | Networking, hardware management | open switches, specifications, operations |
| UEC | AI/HPC Ethernet | transport, congestion, APIs |
| UALink Consortium | accelerator interconnect | scale-up; future optical relevance |

### OCP Initiatives
| Initiative | Role | Optical Relevance |
|---|---|---|
| SAI | switch abstraction interface | NOS/ASIC interoperability |
| FBOSS / SONiC ecosystem | open network software | module telemetry and qualification |
| Goldstone | open NOS for optical systems | coherent/open line systems |
| open switch designs | disaggregated hardware | cages, thermals, module standards |
| hardware management | telemetry/control | CMIS and failure operations |

### UEC
UEC membership includes major cloud, semiconductor, systems, and networking companies; the exact list changes and should be imported from the official site. Its relationship to optics is indirect but important: link rates, congestion control, reliability, telemetry, and topology determine optical port count and utilization.

### US Export Controls
| Instrument | Mechanism | Optical Impact |
|---|---|---|
| EAR / Commerce Control List | product classification and licensing | advanced DSP, equipment, technology transfer |
| Entity List | party-specific license requirements | customer/supplier restrictions |
| advanced-computing rules | performance/end-use controls | AI systems and associated supply chain |
| sanctions/OFAC | person/country restrictions | transactions and financing |

### China Industrial Policy
China’s MIIT and broader national/local programs support optical communications, compound semiconductors, datacenters, and domestic substitution. Relevant vendors include InnoLight, Accelink, Eoptolink, HG Genuine, and Source Photonics-linked operations. Quantified “substitution targets” require primary Chinese policy documents, not press summaries.

### CHIPS and Science Act
| Program | Relevance | Evidence Needed |
|---|---|---|
| CHIPS incentives | domestic fabs and packaging | award-by-award photonics allocation |
| National Semiconductor Technology Center | R&D and prototyping | photonics program scope |
| AIM Photonics | SiPh PDK, packaging, test, workforce | funding and capacity milestones |
| defense/dual-use programs | trusted photonics supply | contract-specific details |

## Data Tables (where applicable)
| Field | Value | Source | Date |
|---|---|---|---|
| 800GbE standard | IEEE 802.3df | IEEE | 2024 |
| Future Ethernet project | IEEE 802.3dj | IEEE | active 2024 baseline |
| AI Ethernet consortium | UEC | UEC | formed 2023 |
| US export regulator | BIS | US Department of Commerce | current |
| US SiPh institute | AIM Photonics | AIM/DoD | active |

## Open Questions / Gaps
- Import exact current IEEE/OIF milestones and completion dates.
- Maintain versioned UEC/OIF/OCP member lists.
- Build a legal-reviewed export classification and restricted-party workflow.
- Source China policy targets from original-language documents.
- Map CHIPS awards to actual photonics tools, wafers, packaging, and jobs.

## References
- IEEE 802.3 | https://www.ieee802.org/3/ | 2026-06-09
- OIF | https://www.oiforum.com/ | 2026-06-09
- ITU-T SG15 | https://www.itu.int/en/ITU-T/studygroups/2022-2024/15/ | 2026-06-09
- Open Compute Project | https://www.opencompute.org/ | 2026-06-09
- Ultra Ethernet Consortium | https://ultraethernet.org/ | 2026-06-09
- BIS | https://www.bis.gov/ | 2026-06-09
- CHIPS for America | https://www.nist.gov/chips | 2026-06-09
