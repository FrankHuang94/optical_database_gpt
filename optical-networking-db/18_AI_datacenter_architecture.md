# AI Datacenter Architecture
> **Last Updated:** 2026-06-09
> **Status:** Draft
> **Tags:** AI, training, inference, Ethernet, InfiniBand, scale-up, scale-out

## Overview
AI clusters create synchronized, bursty, east-west traffic with sensitivity to tail latency and collective-operation completion time. Training often demands lossless or congestion-controlled high-bandwidth fabrics, while inference requirements vary from tightly coupled model parallelism to conventional service networks.

Optical architecture follows three domains: scale-up inside a compute domain, scale-out across racks/pods, and scale-across between datacenters. Electrical links dominate the shortest reaches, but optics moves closer to compute as cluster bandwidth and physical span increase.

> 🔄 Refresh Needed: High Priority — update UALink, Ultra Ethernet, NVLink, Spectrum-X, InfiniBand, and optical scale-up product roadmaps.

## Key Findings / Highlights
- [CONFIRMED] Training collectives can be limited by the slowest flow, making congestion control and fault recovery critical.
- [CONFIRMED] RoCEv2 uses routable Ethernet with RDMA; GPUDirect RDMA reduces CPU involvement in data movement.
- [CONFIRMED] UEC was formed to improve Ethernet for AI/HPC workloads [Source: UEC, 2023].
- [CONFIRMED] UALink targets an open accelerator scale-up interconnect [Source: UALink Consortium, 2024].
- [ESTIMATED] 100K+ accelerator clusters increase the value of OCS and multi-datacenter scale-across, but workload scheduling must accommodate circuit reconfiguration [MED confidence].

## Detailed Content
### Training vs Inference
| Dimension | Training | Inference | Implication for Optics |
|---|---|---|---|
| Bandwidth | very high synchronized collectives | variable; can be high for disaggregated serving | training drives dense scale-out links |
| Latency | collective/tail sensitive | request and token latency sensitive | low-hop, low-loss paths |
| Topology | regular large fabrics | heterogeneous service/storage fabrics | different oversubscription choices |
| Fault tolerance | checkpoint/restart; job-wide impact | replica failover | link reliability and fast recovery |
| Scale | 1K-100K+ accelerators | distributed fleets | optics count grows with tiers/spans |

### Connectivity Domains
| Domain | Technologies | Typical Reach | Optical Role |
|---|---|---|---|
| Scale-up | NVLink/NVSwitch, UALink, CXL | board/rack/domain | emerging optical extension/I/O |
| Scale-out | InfiniBand, Ethernet/RoCE, UEC | rack to campus | 400G/800G/1.6T pluggables/CPO |
| Scale-across | Ethernet + coherent DCI | campus/metro | ZR/ZR+, line systems, OCS |

### Topologies
| Topology | Strength | Weakness | Optical Implication |
|---|---|---|---|
| Fat Tree / Clos | predictable nonblocking design | many switches/links | high module count |
| Dragonfly+ | lower diameter and global links | traffic engineering complexity | longer high-rate links |
| Torus/Mesh | local connectivity and cost | variable hop count | mixed electrical/optical |
| Rail-optimized | aligns NIC rails with collectives | workload/topology coupling | deterministic optical layout |
| Reconfigurable OCS | changes physical connectivity | scheduling/reconfiguration | fewer conversion stages possible |

### Cluster Scaling
| Cluster Size | Likely Network Characteristics | Optical Evolution |
|---:|---|---|
| 1K accelerators | single pod, limited tiers | 400G/800G scale-out |
| 10K | multi-pod Clos/Dragonfly | 800G dense fabrics, DCI-like campus links |
| 100K+ | multiple halls/campuses, fault domains | 1.6T, OCS, coherent scale-across, optical I/O |

### Protocols
| Protocol / Consortium | Domain | Status at Baseline |
|---|---|---|
| RoCEv2 | Ethernet RDMA | deployed |
| GPUDirect RDMA | GPU memory data path | deployed in supported stacks |
| InfiniBand | HPC/AI scale-out | deployed, vertically integrated ecosystem |
| Ultra Ethernet Consortium | AI/HPC Ethernet enhancements | specifications developing [TO VERIFY] |
| UALink | accelerator scale-up | consortium/specification developing [TO VERIFY] |
| CXL | coherent CPU/memory/device interconnect | deployed/emerging; photonic extension research |

### OCS for AI Fabrics
Google’s Jupiter evolution shows production OCS can reconfigure datacenter topology under software control. AI application depends on reconfiguration time, traffic predictability, failure handling, and scheduler integration. Millisecond-class or slower circuits suit stable elephant flows more than packet-by-packet dynamics; faster MEMS, liquid-crystal, silicon-photonic, and other switches trade port count, loss, and cost.

### Scale-Across
| Requirement | Optical Technology |
|---|---|
| 10-80 km campus/metro | coherent ZR or coherent-lite; amplified/direct alternatives |
| high fiber efficiency | DWDM coherent |
| deterministic job placement | topology-aware scheduler |
| failure isolation | redundant routes and fast protection |
| clock/synchronization | precision timing architecture |

### Photonic Extension Proposals
UALink and CXL define logical/electrical ecosystems; optical extension requires retimers/bridges or native optical PHY work, latency and coherency analysis, and interoperability. Treat vendor “optical CXL/UALink” claims as proposals until specifications and products are validated.

## Data Tables (where applicable)
| Field | Value | Source | Date |
|---|---|---|---|
| UEC formation | AI/HPC Ethernet consortium | UEC | 2023 |
| UALink announcement | open accelerator scale-up | consortium | 2024 |
| Main scale-out rates | 400G/800G | vendor deployments | 2024 |
| Next scale-out rate | 1.6T | roadmap | 2025-2027E |
| Production OCS evidence | Google Jupiter evolution | SIGCOMM | 2022 |

## Open Questions / Gaps
- Quantify links and optical endpoints per accelerator by topology.
- Track UEC and UALink ratification and commercial deployment.
- Model job completion sensitivity to OCS reconfiguration and failures.
- Compare Ethernet and InfiniBand optical attach rates.
- Define coherent scale-across economics for multi-site training.

## References
- Ultra Ethernet Consortium | https://ultraethernet.org/ | 2026-06-09
- UALink Consortium | https://ualinkconsortium.org/ | 2026-06-09
- NVIDIA GPUDirect | https://developer.nvidia.com/gpudirect | 2026-06-09
- CXL Consortium | https://www.computeexpresslink.org/ | 2026-06-09
- Google Research Jupiter | https://research.google/pubs/ | 2026-06-09
