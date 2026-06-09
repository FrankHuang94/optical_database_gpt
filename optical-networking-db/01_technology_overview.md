# Technology Overview
> **Last Updated:** 2026-06-09
> **Status:** Draft
> **Tags:** fundamentals, modulation, fiber, metrics, glossary

## Overview
An optical link converts electrical data into modulated light, transports it through fiber or waveguides, and recovers it with photodetectors, transimpedance amplifiers (TIAs), clock/data recovery, and often a digital signal processor (DSP). Datacenter links optimize cost, power, density, reach, latency, and reliability rather than maximum distance alone.

Short links commonly use multimode fiber (MMF) with VCSELs or single-mode fiber (SMF) with EML or silicon-photonic transmitters. Direct-detect PAM4 dominates modern intra-datacenter Ethernet, while coherent IQ modulation adds phase, amplitude, and polarization information for DCI and longer reaches [See: [07_coherent_vs_direct_detect.md](07_coherent_vs_direct_detect.md)].

## Key Findings / Highlights
- [CONFIRMED] PAM4 encodes two bits per symbol and enabled 50G, 100G, and emerging 200G electrical/optical lanes [Source: IEEE 802.3 standards, 2018-2024].
- [CONFIRMED] SMF offers much higher reach and bandwidth-distance headroom than MMF, while MMF can simplify short-reach optical assemblies [Source: IEEE 802.3, 2024].
- [CONFIRMED] Link budgets must include transmitter power, receiver sensitivity, connector/splice/coupling loss, and engineering margin.
- [ESTIMATED] End-to-end link energy, not isolated photonic-device energy, is the correct basis for architecture comparisons [Source: OIF/COBO presentations, 2023; HIGH confidence].
- [CONFIRMED] Pre-FEC BER, post-FEC BER, latency, and coding overhead must be reported together to compare links correctly.

## Detailed Content
### Optical Link Building Blocks
| Block | Function | Common Implementations | Primary Constraint |
|---|---|---|---|
| Laser | Generates optical carrier | VCSEL, DFB, EML source, external CW laser | efficiency, linewidth, lifetime |
| Modulator | Encodes data | EML, ring resonator, MZM | voltage, loss, bandwidth, linearity |
| Waveguide | Routes light on PIC | SOI silicon, SiN, InP | propagation and bend loss |
| Coupler | Connects PIC to fiber | grating, edge, lens/FAU | insertion loss, alignment yield |
| Detector | Converts photons to current | Ge-on-Si, InGaAs | responsivity, bandwidth, dark current |
| TIA/CDR/DSP | Recovers electrical bits | analog front-end, equalizer, FEC | power, latency, process node |

### Fiber Types
| Fiber | Typical Datacenter Role | Strength | Limitation |
|---|---|---|---|
| OM3/OM4/OM5 MMF | SR links, generally <=100 m class | mature VCSEL ecosystem | modal dispersion, connector count |
| OS2 SMF | DR/FR/LR and DCI | reach and WDM scalability | tighter coupling/alignment |
| Hollow-core fiber | Research/early deployment | lower latency and nonlinear potential | manufacturing, loss, splicing, cost |

### Modulation Comparison
| Format | Bits/Symbol | Detection | Typical Role | Caveat |
|---|---:|---|---|---|
| NRZ | 1 | direct | legacy 10G/25G and some optical lanes | lower spectral efficiency |
| PAM4 | 2 | direct | 50G-200G lanes | ~9.5 dB ideal eye-level penalty vs NRZ framing context varies |
| PAM6 | ~2.585 | direct | research/proposals | tighter SNR and linearity; no broad Ethernet baseline |
| Coherent QPSK/16QAM | 2/4 per polarization-symbol | coherent IQ | ZR/ZR+, metro/long-haul | DSP, laser, and power complexity |

### Key Metrics
| Metric | Unit | Interpretation |
|---|---|---|
| Bandwidth density | Tb/s/mm² or Tb/s per package edge | aggregate I/O per physical area |
| Reach | m or km | supported channel under specified loss/dispersion |
| Insertion loss | dB | passive optical power loss |
| BER | errors/bit | report pre-FEC and post-FEC |
| Energy efficiency | pJ/bit | include stated system boundary |
| OSNR | dB | signal-to-noise in reference optical bandwidth |
| Extinction ratio | dB | optical one/zero separation |
| TDECQ | dB | PAM4 transmitter quality penalty metric |

### Media Comparison
| Medium | Practical Reach | Density | Power | Cost | Best Fit |
|---|---|---|---|---|---|
| Passive DAC | ~1-3 m at highest rates | high | lowest | low | same-rack |
| ACC/AEC | ~3-7 m class | high | low-medium | medium | rack/adjacent rack |
| MMF optics | ~30-100 m class | medium-high | medium | medium | row-scale |
| SMF direct detect | 500 m-10 km class | high | medium-high | medium-high | fabric/campus |
| Coherent optics | ~40 km to long-haul | high spectral | high | high | DCI/metro |
| Wireless | niche | variable | variable | variable | management/specialized links |

### Glossary
| Term | Meaning |
|---|---|
| CPO | Co-Packaged Optics |
| LPO | Linear-Drive Pluggable Optics |
| EML | Electro-Absorption Modulated Laser |
| VCSEL | Vertical-Cavity Surface-Emitting Laser |
| SiPh | Silicon Photonics |
| DSP | Digital Signal Processor |
| TIA | Transimpedance Amplifier |
| CDR | Clock and Data Recovery |
| SerDes | Serializer/Deserializer |
| MSA | Multi-Source Agreement |
| OCS / ACS | Optical / all-optical circuit switching |
| WDM / CWDM / DWDM | Wavelength-division / coarse / dense WDM |
| MZM | Mach-Zehnder Modulator |
| PIC | Photonic Integrated Circuit |
| FEC | Forward Error Correction |
| IMDD | Intensity Modulation with Direct Detection |
| ZR / ZR+ | Coherent pluggable interoperability classes for DCI/metro |

## Data Tables (where applicable)
| Field | Value | Source | Date |
|---|---|---|---|
| PAM4 information | 2 bits/symbol | IEEE 802.3 | 2018-2024 |
| Common datacenter wavelength bands | ~850 nm MMF; ~1310 nm SMF; C-band coherent | IEEE/OIF | 2024 |
| 400G DR4 reach class | 500 m | IEEE 802.3bs | 2017 |
| 400G FR4 reach class | 2 km | 100G Lambda MSA / IEEE ecosystem | 2020 |
| 400ZR reach target | DCI class, commonly up to ~80-120 km depending link | OIF | 2020 |

## Open Questions / Gaps
- Normalize pJ/bit boundaries across vendor claims.
- Track PAM6 standardization or rejection relative to PAM4/coherent alternatives.
- Quantify hollow-core fiber lifecycle economics and connector reliability.
- Add representative link budgets for every Ethernet reach class.
- Add test methodology for TDECQ, COM, OSNR, and post-FEC error floors.

## References
- IEEE 802.3 | https://www.ieee802.org/3/ | 2026-06-09
- OIF implementation agreements | https://www.oiforum.com/technical-work/implementation-agreements-ias/ | 2026-06-09
- Fiber Optics 101, Corning | https://www.corning.com/optical-communications/worldwide/en/home/knowledge-center.html | 2026-06-09
- RP Photonics Encyclopedia | https://www.rp-photonics.com/ | 2026-06-09
- COBO | https://www.onboardoptics.org/ | 2026-06-09
