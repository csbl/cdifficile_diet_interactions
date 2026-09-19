# Clostridioides difficile-commensal interactions are impacted by diet more than differences between strains

This repository contains the computational pipeline, genome-scale metabolic models (GEMs), and analysis scripts for evaluating how dietary conditions and strain diversity impact *Clostridioides difficile* metabolism and its interactions with gut commensals.

## Overview

The primary risk factor for *Clostridioides difficile* infection (CDI) is broad-spectrum antibiotic usage, which disrupts the intestinal microbiome. While *C. difficile* is genetically and metabolically diverse, its growth and pathogenesis are strongly modulated by host diet. 

In this study, we built genome-scale metabolic reconstructions of **105 *C. difficile* strains** alongside key gut commensals. By simulating metabolic flux distributions and microbial cross-feeding dynamics under varying nutritional regimes, we show that:
- **Diet shifts *C. difficile* metabolism more strongly than strain differences.**
- **Metabolic cross-feeding interactions** between *C. difficile* and intestinal commensals increase under restrictive nutritional environments.
- Key nutrients driving these beneficial interactions center on **Stickland fermentation pathways** (e.g., aspartate and glutamate exchange).

---

## Repository Structure

```text
cdifficile_diet_interactions/
├── models/                     # Metabolic models (GEMs) for C. difficile strains and commensals
├── scripts/                    # Computational pipeline and analysis scripts
│   ├── reconstruction/         # Gap-filling and model building via Reconstructor
│   ├── flux_sampling/          # Media constraint setting and flux sampling (Gapsplit)
│   ├── MetCT_simulations/      # Metabolic CrossTalk (MetCT) mutualism/competition simulations
│   └── statistics_figures/     # Scripts for PCA, clustering, and plot generation
├── data/                       # In silico media definitions (BHI, HiPLoC, LoPHiC) and processed metadata
└── README.md
