---
title: "ModelFlow — Cloud-Native ML Training Platform"
collection: project
permalink: /projects/2025-01-01-modelflow-cloud-native-ml-platform
excerpt: "Cloud-native platform for ML training/inference on GKE using Ray + KubeRay with observability and secure access. <br/><img src='/images/experience/ModelFlow.png' alt=\"Model Flow Demo\" style=\"max-width: 100%; height: auto; width: 480px;\" >"
date: "2025 December"
created_on: "Fall 2025 CSE 4207 Final Project"
venue: "Washington University in St. Louis"
source_code: "https://github.com/cse4207-fall-2025/finalproject-teammodelflow"
---

Highlights:

- Designed a Next.js + FastAPI workflow for dataset upload, model selection, and job submission.
- Generated RayJob configs dynamically and launched distributed workloads on a KubeRay-managed Ray cluster on GKE.
- Integrated GCS for artifacts (models, metrics, predictions) and added Prometheus + Grafana + Ray Dashboard monitoring.
- Implemented secure cloud access (Kubernetes service accounts/IAM) and load-balanced dashboard access for remote execution.

Tech Stack:
- Kubernetes + Docker
- KubeRay Cluster
- Grafana and Prometheus
- Google Cloud Service

Team Member:
- **Jack Yang**, Bobby Yu, Daniel Yan, Jack Fang, Weizhi Du

Links:
- Source code: https://github.com/cse4207-fall-2025/finalproject-teammodelflow