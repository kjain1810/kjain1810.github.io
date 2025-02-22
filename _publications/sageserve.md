---
title: "Serving Models, Fast and Slow: Optimizing Heterogeneous LLM Inferencing Workloads at Scale"
collection: publications
category: conferences
permalink: /publication/sageserve
excerpt: 'Auto scaling for LLM datacenters'
date: 2025-02-20
venue: 'Under Review'
# slidesurl: 'http://academicpages.github.io/files/slides1.pdf'
paperurl: 'https://arxiv.org/abs/2502.14617'
citation: 'Shashwat Jaiswal*, Kunal Jain*, Yogesh Simmhan, Anjaly Parayil, Ankur Mallick, Rujia Wang, Renee St Amant, et al. ‘Serving Models, Fast and Slow:Optimizing Heterogeneous LLM Inferencing Workloads at Scale’. arXiv [Cs.DC], 2025. https://doi.org/10.48550/ARXIV.2502.14617.
'
---

Large Language Model (LLM) inference workloads handled by global cloud providers can include both latency-sensitive and insensitive tasks, creating a diverse range of Service Level Agreement (SLA) requirements. Managing these mixed workloads is challenging due to the complexity of the inference stack, which includes multiple LLMs, hardware configurations, and geographic distributions. Current optimization strategies often silo these tasks to ensure that SLAs are met for latency-sensitive tasks, but this leads to significant under-utilization of expensive GPU resources despite the availability of spot and on-demand Virtual Machine (VM) provisioning. We propose SAGESERVE, a comprehensive LLM serving framework that employs adaptive control knobs at varying time scales, ensuring SLA compliance while maximizing the utilization of valuable GPU resources. Short-term optimizations include efficient request routing to data center regions, while long-term strategies involve scaling GPU VMs out/in and redeploying models to existing VMs to align with traffic patterns. These strategies are formulated as an optimization problem for resource allocation and solved using Integer Linear Programming (ILP). We perform empirical and simulation studies based on production workload traces with over 8M requests using four open-source models deployed across three regions. SAGESERVE achieves up to 25% savings in GPU-hours while maintaining tail latency and satisfying all SLOs, and it reduces the scaling overhead compared to baselines by up to 80%, confirming the effectiveness of our proposal. In terms of dollar cost, this can save cloud providers up to $2M over the course of a month.
