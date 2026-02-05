---
name: Machine Learning–Driven Player Valuation for Football Scouting
tools: [Dashboard, SQL, Gradio, Football, Python]
image : https://i.imgur.com/dOT0Eao.png
description: Machine Learning–Driven Player Valuation for Football Scouting

---

# Research on Applying Machine Learning to Improve Player Valuation For Scouting in a Football Team



{% include elements/figure.html image="https://i.imgur.com/dOT0Eao.png" caption="The Dashboard" %}

This project aim to explore how machine learning can enhance football scouting by improving the way players are valued and shortlisted for recruitment. Traditional scouting relies heavily on intuition and manual analysis, which becomes increasingly challenging as global talent pools and transfer spending continue to grow. My work proposes a data-driven recommendation system that supports scouts with objective, interpretable insights.

The system integrates season-level performance statistics with event-level match data. A Variational Autoencoder with a Gamma mixture prior (VAE-Gamma) is used for representation learning, transforming high-dimensional and sparse player statistics into meaningful latent profiles. These representations enable robust similarity searches, outperforming raw statistical comparisons when benchmarked against FBref similarity rankings.

To go beyond individual performance, the project involves simulation by incorporating the VAEP (Valuing Actions by Estimating Probabilities) framework. Building on VAEP, Joint Offensive Impact (JOI) and Joint Defensive Impact (JDI) metrics are used to model player chemistry and team fit. A two-stage pipeline first identifies similar players, then refines recommendations based on chemistry with an existing squad.

---

## Key Results

* **Improved player similarity discovery**
  Representation learning with **VAE-Gamma** significantly outperformed raw statistical clustering, nearly doubling the Silhouette Score and producing cleaner, more meaningful player groupings.

* **Stronger alignment with real-world scouting decisions**
  Chemistry-based re-ranking using **Joint Offensive Impact (JOI)** consistently matched real transfer outcomes from the 2025 summer window, with average shortlist ranks of **10–12** and a **Hit@10 rate of ~0.45**.

* **Action-level valuation beyond goals and assists**
  The **VAEP framework** successfully quantified the impact of all on-ball actions, capturing defensive and off-ball contributions that traditional metrics overlook.

* **Effective team-fit modeling**
  Player chemistry metrics (JOI/JDI) provided stable estimates of how well a player would integrate into an existing squad, enabling recommendations that went beyond “similar players” to “right players.”

* **Practical scouting interface**
  An interactive dashboard prototype allowed scouts to explore recommendations, compare key metrics, and visualize player behavior through heatmaps and radar charts, demonstrating real-world usability.

---
