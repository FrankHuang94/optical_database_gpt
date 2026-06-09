# Standards and Multi-Source Agreements
> **Last Updated:** 2026-06-09
> **Status:** Draft
> **Tags:** IEEE-802.3, OIF, MSA, CMIS, Ethernet

## Overview
IEEE defines Ethernet PHYs and media specifications; OIF develops implementation agreements for interoperable electrical and coherent interfaces; MSAs define practical form factors, management interfaces, and optical specifications outside or ahead of formal standards. Product labels may combine an IEEE rate with an MSA reach and a form-factor specification.

Standards status must be tracked by approval date and revision. A task force being active does not mean products are interoperable, while an MSA specification does not carry the same governance or conformance structure as an IEEE standard.

> 🔄 Refresh Needed: High Priority — verify active 802.3dj, CEI-224G, 800ZR, CMIS, OSFP, and QSFP-DD revision status.

## Key Findings / Highlights
- [CONFIRMED] IEEE 802.3bs established 200/400GbE PHYs; 802.3cd covered 50/100/200GbE; 802.3ck specified 100G electrical lanes [Source: IEEE, 2017-2022].
- [CONFIRMED] IEEE 802.3df added 800GbE and related maintenance [Source: IEEE, 2024].
- [CONFIRMED] OIF 400ZR enabled interoperable coherent DCI pluggables [Source: OIF 400ZR IA, 2020].
- [CONFIRMED] CMIS is the common management model for modern high-speed pluggable modules [Source: OIF CMIS, 2024].
- [TO VERIFY] “1.6T OSFP” is an implementation ecosystem term; exact compliance depends on OSFP MSA revision, electrical interface, and optical specification.

## Detailed Content
### Standards Tracker
| Standard / Group | Bandwidth | Reach / Interface | Application | Status | Year Ratified / Baseline |
|---|---:|---|---|---|---:|
| IEEE 802.3bs | 200G/400G | 100 m to 10 km classes | Ethernet optics | [CONFIRMED] published | 2017 |
| IEEE 802.3cd | 50G/100G/200G | electrical/MMF/SMF PHYs | server and network links | [CONFIRMED] published | 2018 |
| IEEE 802.3ck | 100G/lane | chip-to-module/backplane/copper | 400G/800G electrical | [CONFIRMED] published | 2022 |
| IEEE 802.3df | 800G plus 200/400G work | multiple PMDs | 800GbE | [CONFIRMED] published | 2024 |
| IEEE 802.3dj | up to 1.6T | 200G/lane objectives | future Ethernet | active at baseline | expected [TO VERIFY] |
| OIF CEI-112G | 112G class | XSR/VSR/MR/LR electrical | chip/package/module | IA family published | 2022-2024 revisions |
| OIF CEI-224G | 224G class | electrical reaches | 1.6T ecosystem | active | [TO VERIFY] |
| OIF 400ZR | 400G | coherent DCI | router-to-router DCI | deployed IA | 2020 |
| OIF 800ZR | 800G | coherent DCI | next-gen DCI | development | [TO VERIFY] |

### MSA and Interface Ecosystem
| Group / Specification | Scope | Key Contribution | Status |
|---|---|---|---|
| QSFP-DD MSA | double-density QSFP | 8-lane pluggable mechanical/electrical | widely deployed |
| OSFP MSA | 8-lane pluggable | larger thermal envelope and roadmap | widely deployed at 800G |
| OSFP-XD | extra-density proposal | 16 electrical lanes / higher aggregate rate | emerging [TO VERIFY] |
| 100G Lambda MSA | optical PMDs | 100G/lambda DR/FR specifications | deployed ecosystem |
| OpenZR+ MSA | coherent pluggables | higher-performance modes beyond 400ZR | deployed/expanding |
| CMIS | module management | data model, applications, diagnostics | active revisions |
| MDIO | management bus | PHY management under IEEE 802.3 | mature |
| COBO | on-board optics | module and host concepts | limited adoption; CPO influence |

### Form Factor vs Optical Specification
| Layer | Example | Defines |
|---|---|---|
| Mechanical | OSFP, QSFP-DD | dimensions, connector/cage, thermal/mechanical |
| Electrical | IEEE 802.3ck, OIF CEI | host/module signaling and loss budgets |
| Optical PMD | 400GBASE-DR4, 800GBASE-DR8 | wavelength, lanes, reach, optical metrics |
| Management | CMIS | module controls, telemetry, applications |
| Coherent interoperability | 400ZR/OpenZR+ | framing, modulation, FEC, operational modes |

### Governance Notes
- IEEE standards use open task-force processes, objectives, ballots, and publication.
- OIF implementation agreements target multi-vendor interoperability and practical implementation.
- MSAs can move quickly but require careful revision and compliance tracking.
- Marketing names such as DR8, 2xFR4, LR8, and “ZR+” may not map one-to-one across suppliers.
- Host compliance does not guarantee end-to-end interoperability without firmware and management compatibility.

## Data Tables (where applicable)
| Field | Value | Source | Date |
|---|---|---|---|
| 400G Ethernet base standard | IEEE 802.3bs | IEEE | 2017 |
| 100G electrical lane | IEEE 802.3ck | IEEE | 2022 |
| 800G Ethernet | IEEE 802.3df | IEEE | 2024 |
| Coherent DCI IA | OIF 400ZR | OIF | 2020 |
| Module management | CMIS | OIF | active 2024 baseline |

## Open Questions / Gaps
- Record exact latest revision and approval date for every MSA.
- Add clause-level mapping from Ethernet PMDs to module marketing names.
- Track conformance test suites and interoperability events.
- Confirm OSFP-XD industry adoption and competing 3.2T proposals.
- Track 800ZR and 1.6T coherent project scope and completion.

## References
- IEEE 802.3 | https://www.ieee802.org/3/ | 2026-06-09
- IEEE Get Program | https://standards.ieee.org/products-programs/ieee-get-program/ | 2026-06-09
- OIF | https://www.oiforum.com/ | 2026-06-09
- QSFP-DD MSA | http://www.qsfp-dd.com/ | 2026-06-09
- OSFP MSA | https://osfpmsa.org/ | 2026-06-09
- OpenZR+ MSA | https://openzrplus.org/ | 2026-06-09
