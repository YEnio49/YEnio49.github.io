---
title: "Multiscale Spatial Inequality in Pollution and Health: A Policy-Sensitive MGWR Model"
excerpt: "Mapping Environmental Health Inequality with Policy-Weighted MGWR <br/><img src='/images/policy_mgwr_map.png'>"
collection: portfolio
---

**A spatial modeling project that uses Multiscale Geographically Weighted Regression (MGWR) to analyze how pollution exposure affects health outcomes across space, modulated by local policy strength.**

This project investigates how pollution-related health risks are distributed unequally across regions and how the strength of local environmental policies modulates this relationship. Using a MGWR framework, we explore whether the same level of pollution leads to different health outcomes depending on where people live—and how well-protected those regions are by policy.

## Project Overview

- **Model**: Multiscale Geographically Weighted Regression (MGWR)  
- **Focus**: Spatial heterogeneity of pollution-health relationships  
- **Policy Component**: Local environmental governance and regulatory strength used as weighting variables  
- **Study Area**: Urban and peri-urban regions in China (data customizable)  

## Key Research Questions

1. Does pollution exposure lead to worse health outcomes in poorly regulated areas?  
2. Can strong environmental policies buffer the negative health impacts of pollution?  
3. Are there identifiable “policy blind spots” where vulnerable populations are exposed to disproportionate environmental harm?  

## Methodology – MGWR with Policy Interaction

We use a multiscale geographically weighted regression (MGWR) model to estimate spatially varying relationships between pollution, policy, and health:

$$
y_i = \beta_0(u_i, v_i) + \beta_1(u_i, v_i) x_{1i} + \beta_2(u_i, v_i) x_{2i} + \beta_3(u_i, v_i) (x_{1i} \times x_{2i}) + \epsilon_i
$$

where:

$$
\begin{aligned}
&y_i &&\text{: Health outcome (respiratory hospitalization rate)} \\
&x_{1i} &&\text{: Pollution exposure ( PM2.5 concentration)} \\
&x_{2i} &&\text{: Policy intensity or enforcement score} \\
&x_{1i} \times x_{2i} &&\text{: Interaction term capturing how policy modulates pollution impact} \\
&\beta_k(u_i, v_i) &&\text{: Spatially varying coefficients at location } (u_i, v_i) \\
&\epsilon_i &&\text{: Error term}
\end{aligned}
$$ 

Each coefficient is estimated locally with variable-specific spatial bandwidths.



## Tools Used

- **Python**: Spatial preprocessing, data integration  
- **R (GWmodel)**: MGWR model estimation  
- **QGIS & Google Earth Engine**: Geospatial data processing and visualization  
