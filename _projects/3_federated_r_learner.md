---
layout: page
title: Federated R-Learner for Heterogeneous Treatment Effects
description: Fed-R, a privacy-preserving federated R-learner for estimating conditional average treatment effects across heterogeneous sites. ENAR 2026 Distinguished Student Paper Award.
importance: 3
related_publications: true
---

**Graduate Research Assistant, WashU Institute for Informatics, Data Science and Biostatistics** · May 2025 – October 2025
Advisors: Dr. Nan Lin and Dr. Linying Zhang

Estimating conditional average treatment effects (CATE) from multi-site clinical data is hampered by privacy constraints that prevent pooling patient-level records. This project develops **Fed-R**, a federated R-learner that learns across sites without sharing patient-level data.

- Developed Fed-R, a privacy-preserving, communication-efficient federated R-learner combining local cross-fitting with Neyman-orthogonal residualization and FedProx-style proximal aggregation, achieving √*N*-consistency and asymptotic normality without sharing patient-level data.
- Uncovered a performance-reversal phenomenon: federated estimation surpasses centralized pooling once sites violate the overlap assumption, cutting global RMSE by 50–70% and improving local estimation accuracy by 2–4×, with most gains realized within 2–5 communication rounds.
- Benchmarked Fed-R against oracle and centralized R-learners across six synthetic scenarios and the semi-synthetic IHDP benchmark.
- Cleaned and analyzed a multi-site EHR cohort (90K+ patients, 60K+ covariates) comparing two antihypertensive drugs on time-to-event outcomes.

This work received an **ENAR 2026 Distinguished Student Paper Award** and was presented at the ENAR 2026 Spring Meeting in Indianapolis.

{% nocite jin2025fedr xin2026amia xin2026fedr %}
