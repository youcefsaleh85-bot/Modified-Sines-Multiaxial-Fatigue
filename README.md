# Modified-Sines-Multiaxial-Fatigue
Mechanics-constrained Modified Sines framework for proportional axial–torsional fatigue-life prediction across metallic materials, including cross-validation, benchmark criteria, and supplementary interpretability analyses.
# 🔩 Modified-Sines-Multiaxial-Fatigue

## 📘 Overview

This repository contains the computational implementation and supporting analysis associated with the study:

**A Mechanics-Constrained Sines-Based Descriptor for Proportional Axial–Torsional Fatigue-Life Prediction Across Metallic Materials**

The project develops and evaluates a mechanics-constrained extension of the Classical Sines equivalent-stress descriptor for proportional axial–torsional fatigue loading. The formulation retains the classical distortional-amplitude and hydrostatic mean-stress contributions while introducing additional terms representing axial–torsional interaction and mean deviatoric shear effects.

---

## ⚙️ Main Features

The repository includes:

- implementation of the Classical and Modified Sines formulations;
- comparison with von Mises, Dang Van, and Fatemi–Socie reference descriptors;
- Basquin-type fatigue-life calibration in `log10(N)` space;
- five-fold regime-stratified cross-validation;
- pooled out-of-fold prediction analysis;
- regime-wise performance evaluation;
- specimen-level model comparison;
- multicollinearity diagnostics;
- supplementary XGBoost–SHAP interpretability analysis;
- export of prediction and performance results.

---

## 🧪 Materials Evaluated

The study considers fatigue datasets for:

- **S355 structural steel**
- **7075-T651 aluminum alloy**
- **18Ni300 maraging steel**
- **CuZn37 brass**

The first three datasets are used as the principal high-cycle-fatigue evaluation sets. CuZn37 is treated as an external low-cycle-fatigue scope-challenge dataset.

---

## 📊 Performance Metrics

Model performance is evaluated using:

- coefficient of determination, `R²`;
- mean absolute error, `MAE`;
- root mean square error, `RMSE`.

All metrics are calculated in `log10(N)` fatigue-life space using pooled out-of-fold predictions.

---

## 📂 Repository Contents

```text
Modified-Sines-Multiaxial-Fatigue/
│
├── Modified_Sines_model.ipynb
├── README.md
├── LICENSE
├── .gitignore
└── additional supporting files
