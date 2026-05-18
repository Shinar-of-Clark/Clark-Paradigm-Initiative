# Multi-terminal Harmonic Fingerprinting Platform (Clark Paradigm) - Phase 2

> **Project Identity:** Shinar of Clark  
> **Author:** Yi Zeng   
> **Framework:** Causal Auditing and Protection for Offshore Wind Sub-health  
> **📄 Manuscript PDF:** [Read the Full Paper Here](./Causal%20Auditing%20and%20Protection%20Paradigm%20for%20Sub-health%20Offshore%20Wind%20Assets%20based%20on%20Multi-terminal%20Harmonic%20Fingerprinting.pdf)  
> **DOI:** [![DOI](https://img.shields.io/badge/DOI-Pending-blue)](https://doi.org/) *(Update with actual DOI upon publication)*

---

## 📖 Introduction

This repository implements Phase 2 ("Physiology") of the sub-health diagnostic framework for offshore wind assets under the **"Clark Paradigm"**. 

Building upon the "Electromagnetic Ledger" established in Phase 1, this research focuses on capturing **precursor signals** and establishing proactive **protection** mechanisms. By deconstructing the temporal evolution of 1st-20th order harmonic fingerprints across dynamic conditions, this phase achieves a critical transition from pure diagnosis to "predictive protection".

**Core Philosophy:** Precursor Warning = Temporal Evolution of Residuals + Dynamic Time-Lag Analysis ($\Delta T$).

---

## 📁 Repository Structure

To ensure the transparency and reproducibility of our research, the supporting materials for this paper are organized as follows:

- `figures/`: Contains all high-resolution figures, temporal evolution diagrams, and cross-terminal protection architectures presented in the manuscript.
- `data/`: Contains the corresponding datasets (time-series dynamic data) used to generate each figure. Researchers can use this data to independently verify the precursor signal capture algorithms and protection logic.

---

## 🛠️ Technical Architecture

This phase extends the distributed hardware topology with advanced temporal analysis and control engines:

- **Perception Layer (Field Layer):** MCU nodes deployed inside the turbine and at the substation inlet execute high-frequency sampling at **10.24 kHz**, dynamically synchronized with mechanical variables (wind speed, RPM).
- **Audit & Protection Layer:** Edge hosts execute predictive mapping and temporal correlation using **Dynamic Causal Models (DCM)** to track the time-lag ($\Delta T$) of fault contagion across nodes, generating corresponding protective actions.

---

## 🚀 Key Features

- **Precursor Signal Capture:** Captures latent sub-health fingerprints (e.g., microscopic insulation degradation and dielectric drift) before catastrophic failures occur.
- **Dynamic Time-Lag ($\Delta T$) Analysis:** Analyzes the time delay between harmonic frequency shifts across different nodes, utilizing it as a robust precursor indicator of component stress.
- **Mechanical-Electrical Predictive Mapping:** Establishes the causal correlation between wind turbine mechanical dynamics (aerodynamic turbulence, sudden speed shifts) and the resulting electrical harmonic fluctuations.
- **Proactive Protection Shield:** Upgrades the causal auditing engine into a closed-loop protection system. It utilizes the time-lag window to issue dynamic early warnings and preemptively safeguards core power assets.

---

## 📊 Performance

By leveraging dynamic time-lag analysis, the framework successfully identifies precursor signatures of insulation aging and IGBT switching degradation **hours to days** prior to conventional threshold alarms. This significantly extends the critical response and protection window for O&M teams, averting major asset losses.

---

## 📚 Citation

If you utilize the concepts or content of this project in your research, please cite our manuscript:

**APA Format:**
> Zeng, Y. (2026). Causal Auditing and Protection Paradigm for Sub-health Offshore Wind Assets based on Multi-terminal Harmonic Fingerprinting. (In Preparation).

**BibTeX:**
```bibtex
@article{zeng2026clark_protection,
  title={Causal Auditing and Protection Paradigm for Sub-health Offshore Wind Assets based on Multi-terminal Harmonic Fingerprinting},
  author={Yi Zeng},
  year={2026},
  note={In Preparation}
}
```

---

## 🛡️ License

This project is licensed under the [Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/legalcode) License.

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)

**Rights Statement:** You are free to share and adapt this work, provided that you give appropriate credit to the author **Yi Zeng (Project Shinar of Clark)** and indicate if changes were made.
