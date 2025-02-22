---
title: "Seer: A Framework for Optimizing Traffic Camera Placement and Deep Learning Inference at the Edge for Vehicle Path Reconstruction"
collection: publications
category: conferences
permalink: /publication/seer
excerpt: 'Placement and deployment of edge cameras in cities.'
date: 2024-12-04
venue: '2024 IEEE/ACM Symposium on Edge Computing (SEC)'
paperurl: 'https://ieeexplore.ieee.org/abstract/document/10818104/'
citation: 'S. Jain, K. Jain, A. Ravindran and S. Purini, "Seer: A Framework for Optimizing Traffic Camera Placement and Deep Learning Inference at the Edge for Vehicle Path Reconstruction," 2024 IEEE/ACM Symposium on Edge Computing (SEC), Rome, Italy, 2024, pp. 333-345, doi: 10.1109/SEC62691.2024.00033.'
---

Integrating traffic cameras with deep learning facilitates real-time multi-camera vehicle path reconstruction, benefiting smart city initiatives such as traffic management and public safety. The high demands on latency, bandwidth, and privacy underscore the necessity of edge computing platforms. However, the continuous operation of compute-intensive deep learning algorithms on round-the-clock camera streams can exceed the compute and power capacities of edge data centers. Therefore, it is critical to strategically deploy and activate camera streams to balance compute demands with performance requirements. Currently, there is a lack of tools to support this planning process. This paper presents Seer, a comprehensive suite of tools and algorithms that aids traffic planners in optimizing traffic camera placement and deep learning model deployment, considering compute and budgetary constraints. Seer encompasses (1) a graph-based algorithm for efficient camera placement incorporating road network topology, (2) a collaborative algorithm for vehicle path reconstruction that enables the use of less accurate but resource-efficient deep learning models, and (3) a scalable traffic simulation framework derived from open-source projects that model city road networks. Evaluations of Seer on two real-world road networks, each with thousands of intersections and simulated vehicle paths, show a 6.3x reduction in compute requirements. This is achieved through a combination of sparse camera deployment and the use of lightweight models, with an average 55% increase in the Hausdorff distance for the path reconstruction algorithm, translating to an absolute increase of 135 to 195 meters.
