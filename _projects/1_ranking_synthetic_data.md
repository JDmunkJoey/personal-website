---
layout: page
title: Ranking Inference under Synthetic Data Augmentation
description: Statistical guarantees for Bradley–Terry–Luce ranking when training data are iteratively augmented with synthetic comparisons.
importance: 1
related_publications: true
---

**Graduate Research Assistant, Department of Statistics & Data Science, WashU** · June 2025 – February 2026<br>
Advisor: Dr. Mengxin (Maxine) Yu

This project studies ranking inference under the Bradley–Terry–Luce (BTL) model when the training data are iteratively augmented with synthetic comparisons.

- Established finite-sample optimal ℓ₂ and ℓ∞ statistical rates, exact top-<em>K</em> recovery, and asymptotic normality of the iterative maximum likelihood estimator over sparse comparison graphs, enabling uncertainty quantification for retrained ranking systems.
- Developed a coupled induction argument with leave-one-out constructions and quadratic proxies that disentangles temporal dependence across retraining iterations, proving that model collapse is avoided whenever the number of iterations grows at most polynomially in the number of items.
- Validated the theory through large-scale simulations and an application to the Arena Human Preference 140k dataset.

This work was presented at JSM 2026 (session: Uncertainty Quantification in Generative AI) and at the WashU Graduate Student Seminar.

{% nocite jin2026ranking %}
