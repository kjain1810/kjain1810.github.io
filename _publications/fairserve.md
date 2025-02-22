---
title: "Ensuring Fair LLM Serving Amid Diverse Applications"
collection: publications
category: conferences
permalink: /publication/fairserve
excerpt: 'Fairness in serving multiple users and applications.'
date: 2024-11-24
venue: 'Under Review'
# slidesurl: 'http://academicpages.github.io/files/slides2.pdf'
paperurl: 'https://arxiv.org/abs/2411.15997'
citation: 'Redwan Ibne Seraj Khan*, Kunal Jain*, Haiying Shen, Ankur Mallick, Anjaly Parayil, Anoop Kulkarni, Steve Kofsky, et al. ‘Ensuring Fair LLM Serving amid Diverse Applications’. arXiv [Cs.LG], 2024. https://doi.org/10.48550/ARXIV.2411.15997.'
---

In a multi-tenant large language model (LLM) serving platform hosting diverse applications, some users may submit an excessive number of requests, causing the service to become unavailable to other users and creating unfairness. Existing fairness approaches do not account for variations in token lengths across applications and multiple LLM calls, making them unsuitable for such platforms. To address the fairness challenge, this paper analyzes millions of requests from thousands of users on MS CoPilot, a real-world multi-tenant LLM platform hosted by Microsoft. Our analysis confirms the inadequacy of existing methods and guides the development of FairServe, a system that ensures fair LLM access across diverse applications. FairServe proposes application-characteristic aware request throttling coupled with a weighted service counter based scheduling technique to curb abusive behavior and ensure fairness. Our experimental results on real-world traces demonstrate FairServe's superior performance compared to the state-of-the-art method in ensuring fairness. We are actively working on deploying our system in production, expecting to benefit millions of customers world-wide.
