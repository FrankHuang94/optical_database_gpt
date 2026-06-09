# Transceiver Form Factors
> **Last Updated:** 2026-06-09
> **Status:** Draft
> **Tags:** pluggables, OSFP, QSFP-DD, thermal, density

## Overview
A transceiver form factor defines mechanical envelope, host connector, electrical lanes, thermal assumptions, and management conventions; optical reach specifications are separate. QSFP-derived formats optimize installed-base compatibility and density, while OSFP provides a larger thermal envelope favored in many 800G AI systems.

At 1.6T and beyond, front-panel area, connector count, airflow, module power, cage loss, and electrical channel reach become system constraints. This intensifies the debate among conventional DSP pluggables, LPO, on-board optics (OBO), and CPO [See: [17_power_and_thermal.md](17_power_and_thermal.md)].

> 🔄 Refresh Needed: High Priority — validate 1.6T module power and OSFP-XD status from current MSA revisions and shipping products.

## Key Findings / Highlights
- [CONFIRMED] QSFP-DD and OSFP both expose eight high-speed electrical lanes and support 400G/800G implementations [Source: respective MSAs, 2024].
- [CONFIRMED] OSFP's larger body supports a higher thermal envelope than QSFP-derived formats.
- [CONFIRMED] CFP2 remains important for coherent transport even as client optics favor QSFP-DD/OSFP.
- [ESTIMATED] 800G DSP pluggables commonly operate around 14-20 W depending reach and design [Source: vendor datasheets, 2023-2024; MED confidence].
- [ESTIMATED] 1.6T pluggables often target roughly 20-30 W envelopes; exact values require product-level validation [LOW confidence].

## Detailed Content
### Form Factor Comparison
| Form Factor | Max Speed | Lanes | Power (W) | Approx. Dimensions / Envelope | Key Vendors | Volume Status | Notes |
|---|---:|---:|---:|---|---|---|---|
| SFP-DD | 100G/200G class | 2 | ~3-6 | SFP-derived | Molex, Amphenol ecosystem | niche | higher-density server links |
| QSFP28 | 100G | 4 | ~3.5-6 | ~18.35 x 72 x 8.5 mm module body class | broad | mature | 4x25G |
| QSFP56 | 200G | 4 | ~5-8 | QSFP | broad | mature | 4x50G PAM4 |
| QSFP-DD | 400G/800G | 8 | ~12-20 | QSFP double-density | broad | volume | backward-compatible cage concept varies |
| QSFP112 | 400G | 4 | ~10-14 | QSFP | broad | volume/expanding | 4x100G |
| OSFP | 800G/1.6T roadmap | 8 | ~15-30 | ~22.6 x 107.8 x 13.0 mm class | NVIDIA, Innolight, Coherent | 800G volume | thermal headroom |
| OSFP-XD | 3.2T proposal | 16 | [TO VERIFY] | extended-density OSFP | MSA ecosystem | emerging | 16 electrical lanes |
| CDFP | 400G historical | 16 | ~20+ | large | legacy ecosystem | [DEPRECATED] | early 400G concept |
| CFP2 | 400G/800G coherent class | varies | ~20-30+ | transport-oriented | Ciena, Cisco, Nokia ecosystem | active coherent | high thermal envelope |
| CFP8 | 400G | 16 | ~15-25 | large | legacy ecosystem | limited/[DEPRECATED] | early 400G |

> ⚠️ Note: “Max speed” reflects ecosystem roadmaps, not guaranteed compatibility. Power varies materially by reach, temperature class, DSP, and optics.

### Optical Implementations
| Optical Type | Aggregate | Optical Lanes | Fiber | Nominal Reach Class |
|---|---:|---:|---|---:|
| 800G-DR8 | 800G | 8x100G | 8-pair SMF / MPO | 500 m |
| 800G-SR8 | 800G | 8x100G | parallel MMF | ~100 m class |
| 800G 2xFR4 | 800G | 2 groups of 4 WDM lanes | duplex SMF variants | 2 km class |
| 1.6T-DR8 | 1.6T | 8x200G | parallel SMF | 500 m target class [TO VERIFY] |
| 1.6T 2xFR4 | 1.6T | 8x200G WDM grouping | duplex/dual duplex | 2 km target [TO VERIFY] |

### Pluggable vs OBO
| Dimension | Pluggable | OBO |
|---|---|---|
| Serviceability | field replaceable | board replacement/rework |
| Electrical reach | longest host trace | shorter |
| Thermal location | faceplate airflow competition | distributed board cooling |
| Vendor modularity | high | tighter system integration |
| Faceplate density | cage-limited | fiber connector still constrained |
| Upgrade cycle | optics separable from switch | coupled to board |

### Power Trend
| Generation | Indicative Module Power | Normalized W/400G | Status |
|---|---:|---:|---|
| 400G DR4/FR4 | ~8-14 W | ~8-14 | [ESTIMATED] product dependent |
| 800G DR8/2xFR4 | ~14-20 W | ~7-10 | [ESTIMATED] |
| 1.6T | ~20-30 W | ~5-7.5 | [ESTIMATED][LOW confidence] |

### Density and Thermal Constraints
- A 1RU switch faceplate must allocate space to cages, fiber connectors, status/retention features, fans, and service access.
- Module heat recirculation can make center cages hotter than edge cages.
- Finned OSFP modules can use system airflow; flat-top versions depend more on cage/host cooling.
- Liquid-cooled accelerator racks complicate airflow assumptions for front-panel optics.
- MPO connector cleanliness and high fiber counts create operational overhead.

## Data Tables (where applicable)
| Field | Value | Source | Date |
|---|---|---|---|
| QSFP-DD electrical lanes | 8 | QSFP-DD MSA | 2024 |
| OSFP electrical lanes | 8 | OSFP MSA | 2024 |
| Common 800G mapping | 8x100G | IEEE/MSA ecosystem | 2023-2024 |
| Emerging 1.6T mapping | 8x200G | IEEE 802.3dj ecosystem | 2024 |
| 800G module power range | ~14-20 W [ESTIMATED] | vendor datasheets | 2023-2024 |

## Open Questions / Gaps
- Populate exact dimensions and thermal classes from current MSA documents.
- Track shipping 1.6T SKUs, qualification status, and measured power.
- Compare connector/fiber-count economics for DR8, 2xFR4, and WDM variants.
- Quantify field failure and replacement costs for OBO/CPO.
- Determine whether OSFP-XD or another format wins 3.2T.

## References
- OSFP MSA | https://osfpmsa.org/ | 2026-06-09
- QSFP-DD MSA | http://www.qsfp-dd.com/ | 2026-06-09
- IEEE 802.3 | https://www.ieee802.org/3/ | 2026-06-09
- OIF CMIS | https://www.oiforum.com/technical-work/implementation-agreements-ias/ | 2026-06-09
- COBO | https://www.onboardoptics.org/ | 2026-06-09
