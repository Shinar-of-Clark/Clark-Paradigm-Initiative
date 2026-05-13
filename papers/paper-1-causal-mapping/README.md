# Multi-terminal Harmonic Fingerprinting Platform (Clark Paradigm)

> **Project Identity:** Shinar of Clark  
> **Author:** Yi Zeng   
> **Framework:** Causal Auditing for Offshore Wind Sub-health Diagnosis

---

## 📖 Introduction

This repository implements the sub-health diagnostic framework for offshore wind assets under the **"Clark Paradigm"**. 

Unlike traditional black-box prediction models, this project establishes an **"Electromagnetic Ledger"** system. By conducting a real-time audit of the **1st-20th order harmonic fingerprints** across the generator, converter, tower-base switchgear, and remote collector cables, it achieves a paradigm shift from "stochastic state prediction" to "deterministic causal auditing".

**Core Philosophy:** Anomaly = Physical Reality - Causal Expectation ($\Delta = Physical\ Reality - Causal\ Expectation$).

---

## 📁 Repository Structure

To ensure the transparency and reproducibility of our research, the supporting materials for this paper are organized as follows:

- `figures/`: Contains all high-resolution figures, architectural diagrams, and result charts presented in the manuscript.
- `data/`: Contains the corresponding datasets (raw and processed) used to generate each figure. Researchers can use this data to independently verify the causal auditing results.

---

## 🛠️ Technical Architecture

This platform adopts a distributed hardware topology, decoupling the perception layer from the audit layer:

- **Perception Layer (Field Layer):** MCU nodes deployed inside the turbine and at the substation inlet execute high-frequency sampling at **10.24 kHz** and local FFT extraction.
- **Audit Layer:** Edge hosts perform feature decoupling and causal mapping via a **Recursive Least Squares (RLS)** engine and **Multi-Head Attention** mechanisms.

---

## 🚀 Key Features

- **Causal Auditing Engine:** Utilizes the RLS operator to dynamically track the dielectric drift of assets, superseding simple threshold-based alarms.
- **Frequency-Selective Sovereignty:**
    - `5th/7th Harmonics`: Locks onto the health state of core power devices within full-scale converters. Precisely captures switching characteristic degradation induced by IGBT junction temperature elevation, dead-time drift, or gate drive delays, while also serving as an early diagnostic indicator for the capacitance decay of AC/DC-side filtering capacitors.
    - `11th/13th Harmonics`: Probes the impedance evolution trajectory of long-distance subsea collection cables. Deeply analyzes distributed capacitance/inductance drift and high-frequency resonance point shifts triggered by "Water Treeing", microscopic insulation dampness, and physical strain of cables caused by subsea currents.
    - `17th+ Harmonics`: Captures feature shifts induced by transformer winding mechanical loosening or magnetic circuit saturation. Furthermore, prolonged spectral imbalance in this range imposes cumulative dielectric stress, serving as a latent indicator for potential partial discharge (PD) activities (while limited by frequency range to capture transient PD pulses directly, it serves as a lateral reflection of insulation aging trends).
- **Ultra-low Latency:** The single-iteration computation time for the 21-dimensional causal vector is **< 5ms**, fully meeting the real-time requirements of 50Hz power infrastructure.
- **Game Theory Decision Optimization:** Introduces a **Nash Equilibrium model** to balance generation revenue, failure risks, and O&M costs, maximizing residual asset value.

---

## 📊 Performance

Under extreme aerodynamic turbulence (e.g., sudden wind speed shifts), the error of traditional LSTM models may surge to 25%. In contrast, this framework, through rapid self-calibration, strictly restricts the audit residual $\Delta$ to within **5%**.

---

## 📚 Citation

If you utilize the concepts or content of this project in your research, please cite our preprint paper:

```bibtex
@article{zeng2026clark,
  title={A Causal Auditing Paradigm for Sub-health Diagnosis of Offshore Wind Assets via Multi-terminal Harmonic Fingerprinting},
  author={Yi Zeng},
  year={2026},
  journal={Preprint},
  doi={10.5281/ZENODO.20149719}
}
```

---

## 🛡️ License

This project is licensed under the [Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/legalcode) License.

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)

**Rights Statement:** You are free to share and adapt this work, provided that you give appropriate credit to the author **Yi Zeng (Project Shinar of Clark)** and indicate if changes were made.
