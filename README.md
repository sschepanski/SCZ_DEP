# High Resolution Joint Symbolic Dynamics in Depression and Schizophrenia
## Overview

This repository contains the reproducible analysis workflow for the project titled “High Resolution Joint Symbolic Dynamics Reveal Altered Cardiorespiratory Network Pathways and Autonomic Dysregulation in Schizophrenia and Depression”.
The project investigates autonomic regulation and cardiorespiratory network dynamics in patients with depression and schizophrenia using high resolution joint symbolic dynamics (HRJSD), heart rate variability measures, respiratory parameters, and directional coupling metrics.
The study includes two separate clinical cohorts. The depression cohort consists of healthy controls, unmedicated patients with depression, and patients treated with antidepressant medication. The schizophrenia cohort consists of a separate healthy control group and patients with schizophrenia.
This repository serves as the main reproducible analysis environment for the project.
It contains the code used to clean and harmonize the study data, derive autonomic and symbolic dynamics variables, perform statistical analyses, and generate manuscript ready tables and figures.

## Purpose of This Repository

The purpose of this repository is to provide a transparent and reproducible record of:
- cleaning and harmonizing raw clinical and physiological datasets
- deriving HRV, respiration, and symbolic dynamics variables
- generating depression and schizophrenia comparison groups
- performing nonparametric group comparisons across physiological measures
- conducting correlation analyses between symbolic dynamics parameters and classical autonomic markers
- applying multiple testing correction procedures
- generating manuscript ready tables, supplementary material, and figures

This repository therefore provides the full reproducible workflow underlying the planned manuscript analyses.

## Project Context (Short Summary)

The main goal of the project is to investigate whether patients with depression and schizophrenia show altered autonomic regulation and cardiorespiratory coupling compared with healthy controls.

The depression cohort includes:
- KON1 = healthy controls
- DEP = unmedicated depression
- DEP1 = SSRI treated depression
- DEP2 = SNRI treated depression

The schizophrenia cohort includes:
- KON2 = healthy controls
- SCZ = schizophrenia

The project focuses on physiological variables including:
- heart rate variability indices such as sdNN, RMSSD, and pvRSA
- respiratory measures such as breathing frequency and inspiration to expiration ratio
- symbolic dynamics parameters such as D_12n_tau0, NF, and symbolic entropy
- directional coupling measures including Area_BBI->RESP and Area_RESP->BBI

The planned analyses include:
- group comparisons between healthy controls and psychiatric groups
- comparisons between unmedicated and medicated depression groups
- evaluation of potential SSRI and SNRI effects on autonomic regulation
- comparison of schizophrenia related versus depression related alterations
- correlation analyses between symbolic dynamics measures and classical autonomic markers

The project aims to identify whether altered cardiorespiratory coupling patterns are shared across psychiatric disorders or are disorder specific.

## Repository Structure

- **`data/`**: cleaned and intermediate datasets used for the analyses
- **`scr/`**: scripts for data cleaning, variable derivation, statistical analyses, and figure generation
- **`tables/`**: exported descriptive tables, group comparison results, and supplementary outputs
- **`graphs`**: exported figures for the manuscript and supplementary material

## Statistical Approach

The main group comparisons are performed using nonparametric two tailed Mann Whitney U tests because several physiological and symbolic dynamics parameters show non normal distributions and unequal variances across groups.
Spearman rank correlations are used to assess associations between symbolic dynamics measures and classical autonomic markers.
Given the large number of pairwise comparisons across autonomic and symbolic dynamics variables, p values are adjusted using the Bonferroni Holm procedure.
Results are primarily reported as mean ± SD together with medians and interquartile ranges where appropriate.

## Acknowledgements

This repository represents the main reproducible analysis framework for the project on autonomic dysregulation and altered cardiorespiratory coupling in depression and schizophrenia.
It serves as the central record of how clinical, physiological, and symbolic dynamics variables were processed, analyzed, and visualized for the planned manuscript.

## Getting Started

1. **Clone this repository:**

   ```bash
   git clone https://github.com/sschepanski/SCZ_DEP.git
   ```

2. **Set up your enviornment using the provided requirement file:**
   ```bash
   pyenv local 3.11.3
   python -m venv .venv
   source .venv/bin/activate
   pip install --upgrade pip
   pip install -r requirements.txt
   ```

3. **Run the provided notebooks in the `scr/` directory for data preprocessing, model training, and evaluation.**

## **Contributions**

This project was conducted by Dr. Steven Ngandeu Schepanski.

## **License**

This project is licensed under the MIT License.