# Co-Packaged Optics
> **Last Updated:** 2026-06-09
> **Status:** Draft
> **Tags:** CPO, optical-I-O, switch-ASIC, packaging, external-laser

## Overview
Co-packaged optics places optical engines adjacent to a switch or compute ASIC on a shared package substrate or tightly integrated assembly. The objective is to replace long, power-hungry high-speed electrical paths to front-panel modules with short electrical connections and optical fiber leaving the package.

CPO can improve bandwidth density and electrical I/O energy, but total system benefit depends on laser power, thermal control, fiber attach, manufacturing yield, redundancy, field repair, and switch lifecycle. Optical I/O chiplets apply related concepts to accelerator-to-accelerator and memory fabrics [See: [18_AI_datacenter_architecture.md](18_AI_datacenter_architecture.md)].

> 🔄 Refresh Needed: High Priority — verify every 2025-2026 CPO product announcement, launch date, performance claim, and customer deployment.

## Key Findings / Highlights
- [CONFIRMED] CPO shortens the high-speed electrical path between ASIC and optical engine [Source: OIF CPO Framework, 2023].
- [CONFIRMED] External laser source modules can improve serviceability and isolate laser heat/reliability from the switch package.
- [CONFIRMED] Package-level yield is multiplicative: failure of one expensive die or optical engine can affect the value of the full assembly.
- [ESTIMATED] CPO becomes more compelling as switch bandwidth reaches 102.4T and 204.8T and electrical lanes move to 224G [MED confidence].
- [TO VERIFY] NVIDIA's 2025 silicon-photonics Quantum/Spectrum-X announcement cited up to roughly 3.5x power efficiency improvement; system boundary and production status must be checked against the official launch materials.

## Detailed Content
### Architecture
| Element | Role | Design Issue |
|---|---|---|
| Switch ASIC | packet forwarding / SerDes | heat flux and package edge bandwidth |
| Optical engine | E/O and O/E conversion | yield, wavelength control, replaceability |
| External laser source | CW optical power | redundancy, connector safety, distribution loss |
| Fiber attach unit | package-to-fiber connection | alignment, contamination, rework |
| Package substrate/interposer | electrical and mechanical integration | warpage, signal integrity, cost |
| Control/telemetry | bias, temperature, alarms | calibration and failure isolation |

### CPO vs Pluggable
| Dimension | Pluggable | CPO |
|---|---|---|
| Electrical path | ASIC-board-cage-module | very short package path |
| I/O energy | higher at fastest lanes | potentially lower |
| Serviceability | replace individual module | package/system repair complexity |
| Yield isolation | known-good module | integrated assembly yield risk |
| Thermal environment | faceplate | near hot ASIC |
| Vendor interchangeability | relatively high | tighter co-design |
| Time to market | mature ecosystem | longer qualification |
| Latency | DSP-dependent | architecture-dependent; potentially lower |

### Player Approaches
| Player | Program / Product | Approach | Baseline Status |
|---|---|---|---|
| Broadcom | Tomahawk/Trident CPO demonstrations and Bailly-related ecosystem | switch ASIC + co-packaged optical engines | demonstrated / roadmap [TO VERIFY] |
| Intel | Integrated Photonics Solutions work | SiPh engines and CPO research/products | active technology; strategy evolving |
| Ayar Labs | TeraPHY + SuperNova | optical I/O chiplet + external laser | sampling/partnerships [TO VERIFY] |
| Ranovus | Odin/ORON platform | multi-terabit optical engine / CPO module | demonstrations and partnerships |
| Celestial AI | Photonic Fabric | optical scale-up/memory connectivity | development; private company |
| Lightmatter | Passage | photonic interconnect fabric | development/sampling [TO VERIFY] |
| NVIDIA | silicon-photonics Quantum-X/Spectrum-X switches | integrated optics for AI fabrics | announced 2025 [TO VERIFY production] |

### Switch Roadmap
| Switch Capacity | Typical Front-Panel Equivalent | CPO Relevance | Expected Window |
|---:|---|---|---|
| 51.2T | 64x800G | pluggables remain practical | 2023-2025 |
| 102.4T | 64x1.6T | stronger thermal/electrical case | 2025-2027E |
| 204.8T | 128x1.6T or 64x3.2T | CPO/optical I/O increasingly likely | 2027+ [LOW confidence] |

### Production Readiness Checklist
- Known-good-die screening before assembly.
- Passive and active optical alignment with rework strategy.
- Laser redundancy and hot-swap design.
- Thermal isolation between switch ASIC, rings, lasers, and TIAs.
- Fiber attach reliability under shock, vibration, and repeated service.
- Package test coverage for every wavelength/channel.
- Field-failure containment without replacing the entire switch.

### Hyperscaler Signals
| Organization | Public Signal | Interpretation |
|---|---|---|
| Microsoft | research/industry participation in CPO and optical networking | interest; deployment details limited |
| Google | OCS and custom network architecture; SiPh research footprint | strong optical integration capability; CPO specifics limited |
| Meta | OCP networking and optical specifications | ecosystem influence; internal CPO status [TO VERIFY] |
| Cloud industry | OIF/COBO/OCP participation | requirements shaping rather than proof of volume adoption |

### Standards Work
OIF has published CPO framework and external laser source work. COBO and OCP provide related implementation forums. The prompt's reference to an “IEEE 802.3 CPO study group” requires exact project verification; IEEE Ethernet projects often specify interfaces and PHY objectives rather than package architecture itself.

## Data Tables (where applicable)
| Field | Value | Source | Date |
|---|---|---|---|
| CPO framework | OIF CPO Framework IA | OIF | 2023 |
| External laser work | OIF ELSFP projects | OIF | 2022-2024 |
| Current switch baseline | 51.2 Tb/s | Broadcom/NVIDIA | 2023-2024 |
| Next switch class | 102.4 Tb/s [roadmap] | vendor roadmaps | 2024-2025 |
| NVIDIA efficiency claim | up to ~3.5x [TO VERIFY scope] | NVIDIA announcement | 2025 |

## Open Questions / Gaps
- Obtain measured switch-level watts/Tb rather than component claims.
- Quantify package yield, rework rate, and field replacement economics.
- Verify production dates and customer deployments for each named platform.
- Determine standards-based interoperability boundaries for optical engines and lasers.
- Track laser safety, connector, and redundant-source requirements.

## References
- OIF Co-Packaging | https://www.oiforum.com/technical-work/hot-topics/co-packaging/ | 2026-06-09
- Broadcom CPO | https://www.broadcom.com/solutions/data-center/co-packaged-optics | 2026-06-09
- Ayar Labs | https://ayarlabs.com/ | 2026-06-09
- Ranovus | https://ranovus.com/ | 2026-06-09
- Lightmatter Passage | https://lightmatter.co/ | 2026-06-09
- NVIDIA Networking | https://www.nvidia.com/en-us/networking/ | 2026-06-09
