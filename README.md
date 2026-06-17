# 🌌 Analysis of high-redshift galaxies with NIRSpec

## 📌 Overview

This project focuses on the analysis of astronomical spectroscopy data obtained from the **James Webb Space Telescope (JWST)**, specifically using **NIRSpec** observations from the ** Data Archive of the Cosmic Dawn Center**.

The work involves building Python-based pipelines for:

* Data preprocessing
* Emission-line fitting using single Gaussian profiles
* Lyman-α fitting and neutral hydrogen estimation
* Galaxy classification using diagnostic diagrams

These tools enable the extraction of **physical parameters** and the interpretation of **high-redshift sources**, contributing to the study of galaxy formation and evolution in the early universe.

---

## 📂 Data Source

The spectral data used in this project is publicly available through the DJA archive:

🔗 https://s3.amazonaws.com/msaexp-nirspec/extractions/nirspec_graded.html?&sn50_min=3

---

## ⚙️ Features

* 🔧 Preprocessing of JWST/NIRSpec spectra with focus on high-redshift 5<z<7 (early universe) sources
* 📊 Spectral line identification and fitting
* 📈 Model fitting and estimation of neutral hydrogen
* 🌠 Correlation between parameters 
* 🧪 BPT classification diagram (3 sigma upper limits)

---

## 🧠 Methodology

The analysis combines observational data with theoretical modeling. In particular:

* Spectral analysis tool for infared spectra
* Special attention is given to **Lyman-α line modeling** to obtain neutral hydrogen, critical for high-redshift studies

---

## 📚 Reference

For the analytic approximation of the Voigt-Hjerting function used in Lyman-α modeling, this project follows:

> Tepper García, T. (2006). *Voigt profile fitting to quasar absorption lines: an analytic approximation to the Voigt-Hjerting function: A new method to compute Voigt profiles.*
> Monthly Notices of the Royal Astronomical Society, 369(4), 2025–2035.
> doi: 10.1111/j.1365-2966.2006.10450.x
> http://dx.doi.org/10.1111/j.1365-2966.2006.10450.x

---

## 🚀 Technologies

* Python
* NumPy / SciPy
* Astropy
* Matplotlib
* Custom spectral analysis tools

---

## 🎯 Goals

* Extract reliable physical parameters from JWST spectra
* Improve efficiency of spectral modeling pipelines
* Contribute to the understanding of early galaxy formation

---
## 📓 Notebooks
Note: The workflow was not fully automated, as visual inspection was required due to the high variability and complexity of the objects in the dataset.

### Scientific Analysis

This notebook combines emission-line analysis and Ly$\alpha$ absorption modeling to derive the physical properties of high-redshift galaxies.

* Gaussian fitting of prominent emission lines (e.g., H$\alpha$, H$\beta$, [OIII])
* Flux extraction and calibration
* Estimation of the **Star Formation Rate (SFR)** from H$\alpha$ luminosity using standard calibrations
* Voigt profile fitting of the Ly$\alpha$ region using the Tepper-García approximation
* Estimation of the neutral hydrogen (HI) column density and related physical parameters

```bash
highzgalaxy_P1.py
```

---

### Galaxy Classification and Data Visualization

This notebook focuses on the classification and visualization of galaxy properties derived from spectroscopic measurements.

* Calculation of diagnostic emission-line ratios (e.g., [OIII]/H$\beta$, [NII]/H$\alpha$)
* Construction of BPT diagnostic diagrams
* Classification of galaxies as star-forming, composite, LINER, or AGN
* Spectral visualization with Matplotlib, including line identification and annotations
* Generation of publication-quality multi-panel figures
* Exploration of correlations between physical parameters (e.g., SFR and redshift)

```bash
highzgalaxy_P2.py
```

## ⚠️ Note

These notebooks are provided solely to showcase the analysis tools and methodology developed in this project.

