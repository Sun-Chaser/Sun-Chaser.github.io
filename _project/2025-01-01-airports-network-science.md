---
title: "Size Prediction & Role Analysis of U.S. Airports"
collection: project
permalink: /projects/2025-01-01-airports-network-science
excerpt: "Network science project analyzing U.S. aviation connectivity, roles, and resilience using community detection and role mining. <br/><img src='/images/experience/us_airport_network.png' alt=\"US network overview\" style=\"max-width: 100%; height: auto; width: 480px;\" >"
date: 2025 December
created_on: "Fall 2025 CSE 4106 Final Project"
venue: "Washington University in St. Louis"
source_code: "https://github.com/cse4106-fl25/finalproject-honghao_shiyuan-z_pxinyu"
---

Highlights:

- Built a weighted U.S. aviation network from OpenFlights + OurAirports to study connectivity and resilience.
- Computed centrality metrics and compared STL vs ORD at national and community levels.
- Ran community detection (Girvan–Newman, spectral clustering, Louvain) and selected Louvain for highest modularity.
- Applied RolX role detection and designed an adaptive z-score naming scheme for stable role labels.
- Trained a Random Forest airport-size classifier with RolX features, reaching ~90.3% ± 3.1% CV accuracy.
- Ran robustness simulations showing targeted hub removals drastically fragment the network (components 2→78).

Tech Stack:
- Gragh Role Analysis
- Community Detection
- Random Forest Classifier
- Quantitative and Qualitative Analysis

Team Member:
- **Jack Yang**, Xinyu Pan, Shiyuan Zhang

Links:
- Source code: https://github.com/cse4106-fl25/finalproject-honghao_shiyuan-z_pxinyu
