# 2026 IEEE and OIF Status
> **Last Updated:** 2026-06-09
> **Status:** In Review
> **Tags:** IEEE-802.3dj, OIF, 800ZR, 1600ZR, CEI, CMIS, standards

## Overview
This dated tracker supersedes the status fields in [03_standards_and_msa.md](03_standards_and_msa.md). It records published implementation agreements separately from active projects and draft standards.

IEEE P802.3dj has advanced substantially: Draft 3.0 entered IEEE Standards Association ballot in 2026. OIF has published 800ZR, 800LR, updated 400ZR, ELSFP 2.0, CEI 5.3, RTLR, and CMIS 5.4 while opening work on 448G electrical interfaces, compute optics, NPO, 1600ZR, and 1600ZR+.

> ⚠️ Note: IEEE draft content can still change until Standards Board approval. OIF “current work” is not an approved implementation agreement.

## Key Findings / Highlights
- [CONFIRMED] IEEE P802.3dj Draft 3.0 was in Standards Association ballot by March-June 2026 [Source: IEEE 802.3dj comments register, 2026-06-04].
- [CONFIRMED] The adopted 802.3dj timeline targets standards completion in 2026, subject to ballot resolution and Standards Board approval [Source: IEEE adopted timeline, 2024-11-14].
- [CONFIRMED] OIF-800ZR-01.0 was published in October 2024 and OIF-800LR-01.0 in April 2025 [Source: OIF IA register].
- [CONFIRMED] CMIS 5.4 was published in May 2026 [Source: OIF IA register].
- [CONFIRMED] OIF's active portfolio includes 1600ZR, 1600ZR+, 1600CL, 12.8T NPO, Compute Optics Interface, and 448G signaling work [Source: OIF Current Work, 2026].

## Detailed Content
### IEEE 802.3 Status
| Project | Scope | Current Stage | Latest Public Evidence | Expected Completion |
|---|---|---|---|---|
| IEEE 802.3bs | 200/400GbE | [CONFIRMED] published | IEEE standard | 2017 complete |
| IEEE 802.3cd | 50/100/200GbE | [CONFIRMED] published | IEEE standard | 2018 complete |
| IEEE 802.3ck | 100G electrical lanes | [CONFIRMED] published | IEEE standard | 2022 complete |
| IEEE 802.3df | 800GbE | [CONFIRMED] published | IEEE standard | 2024 complete |
| IEEE P802.3dj | 200G, 400G, 800G, 1.6T Ethernet | [CONFIRMED] Draft 3.0 SA ballot | comments received 2026-03-30; unsatisfied list 2026-06-04 | 2026 target; not yet final |

### 802.3dj Ballot Record
| Milestone | Date | Interpretation |
|---|---|---|
| Draft 2.0 Working Group ballot comments | 2025-06-16 | WG ballot phase began |
| Draft 2.4 | 2026-02-13 | zero comments received |
| Draft 3.0 SA ballot comments received | 2026-03-30 | entered Standards Association ballot |
| Draft 3.0 final responses | 2026-05-18 | comment resolution progressed |
| Draft 3.0 unsatisfied comments list | 2026-06-04 | project not yet final |

### Published OIF Agreements
| Document | Scope | Publication | Status |
|---|---|---:|---|
| OIF-800ZR-01.0 | interoperable 800G coherent DCI | 2024-10 | [CONFIRMED] published |
| OIF-400ZR-03.0 | updated 400ZR | 2024-10 | [CONFIRMED] published |
| OIF-800LR-01.0 | 800G coherent light/reach interface | 2025-04 | [CONFIRMED] published |
| OIF-ELSFP-02.0 | external laser small form factor pluggable | 2025-01 | [CONFIRMED] published |
| OIF-EEI-112G-RTLR-01.0 | 112G retimed transmitter / linear receiver | 2025-10 | [CONFIRMED] published |
| OIF-CEI-05.3 | CEI through 112G+ classes | 2025-07 | [CONFIRMED] published; not a 224G IA |
| OIF-CMIS-05.4 | common module management | 2026-05 | [CONFIRMED] published |
| OIF-C-CMIS-01.4 | coherent CMIS | 2025-04 | [CONFIRMED] published |
| OIF-CMIS-VCS-01.1 | versatile control set | 2025-07 | [CONFIRMED] published |

### Active OIF Work
| Project | Target | Current Meaning |
|---|---|---|
| 448G signaling workshop/project work | future AI electrical I/O | research and requirements stage; no published CEI-448G IA found |
| 12.8T NPO module | 12.8T and 6.4T, 200G/lane | mechanical, electrical, liquid cooling, laser, power, connector IA development |
| Compute Optics Interface | PCIe/NVLink/UALink optical scale-up | low-latency photonic interface project |
| 1600CL | power/latency optimized campus links | coherent-light project building on 800LR |
| 1600ZR | 1.6T DP-16QAM, up to 120 km amplified DCI target | active IA development |
| 1600ZR+ | 1.6T up to 1,000 km; 1.2T up to 2,000 km target | active IA development |
| 1.6T pluggable MACsec | security profile | technical white paper project |

### Corrected Terminology
| Prior Database Phrase | Correct 2026 Treatment |
|---|---|
| “CEI-224G active” | OIF publicly lists CEI 5.3 through 112G+; future 224G/448G work must be tracked by named project and published IA status |
| “800ZR developing” | [DEPRECATED] status; 800ZR IA published October 2024 |
| “CMIS 5.3 latest” | [DEPRECATED] status; CMIS 5.4 published May 2026 |
| “802.3dj active” | too broad; currently Draft 3.0 SA ballot, not ratified |
| “IEEE CPO study group” | no separate current IEEE CPO standard identified; Ethernet PHY work and OIF EEI/CPO work should not be conflated |

## Data Tables (where applicable)
| Field | Value | Source | Date |
|---|---|---|---|
| 802.3dj current draft | D3.0 | IEEE comments register | 2026-06-04 |
| 800ZR publication | OIF-800ZR-01.0 | OIF | 2024-10 |
| 800LR publication | OIF-800LR-01.0 | OIF | 2025-04 |
| CMIS latest public revision | 5.4 | OIF | 2026-05 |
| NPO target | 12.8T / 6.4T at 200G/lane | OIF | active 2026 |

## Open Questions / Gaps
- Record final 802.3dj approval date and amendment number when published.
- Track whether OIF publishes CEI agreements explicitly covering 224G and 448G classes.
- Add clause-level 802.3dj PMD and reach mapping after final approval.
- Track 1600ZR/1600ZR+ ballot and interoperability milestones.
- Update OSFP, QSFP-DD, OpenZR+, and CMIS revision compatibility together.

## References
- IEEE P802.3dj Task Force | https://www.ieee802.org/3/dj/ | 2026-06-09
- IEEE P802.3dj Comments | https://www.ieee802.org/3/dj/comments/index.html | 2026-06-09
- IEEE P802.3dj Adopted Timeline | https://www.ieee802.org/3/dj/projdoc/timeline_3dj_241114.pdf | 2026-06-09
- OIF Implementation Agreements | https://www.oiforum.com/technical-work/implementation-agreements-ias/ | 2026-06-09
- OIF Current Work | https://www.oiforum.com/technical-work/current-work/ | 2026-06-09
