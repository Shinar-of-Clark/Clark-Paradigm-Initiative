# Spatio-Temporal Fault Contagion Tracking and Predictive Asset Management for Offshore Wind Farms Based on Multi-Terminal Harmonic Fingerprints (Clark Paradigm) - Phase 3

> **Project Identity:** Shinar of Clark  
> **Author:** Yi Zeng   
> **Framework:** Spatio-Temporal Fault Contagion Tracking and Predictive Asset Management  
> **📄 Manuscript PDF:** [Read the Full Paper Here](./Spatio-Temporal%20Fault%20Contagion%20Tracking%20and%20Predictive%20Asset%20Management%20for%20Offshore%20Wind%20Farms%20Based%20on%20Multi-Terminal%20Harmonic%20Fingerprints.pdf)  
> **DOI:** [![DOI](https://img.shields.io/badge/DOI-10.5281%2Fzenodo.20306854-blue)](https://doi.org/10.5281/zenodo.20306854)

---

## 📖 Introduction

This repository implements Phase 3 ("Pathology & Prognosis") of the sub-health diagnostic framework for offshore wind assets under the **"Clark Paradigm"**. 

Building upon the "Electromagnetic Ledger" (Phase 1) and the "Proactive Protection Shield" (Phase 2), this phase focuses on **cross-terminal fault contagion tracking** and **proactive asset management**. By tracking the spatio-temporal propagation of sub-health anomalies across a **"5-Level 7-Node"** distributed topology, this phase achieves a critical transition from localized anomaly detection to network-wide cascading propagation analysis and Remaining Useful Life (RUL) estimation.

**Core Philosophy:** Fault Contagion Tracking = Spatio-Temporal Anomaly Envelopes + Cascade Propagation Time-Delay Prediction ($\Delta t$).

---

## 📁 Repository Structure

To ensure the transparency and reproducibility of our research, the supporting materials for this paper are organized as follows:

- `figures/`: Contains all high-resolution figures, attention heatmaps, and fault contagion mechanism flowcharts presented in the manuscript.
- `scripts/`: Contains Python implementation scripts, including the CNN feature trigger, the Transformer spatio-temporal sequence analyzer, and figure generation routines.
- `data/`: Contains the generated simulation datasets representing multi-terminal harmonic signals under different fault propagation scenarios.

---

## 🛠️ Technical Architecture

This phase implements a hybrid deep learning framework to track how sub-health states propagate across the multi-terminal electrical layout:

- **5-Level 7-Node Spatio-Temporal Topology:** Maps offshore wind assets into WTG (Level A/Node A), Converter (Level B/Node B), Collector Cables (Level C/Nodes C1, C2), Transmission Cables (Level D/Nodes D1, D2), and Point of Common Coupling (Level E/Node E).
- **Two-Stage Collaborative Model:**
  - **Stage 1 (CNN Anomaly Envelope Trigger):** Translates high-dimensional frequency-domain harmonic signals ($X_t \in \mathbf{R}^{7 \times 50}$) into real-time anomaly probabilities ($p_t$).
  - **Stage 2 (Transformer Spatio-Temporal Analyzer):** Uses multi-head self-attention with spatio-temporal positional encoding to track the propagation path and estimate the contagion time-delay ($\Delta t$).

---

## 🚀 Key Features

- **Spatio-Temporal Contagion Tracking:** Traces how transient anomalies and sub-health degradation propagate downstream (from turbine to grid) or upstream (from grid disturbances back to the turbine).
- **CNN Anomaly Trigger:** Captures early fault envelopes with high robustness against measurement noise and fluctuating environmental conditions.
- **Transformer-based Delay Estimation ($\Delta t$):** Quantifies the contagion propagation delays, allowing O&M systems to identify the root cause and forecast warning lead times.
- **Multi-Terminal Harmonic Fingerprinting:** Relies on low- and mid-frequency harmonic envelopes (up to the 50th order) to identify mechanical and electrical issues (e.g., blade icing, cable degradation) without expensive high-frequency sensors.

---

## 📊 Performance

By utilizing the collaborative CNN-Transformer model, the platform achieves high accuracy in predicting cross-terminal fault contagion delays:
- **Cascade Tracking:** Successfully forecasts downstream propagation paths and provides early warning windows of **10 to 30 seconds** prior to catastrophic grid shock or terminal failures.
- **Interpretability:** The self-attention weight heatmaps clearly highlight the causal dependencies and bottleneck nodes in the 5-Level 7-Node architecture.

---

## 📚 Citation

If you utilize the concepts or content of this project in your research, please cite our manuscript:

**APA Format:**
> Zeng, Y. (2026). Spatio-Temporal Fault Contagion Tracking and Predictive Asset Management for Offshore Wind Farms Based on Multi-Terminal Harmonic Fingerprints (v1.0.0). Zenodo. https://doi.org/10.5281/zenodo.20306854

**BibTeX:**
```bibtex
@misc{zeng2026clark_contagion,
  title={Spatio-Temporal Fault Contagion Tracking and Predictive Asset Management for Offshore Wind Farms Based on Multi-Terminal Harmonic Fingerprints},
  author={Yi Zeng},
  year={2026},
  publisher={Zenodo},
  version={v1.0.0},
  doi={10.5281/zenodo.20306854},
  url={https://doi.org/10.5281/zenodo.20306854}
}
```

---

## 🛡️ License

This project is licensed under the [Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/legalcode) License.

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)

**Rights Statement:** You are free to share and adapt this work, provided that you give appropriate credit to the author **Yi Zeng (Project Shinar of Clark)** and indicate if changes were made.
