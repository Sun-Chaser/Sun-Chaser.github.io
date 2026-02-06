---
title: "Size Prediction & Role Analysis of U.S. Airports"
collection: portfolio
permalink: /portfolio/2025-01-01-airports-network-science
excerpt: "Network science project analyzing U.S. aviation connectivity, roles, and resilience using community detection and role mining."
date: 2025-01-01
venue: "Washington University in St. Louis"
---

Highlights:

- Built a weighted U.S. aviation network from OpenFlights + OurAirports to study connectivity and resilience.
- Computed centrality metrics and compared STL vs ORD at national and community levels.
- Ran community detection (Girvan–Newman, spectral clustering, Louvain) and selected Louvain for highest modularity.
- Applied RolX role detection and designed an adaptive z-score naming scheme for stable role labels.
- Trained a Random Forest airport-size classifier with RolX features, reaching ~90.3% ± 3.1% CV accuracy.
- Ran robustness simulations showing targeted hub removals drastically fragment the network (components 2→78).
