# Greenspace Interventions and Mental Disorders - Risk of Bias Figure (Supporting Material)

## Overview

This repository contains a supporting risk of bias analysis created as part of the WHO-funded systematic review and meta-analysis titled “Effects of greenspace interventions on mental disorders” (PROSPERO CRD42023452769). The review summarizes evidence from randomized controlled trials evaluating whether nature-based or greenspace interventions improve clinical outcomes in individuals with mental disorders.

The systematic review was conducted by the original research team listed in the manuscript. This repository is not the primary project repository.

It contains only the code and figure related to the risk of bias assessment that contributed to the full analysis.

## Purpose of This Repository

My contribution to the project was limited to:
- performing part of the Cochrane Risk of Bias Tool (RoB-1) assessment
- generating a risk of bias visualization for the included randomized controlled trials
- providing supporting code and exportable graphics used in the manuscript supplements

This repository therefore provides a clean and reproducible record of how the risk of bias figure was generated, independent of the main analysis workflow.

## Project Context (Short Summary)

The full WHO-commissioned systematic review investigated whether greenspace interventions such as horticultural therapy, forest therapy, and nature-based activities improve mental health outcomes across diagnoses including:
- depression
- schizophrenia
- dementia
- ADHD
- adjustment disorder
- PTSD
- substance use disorders

Seventeen randomized controlled trials (948 participants) were eligible. Eight studies contributed data to the quantitative meta-analyses.

The review reported:
- beneficial effects of greenspace interventions on depressive symptoms and positive affect
- significant improvements in positive affect, negative affect, and general psychopathology among individuals with schizophrenia
- heterogeneity and substantial variation in intervention types, settings, and reporting quality
- frequent unclear or high risk of bias, motivating the need for a clear RoB-1 figure

## Repository Structure

- **`data/`**: minimal data files needed to create the risk of bias plots
- **`scr/`**: scripts for preparing RoB-1 assessments and generating the graphics
- **`graphs`**: exported risk of bias plots used for manuscript supplements

## Acknowledgements

This risk of bias figure forms one small component of the broader WHO-funded project carried out by the primary research team. Full methodological details, statistical analyses, and interpretation of findings are documented in the main manuscript.

## Getting Started

1. **Clone this repository:**

   ```bash
   git clone https://github.com/sschepanski/GreenSpacesMetaAnalysis.git
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