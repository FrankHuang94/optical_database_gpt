# Power and Thermal
> **Last Updated:** 2026-06-09
> **Status:** Draft
> **Tags:** power, thermal, pJ-per-bit, liquid-cooling, LPO, CPO

## Overview
Optical power must be measured at a declared boundary: photonic device, optical engine, module, switch I/O, or full cooled system. Module-only comparisons can omit host SerDes, retimers, laser sources, regulators, and cooling overhead.

As AI racks adopt liquid cooling for accelerators, front-panel optics often remain air-cooled, creating a mixed thermal architecture. Higher module power also reduces allowable ambient temperature, port density, or fan efficiency.

> 🔄 Refresh Needed: High Priority — populate measured product power at common temperature, reach, traffic, and FEC conditions.

## Key Findings / Highlights
- [CONFIRMED] DSP and high-speed electrical I/O are major power contributors in modern pluggable links.
- [ESTIMATED] LPO can reduce module power by removing the module DSP, but shifts equalization burden and link-margin risk to the host [HIGH confidence].
- [ESTIMATED] CPO can reduce switch I/O energy by shortening electrical reach; whole-system savings depend on lasers, control, cooling, and redundancy [MED confidence].
- [CONFIRMED] pJ/bit improves with aggregate speed even when absolute module watts rise.
- [CONFIRMED] Integrated voltage regulation and power integrity become harder near high-current ASIC/optical packages.

## Detailed Content
### Indicative Port Power
| Speed | DSP Pluggable Power (W) | LPO Power (W) | CPO Optical Portion (W equivalent/port) | Power/Bit (pJ/bit) |
|---:|---:|---:|---:|---:|
| 400G | 8-14 | 5-9 | 3-7 | 20-35 pluggable |
| 800G | 14-20 | 8-12 | 5-10 | 17.5-25 pluggable |
| 1.6T | 20-30 | 12-20 | 8-16 | 12.5-18.8 pluggable |

> ⚠️ Note: [ESTIMATED] ranges are architecture-level placeholders. CPO “per port” allocation is artificial because engines, lasers, and switch cooling are shared.

### System Power Stack
| Contributor | Pluggable | LPO | CPO |
|---|---|---|---|
| Host SerDes | long-reach/high power | linear-compatible/high quality | short-reach/lower target |
| Module DSP | present | removed/reduced | architecture dependent |
| Drivers/TIAs | present | linear analog | optical engine |
| Laser | internal/external | internal/external | commonly external shared |
| Thermal control | module | module | package/engine wavelength control |
| Cooling | cage/front panel | cage/front panel | package plus laser module |

### Thermal Management
| Method | Benefit | Limitation |
|---|---|---|
| High-airflow heat sinks | mature and serviceable | fan power/noise and air-temperature limits |
| Heat pipes/vapor chambers | spread module/ASIC heat | mechanical integration |
| Cold plates | high heat removal | difficult at pluggable faceplate |
| Immersion cooling | whole-system heat transfer | optical connector/material compatibility |
| Rear-door heat exchanger | rack-level retrofit | does not remove local hot spots |
| External laser placement | separates laser heat | distribution loss and redundancy |

### OIF Efficiency Direction
OIF and industry roadmaps target decreasing I/O energy toward single-digit and eventually sub-pJ/bit component/interconnect goals. A blanket “<1 pJ/bit” target must specify whether it applies to an electrical interface segment, optical engine, or complete link; complete pluggable links remain well above that threshold at the 2024 baseline.

### PUE Impact
| Variable | Effect |
|---|---|
| IT optics power | directly increases facility input power |
| Fan/pump power | architecture and temperature dependent |
| PUE | facility energy / IT energy; optics choice changes denominator and cooling load |
| Port utilization | idle power can dominate lightly loaded fabrics |
| Redundancy | spare lasers/modules add embodied and operating overhead |

### Power as a Moat
Benchmark vendors on same-rate/same-reach module watts, host SerDes requirement, case temperature, FEC latency, BER margin, and field failure. Marketing pJ/bit without these controls is not comparable.

### Power Delivery
- Point-of-load regulators reduce distribution loss but add package heat.
- High di/dt SerDes/DSP loads challenge power integrity and jitter.
- CPO package escape competes for electrical, optical, thermal, and mechanical area.
- Shared external lasers require monitored redundant power and safe switching.
- Telemetry should expose voltage, current, temperature, laser bias, and error margin.

## Data Tables (where applicable)
| Field | Value | Source | Date |
|---|---|---|---|
| 800G pluggable baseline | 14-20 W [ESTIMATED] | vendor datasheets | 2023-2024 |
| 1.6T target envelope | 20-30 W [ESTIMATED] | roadmaps | 2024-2025 |
| 800G normalized energy | 17.5-25 pJ/bit | calculation | baseline |
| Main removable LPO block | module DSP | LPO architecture | 2024 |
| Main CPO power mechanism | shorter electrical reach | OIF CPO | 2023 |

## Open Questions / Gaps
- Build a measured SKU-level power database at common conditions.
- Include host SerDes, regulators, laser, and cooling in total link power.
- Test optics compatibility with immersion fluids and liquid-cooled rack layouts.
- Track idle versus loaded power and thermal derating.
- Define OIF roadmap target boundaries precisely.

## References
- OIF CEI and CPO work | https://www.oiforum.com/technical-work/ | 2026-06-09
- OSFP MSA | https://osfpmsa.org/ | 2026-06-09
- QSFP-DD MSA | http://www.qsfp-dd.com/ | 2026-06-09
- ASHRAE Data Centers | https://www.ashrae.org/technical-resources/bookstore/datacom-series | 2026-06-09
- The Green Grid PUE | https://www.thegreengrid.org/ | 2026-06-09
