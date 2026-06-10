# Full-System Power Benchmarks
> **Last Updated:** 2026-06-09
> **Status:** In Review
> **Tags:** power, CPO, LPO, pluggables, watts-per-terabit, measurement

## Overview
This file corrects a recurring comparison error in [17_power_and_thermal.md](17_power_and_thermal.md): module watts, optical-engine watts, port watts, and facility megawatts are not interchangeable. Every benchmark below declares its system boundary and evidence type.

Public 2025-2026 CPO comparisons are primarily vendor design models, not independent production measurements. No open, reproducible third-party dataset was found that compares equivalent 102.4T pluggable, LPO, and CPO switches under the same traffic, reach, ambient temperature, cooling, and redundancy conditions.

> ⚠️ Note: The absence of independent data is a material finding. Vendor claims are retained because they inform architecture, but they are not labeled “measured full-system” without test methodology.

## Key Findings / Highlights
- [CONFIRMED] NVIDIA compares approximately 30 W per 800G pluggable port with approximately 9 W for its CPO design, a 3.3x ratio consistent with its “3.5x power efficiency” claim [Source: NVIDIA Hot Chips/GTC disclosures, 2025].
- [CONFIRMED] NVIDIA cited electrical channel loss falling from roughly 22 dB to 4 dB, explaining reduced equalization/retiming power [Source: same].
- [CONFIRMED] Broadcom claimed Bailly's optical interconnect operates at 70% lower power than pluggable-transceiver alternatives [Source: Broadcom announcement, 2024].
- [ESTIMATED] Typical 800G DSP pluggable power remains roughly 14-20 W for many current modules, but 30 W is plausible for higher-power 200G/lane/future comparison boundaries [MED confidence].
- [CONFIRMED] OIF has defined EEI/CPO-related interfaces, but it does not provide a universal full-switch power benchmark.

## Detailed Content
### Evidence Hierarchy
| Tier | Evidence | Use |
|---|---|---|
| 1 | independent instrumented system test | preferred investment/procurement benchmark |
| 2 | vendor measured product datasheet under declared conditions | SKU comparison |
| 3 | vendor reference-design/model comparison | architecture planning only |
| 4 | component/device simulation | R&D potential, not system economics |
| 5 | unsourced marketing ratio | exclude |

### Published Comparison Register
| Source | Baseline | Alternative | Boundary | Result | Evidence Tier |
|---|---|---|---|---|---|
| NVIDIA | ~30 W/800G pluggable port | ~9 W/800G CPO port | switch optical I/O path as presented | ~3.3x lower; marketed as 3.5x efficiency | Tier 3 |
| NVIDIA | ~22 dB electrical loss | ~4 dB CPO electrical loss | ASIC-to-optics electrical channel | 18 dB reduction | Tier 3 |
| Broadcom Bailly | pluggable optical interconnect | CPO optical interconnect | optical interconnect portion | 70% lower power claim | Tier 3 |
| OIF 112G RTLR | fully retimed receive path | retimed transmitter / linear receiver | module interface architecture | avoids receiver-side retiming block | specification, not system benchmark |

### Normalized Calculations
| Case | Port Rate | Port Power | Optical-I/O Energy | 64-Port Total | Caveat |
|---|---:|---:|---:|---:|---|
| NVIDIA pluggable comparison | 800G | 30 W | 37.5 pJ/bit | 1.92 kW | vendor future/high-power baseline |
| NVIDIA CPO comparison | 800G | 9 W | 11.25 pJ/bit | 576 W | excludes/allocates shared system blocks per vendor boundary |
| Typical 800G pluggable range | 800G | 14-20 W | 17.5-25 pJ/bit | 896-1,280 W | module datasheet class, reach-dependent |
| Estimated 1.6T pluggable range | 1.6T | 20-30 W | 12.5-18.75 pJ/bit | 1.28-1.92 kW for 64 ports | not a specific measured SKU |

### Full-Switch Boundary
| Include | Why |
|---|---|
| switch ASIC core | CPO may change SerDes configuration and package thermals |
| host/package SerDes | main electrical-reach savings mechanism |
| module/optical engine | direct conversion power |
| external laser source | often omitted from CPO engine claims |
| voltage-regulator loss | architecture-dependent |
| fans/pumps/cold plate | thermal design can erase component savings |
| control/heaters/telemetry | ring and wavelength stabilization |
| redundancy/spares | ELS redundancy and failed-engine tolerance |

### Facility-Level Model
For a reproducible model:

```text
Facility power delta = (IT optical delta + switch/SerDes delta + cooling delta)
                     x deployment count
                     x PUE adjustment
```

NVIDIA's widely cited 400,000-GPU example compared approximately 72 MW for conventional networking with 21.6 MW for the photonics design. Treat this as a vendor scenario until port counts, topology, reach mix, utilization, redundancy, and cooling assumptions are published in a reproducible workbook.

### Required Lab Procedure
| Variable | Required Control |
|---|---|
| Rate/reach | same aggregate throughput and fiber reach |
| Traffic | idle, 50%, and line-rate bidirectional load |
| BER/FEC | same post-FEC target and margin |
| Temperature | same inlet and case temperature |
| Cooling | meter fans, pumps, and cold-plate loop |
| Laser | include wall-plug power and redundant source |
| Telemetry | record switch ASIC, SerDes, optics, regulators separately |
| Reliability | include failed-channel degradation and repair mode |

### Procurement Benchmark Schema
| Field | Unit |
|---|---|
| Total switch input power | W |
| Aggregate useful throughput | Tb/s after coding overhead |
| System energy | pJ/useful bit |
| Optical subsystem power | W |
| Cooling power | W |
| Inlet/coolant temperature | °C |
| Reach and fiber plant | m/km and loss dB |
| Post-FEC BER | errors/bit |
| Availability/repair model | hours and replaceable unit |

## Data Tables (where applicable)
| Field | Value | Source | Date |
|---|---|---|---|
| NVIDIA pluggable comparison | ~30 W/800G port | NVIDIA | 2025 |
| NVIDIA CPO comparison | ~9 W/800G port | NVIDIA | 2025 |
| NVIDIA channel-loss comparison | ~22 dB vs ~4 dB | NVIDIA | 2025 |
| Broadcom Bailly claim | 70% lower optical interconnect power | Broadcom | 2024 |
| Independent like-for-like dataset | not publicly found | research audit | 2026-06-09 |

## Open Questions / Gaps
- Obtain metered input power for shipping Bailly and Quantum-X/Spectrum-X systems.
- Allocate external-laser, pump, control, and cooling power consistently.
- Compare equivalent 102.4T pluggable, LPO, NPO, and CPO systems.
- Publish workload/topology assumptions behind the 72 MW versus 21.6 MW NVIDIA scenario.
- Add failure-adjusted energy and total cost, not only steady-state watts.

## References
- NVIDIA Hot Chips roadmap coverage | https://www.tomshardware.com/networking/nvidia-outlines-plans-for-using-light-for-communication-between-ai-gpus-by-2026-silicon-photonics-and-co-packaged-optics-may-become-mandatory-for-next-gen-ai-data-centers | 2026-06-09
- Broadcom Bailly coverage | https://www.investors.com/news/technology/broadcom-stock-avgo-bailly-cpo-ethernet-switch-ai/ | 2026-06-09
- OIF Implementation Agreements | https://www.oiforum.com/technical-work/implementation-agreements-ias/ | 2026-06-09
- OSFP MSA | https://osfpmsa.org/ | 2026-06-09
