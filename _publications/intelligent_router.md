---
title: "Intelligent router for llm workloads: Improving performance through workload-aware scheduling"
collection: publications
category: conferences
permalink: /publication/intelligent_router
excerpt: 'Load balancing amid multiple instances of the same LLM'
date: 2024-08-24
venue: "The 5th Workshop on Machine Learning and Systems (EuroMLSys) co-located with EuroSys'25" 
# slidesurl: 'http://academicpages.github.io/files/slides3.pdf'
paperurl: 'https://arxiv.org/abs/2408.13510'
citation: "Kunal Jain, Anjaly Parayil, Ankur Mallick, Esha Choukse, Xiaoting Qin, Jue Zhang, Íñigo Goiri, Rujia Wang, Chetan Bansal, Victor Rühle, Anoop Kulkarni, Steve Kofsky, Saravan Rajmohan, Microsoft . 2025. Performance Aware LLM Load Balancer for Mixed Workloads. In The 5th Workshop on Machine Learning and Systems (EuroMLSys ’25), March 30-April 3, 2025, Rotterdam, Netherlands. ACM, New York, NY, USA, 12 pages. https://doi. org/10.1145/3721146.3721947"
---

Large Language Model (LLM) workloads have distinct prefill and decode phases with different compute and memory requirements which should ideally be accounted for when scheduling input queries across different LLM instances in a cluster. However existing scheduling algorithms treat LLM workloads as monolithic jobs without considering the distinct characteristics of the two phases in each workload. This leads to sub-optimal scheduling and increased response latency. In this work, we start by characterizing factors affecting the response latency during LLM inference serving. We establish that better load balancing of inference requests across the available LLM instances can improve the end-to-end latency to a larger extent than merely focusing on optimizing the instance-level scheduler. Motivated by our findings, we propose a heuristic-guided reinforcement learning-based intelligent router for data-driven and workload-aware scheduling. Our router schedules queries across LLM instances by leveraging a trainable response-length predictor, and a novel formulation for estimating the impact of mixing different workloads and achieves over 11% lower end-to-end latency than existing approaches on a mix of public datasets and 7.8% lower end-to-end latency on real workload data with diverse input and output trends from Cloud Provider X. Additionally, the proposed framework can also serve as a standard for benchmarking different LLM inference schedulers since it provides the best latency for a given model, hardware, and instance-level scheduler combination.
