# Detecting New and Rare Cyber Attacks on NSL-KDD

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/mutwassim/Detecting-New-and-Rare-Cyber-Attacks-on-NSL-KDD/blob/main/NSL_KDD_Notebook1_Baselines.ipynb)

This repository contains research and reproducible benchmarks for detecting new and rare cyber attacks on the NSL-KDD benchmark dataset.

## Research Overview & Experiments

- **Experiment A (Literature Protocol Reproduction):** Reproduces the random stratified 80:20 split of `KDDTrain+` as reported in recent literature (e.g. Antony et al., 2026), demonstrating artificially inflated performance (~99% accuracy).
- **Experiment B (Official Benchmark Protocol):** Evaluates models under honest NSL-KDD conditions (train on `KDDTrain+`, test on official `KDDTest+` and `KDDTest-21`) across multiple random seeds for both binary and 5-class tasks.
- **Novel & Rare Attack Evaluation:** Specifically examines detection recall on the 17 attack types that appear only in the test set (zero-day / unseen attacks), breakdown by attack family (DoS, Probe, R2L, U2R).

## Quick Start

You can run the notebook directly in Google Colab using the badge above, or run locally:

```bash
pip install catboost xgboost lightgbm scikit-learn pandas numpy
```

Open [`NSL_KDD_Notebook1_Baselines.ipynb`](NSL_KDD_Notebook1_Baselines.ipynb) in Jupyter Notebook or VS Code / IDE and run all cells.
