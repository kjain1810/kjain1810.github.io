---
title: "CloakLM: Obfuscating GPU Memory Layout to Mitigate Model Ex-filtration for Serving"
collection: publications
category: conferences
permalink: /publication/cloaklm
excerpt: 'Secure execution of LLMs on untrusted hardware with physical attack vectors'
date: 2026-06-16
venue: 'Preprint'
# slidesurl: 'http://academicpages.github.io/files/slides1.pdf'
paperurl: 'https://arxiv.org/abs/2606.18400'
citation: 'Kunal Jain, Seokjin Go, Divya Mahajan. `CloakLM: Obfuscating GPU Memory Layout to Mitigate Model Ex-filtration for Serving` arXiv [Cs.OS], 2026. https://doi.org/10.48550/arXiv.2606.18400'
---

Large foundation models deployed on third-party and shared accelerator infrastructure face a practical risk of model exfiltration that existing defenses do not fully address. In common serving deployments, model providers control the VM or bare-metal serving stack but not the surrounding hardware substrate. The host to GPU interconnect, accelerator fabric, and neighboring infrastructure components remain outside the tenant's trust boundary and have been shown to be exploitable. Hermes demonstrates lossless DNN reconstruction from passive PCIe observation, while TunnelS exfiltrates HBM contents at high throughput via driver-level access without disrupting inference. Co-tenant VMs can further access memory-mapped interfaces or misconfigured RDMA regions without physical co-location. These attacks exploit a common property of ML systems: model weights are stored in large, contiguous, and repeatedly accessed memory regions, making intercepted PCIe transfers and HBM dumps rich enough to reveal model structure and parameters.

We present CloakLM, a software-only memory-obfuscation framework that removes this structural regularity without changing the inference stack's logical view of memory. CloakLM combines three mechanisms: PCIe traffic shaping, inter- and intra-layer weight shuffling, and physical HBM page remapping. Authorized execution retains a valid virtual memory layout with negligible overhead, while unauthorized observers see fragmented and semantically incoherent state.

CloakLM integrates with vLLM and PyTorch, requires no hardware changes, and complements confidential computing. Evaluation on distributed inference workloads using LLaMA and Qwen models shows near-native performance while significantly increasing resistance to PCIe snooping and HBM dump attacks, making inference-time model exfiltration substantially less practical. 

