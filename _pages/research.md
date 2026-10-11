---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
---

{% include base_path %}

My research lies at the intersection of **applied probability, mathematical statistics, and data science**, with a primary focus on **Extreme Value Theory (EVT)** and **Complex Random Networks**.

In real-world networks—such as large financial interbank transaction webs, social networks, and biological interaction graphs—connectivity is rarely uniform. Instead, these systems are governed by **heavy-tailed distributions**, where rare, gigantic "hub" nodes exert a disproportionate influence over systemic risk, cascading failures, and information diffusion. My work develops rigorous probabilistic frameworks and statistical inference methodologies to understand, model, and monitor these heavy-tailed network phenomena.

---

## 1. Heavy Tails & Extreme Value Theory in Complex Networks

<p align="center">
  <img src="{{ base_path }}/images/research_extremes_networks.png" alt="Heavy-tailed degree distributions and multivariate extremes in random networks" style="max-width: 100%; border-radius: 6px; box-shadow: 0 2px 8px rgba(0,0,0,0.08);">
  <br>
  <em>Figure 1: (Left) Power-law degree tail distribution in scale-free networks. (Right) Joint in- and out-degree asymptotic dependence revealing systemic hub nodes.</em>
</p>

Classical network models often rely on light-tailed Poisson or Gaussian assumptions, which severely underestimate the likelihood and impact of extreme hub events. Our research investigates how scale-free and heavy-tailed topologies emerge through preferential attachment and inhomogeneous random graphs:

* **Degree Growth & Tail Estimation:** Establishing rigorous continuous-time embedding and point-process representations to characterize degree growth rates for nodes entering at arbitrary times, proving consistency and asymptotic normality for Hill estimators and tail index inference in network data.
* **Multivariate Extremes in Multilayer Systems:** Extending extreme value analysis to multilayer and multiplex networks, characterizing the joint tail behavior of degree sequences across interconnected layers and revealing how shocks in one layer trigger catastrophic cascades across others.
* **Systemic Risk Mitigation:** Harnessing multivariate extremal dependence structures to model contagion in financial systems and identifying optimal network interventions (e.g., via maximum independent sets).

### Representative Papers:
* **T. Wang** and S.I. Resnick. *Degree growth rates and index estimation in a directed preferential attachment model.* **Stochastic Processes and their Applications**, 130(2): 878–906, 2020. [[DOI: 10.1016/j.spa.2019.03.014](https://doi.org/10.1016/j.spa.2019.03.014)]
* D. Cirkovic, **T. Wang** and D.B.H. Cline. *Emergence of multivariate extremes in multilayer inhomogeneous random graphs.* **Stochastic Processes and their Applications**, 190: 104762, 2025. [[DOI: 10.1016/j.spa.2025.104762](https://doi.org/10.1016/j.spa.2025.104762)]
* Q. Hui and **T. Wang**. *Extremal dependence networks for mitigating systemic risk via maximum independent sets.* **Journal of Complex Networks**, 14(4): cnag005, 2026. [[DOI: 10.1093/comnet/cnag005](https://doi.org/10.1093/comnet/cnag005)]

---

## 2. Directed Networks with Realistic Mechanics: Reciprocity & Dynamics

<p align="center">
  <img src="{{ base_path }}/images/research_reciprocity_changepoints.png" alt="Directed preferential attachment with reciprocity and changepoint detection" style="max-width: 100%; border-radius: 6px; box-shadow: 0 2px 8px rgba(0,0,0,0.08);">
  <br>
  <em>Figure 2: (Left) Directed edge growth with reciprocal feedback loops. (Right) Sequential likelihood-ratio monitoring for structural changepoint detection in evolving networks.</em>
</p>

Real directed interaction networks (e.g., communication logs, trade networks, online social interactions) exhibit distinctive features that cannot be captured by standard static models:

* **Heterogeneous Reciprocity:** Real networks demonstrate pronounced reciprocal behaviors (mutual links $u \rightleftarrows v$). We developed directed preferential attachment models that incorporate heterogeneous node-level reciprocity mechanisms, proving how reciprocity fundamentally alters the asymptotic joint distribution of in- and out-degrees.
* **Dynamic Changepoint Detection:** Growing networks undergo structural regime shifts over time due to external shocks or policy changes. We devised likelihood-based inference procedures and sequential monitoring test statistics capable of detecting changepoints in evolving random networks with provable theoretical guarantees.
* **Open-Source Tooling:** Implemented novel network generation and inference algorithms in the R package [`wdnet`](https://cran.r-project.org/web/packages/wdnet/index.html) for weighted directed networks.

### Representative Papers:
* D. Cirkovic and **T. Wang**. *Modeling random networks with heterogeneous reciprocity.* **Journal of Machine Learning Research**, 25(10): 1–40, 2024. [[JMLR Link](https://jmlr.org/papers/v25/22-0941.html)]
* D. Cirkovic, **T. Wang** and X. Zhang. *Likelihood-based inference for random networks with changepoints.* **IEEE Transactions on Network Science and Engineering**, 13: 344–359, 2025. [[DOI: 10.1109/TNSE.2024.3499427](https://doi.org/10.1109/TNSE.2024.3499427)]
* Y. Yuan, **T. Wang**, P. Zhang and J. Yan. *Generating general preferential attachment networks with R package `wdnet`.* **Journal of Data Science**, 21(3): 538–556, 2023.

---

## 3. High-Dimensional Network Inference & Heterogeneous Graphical Models

<p align="center">
  <img src="{{ base_path }}/images/research_graphical_models.png" alt="Heterogeneous graphical models and community detection" style="max-width: 100%; border-radius: 6px; box-shadow: 0 2px 8px rgba(0,0,0,0.08);">
  <br>
  <em>Figure 3: (Left) Block-structured precision matrix showing community clusters. (Right) Inferred heterogeneous graphical model with dense intra-community interactions and sparse inter-community bridges.</em>
</p>

Modern biomedical and socio-economic datasets often consist of high-dimensional observations drawn from heterogeneous populations with latent group structures:

* **Simultaneous Identification of Structure & Communities:** When analyzing graphical models with underlying community heterogeneity, estimating the conditional independence graph and finding community assignments are tightly coupled. We proposed an integrated framework that simultaneously uncovers sparse precision matrices and latent community memberships, establishing asymptotic consistency under high-dimensional scaling.
* **Multilayer Network Regression:** Developed regression models incorporating multilayer network topology, leveraging eigenvector centralities and shared community structures to predict nodal responses while accounting for cross-layer interdependencies.

### Representative Papers:
* D. Shi, **T. Wang**, Z. Ying. *Simultaneous identification of sparse structures and communities in heterogeneous graphical models.* **Journal of Machine Learning Research**, 27(148): 1–63, 2026.
* Z. Han, **T. Wang** and Z. Ying. *Multilayer network regression with eigenvector centrality and community structure.* **Statistica Sinica**, 2025. [[DOI: 10.5705/ss.202025.0101](https://doi.org/10.5705/ss.202025.0101)]

---

<p align="center">
  <a href="{{ base_path }}/publications/" class="btn btn--primary" style="padding: 10px 20px; font-weight: bold; text-decoration: none; border-radius: 4px; background: #2b5c8f; color: white;">Explore Full Publication List &raquo;</a>
</p>
