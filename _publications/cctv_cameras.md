---
title: "A cloud-fog architecture for video analytics on large scale camera networks using semantic scene analysis"
collection: publications
category: conferences
permalink: /publication/cctv_cameras
excerpt: 'Distributed infrastructure for managing large scale camera networks.'
date: 2023-05-01
venue: '2023 IEEE/ACM 23rd International Symposium on Cluster, Cloud and Internet Computing (CCGrid)'
paperurl: 'https://ieeexplore.ieee.org/abstract/document/10171548'
citation: 'K. Jain, K. S. Adapa, K. Grover, R. K. Sarvadevabhatla and S. Purini, "A Cloud-Fog Architecture for Video Analytics on Large Scale Camera Networks Using Semantic Scene Analysis," 2023 IEEE/ACM 23rd International Symposium on Cluster, Cloud and Internet Computing (CCGrid), Bangalore, India, 2023, pp. 513-523, doi: 10.1109/CCGrid57682.2023.00054.'
---

This paper proposes a scalable distributed video analytics framework that can process thousands of video streams from sources such as CCTV cameras using semantic scene analysis. The main idea is to deploy deep learning pipelines on the fog nodes and generate semantic scene description records (SDRs) of video feeds from the associated CCTV cameras. These SDRs are transmitted to the cloud instead of video frames saving on network bandwidth. Using these SDRs stored on the cloud database, we can answer many complex queries and perform rich video analytics, within extremely low latencies. There is no need to scan and process the video streams again on a per query basis. The software architecture on the fog nodes allows for integrating new deep learning pipelines dynamically into the existing system, thereby supporting novel analytics and queries. We demonstrate the effectiveness of the system by proposing a novel distributed algorithm for real-time vehicle pursuit. The proposed algorithm involves asking multiple spatio-temporal queries in an adaptive fashion to reduce the query processing time and is robust to inaccuracies in the deployed deep learning pipelines and camera failures.
