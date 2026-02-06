---
title: "Temporal Income Prediction with Incomplete Observations"
collection: portfolio
permalink: /portfolio/2025-01-01-temporal-income-prediction
excerpt: "Forecasted firm profitability from SEC filings using Kalman-EM imputation and Bayesian ARMA modeling."
date: 2025-01-01
venue: "Washington University in St. Louis"
---

Highlights:

- Built a 2008–2024 quarterly panel from SEC APIs and merged firm metadata with location + SIC.
- Imputed missing income using EM, choosing Kalman-EM over GMM based on lower relative error.
- Embedded SIC descriptions via sentence-transformer and clustered firms into industry groups.
- Modeled income dynamics with Bayesian ARMA (Student-t), achieving ~3.1B holdout MAE in 2024.
