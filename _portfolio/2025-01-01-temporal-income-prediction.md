---
title: "Temporal Income Prediction with Incomplete Observations"
collection: portfolio
permalink: /portfolio/2025-01-01-temporal-income-prediction
excerpt: "Forecasted firm profitability from SEC filings using Kalman-EM imputation and Bayesian ARMA modeling. <br/><img src='/images/project_4210.png' alt=\"Temporal Analysis\" style=\"max-width: 100%; height: auto; width: 480px;\" >"
date: "2025 December"
created_on: "Fall 2025 SDS 4210 Final Project"
venue: "Washington University in St. Louis"
source_code: "https://github.com/Sun-Chaser/SDS4210FinalProject"
---

Highlights:

- Built a 2008–2024 quarterly panel from SEC APIs and merged firm metadata with location + SIC.
- Imputed missing income using EM, choosing Kalman-EM over GMM based on lower relative error.
- Embedded SIC descriptions via sentence-transformer and clustered firms into industry groups.
- Modeled income dynamics with Bayesian ARMA (Student-t), achieving ~3.1B holdout MAE in 2024.

Tech Stack:
- Data Aggregatin and Clean
- Data Imputation
- Kalman Filter / Finite Gaussian Mixture
- EM Algorithm

Links:
- Source code: https://github.com/Sun-Chaser/SDS4210FinalProject