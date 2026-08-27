# Nusantara-Ligand-DB: Comprehensive 3D Database of Indonesian Natural Products 🇮🇩

![Open Access](https://img.shields.io/badge/Open%20Access-Yes-brightgreen) ![Format](https://img.shields.io/badge/Format-SDF%20%7C%20XLSX-blue) ![License](https://img.shields.io/badge/License-CC%20BY--NC%204.0-orange) ![HAKI](https://img.shields.io/badge/HAKI-EC002026156809-purple) ![DOI](https://img.shields.io/badge/DOI-10.5281%2Fzenodo.22127902-blue)

A 3D-optimized, open-access chemoinformatics database mapping the secondary metabolites of plant species indigenous to Indonesia, curated for High-Throughput Virtual Screening (HTVS) and Computer-Aided Drug Discovery (CADD).

---

## ⚖️ License & Terms of Use
This database is strictly licensed under the **Creative Commons Attribution-NonCommercial 4.0 International (CC BY-NC 4.0)**.
* **Academic/Research Use:** Free to download, share, and adapt for non-commercial scientific research, provided appropriate credit is given.
* **Commercial Use:** STRICTLY PROHIBITED without explicit prior permission and licensing agreements. Pharmaceutical companies or commercial entities wishing to utilize this database must contact the authors.

---

## Overview

This repository contains a comprehensive, curated, 3D-optimized molecular database cataloging the secondary metabolites of 25,634 plant species indigenous to Indonesia (featuring 34,105 unique natural compounds). It is explicitly designed to accelerate computer-aided drug discovery by providing ready-to-use, biologically relevant ligand conformations optimized for Structure-Based Virtual Screening (SBVS) and Molecular Docking campaigns against various biological targets.

---

## Dataset Curation Pipeline

The library was generated and processed through a rigorous, multi-layered chemoinformatic and computational pipeline:
1. **Structural Deduplication & Standardization:** Removal of duplicate entries and salt/solvent separation.
2. **Physicochemical Filtering:** Molecular weight and property filtering to ensure drug-likeness.
3. **Reactive Scaffold Elimination:** Pan Assay Interference Compounds (PAINS) and frequent hitter filters.
4. **ADMET Profiling:** In-depth pharmacokinetic and toxicity predictions (including hERG, DILI, Ames, and CYP450 inhibition probabilities).
5. **3D Conformational Optimization:** Energy minimization and 3D coordinate generation using robust force fields in YASARA-Structure at physiological pH 7.4.

---

## Repository Structure & Tiered Output

The dataset is stratified into specific archives based on probability thresholds for pharmacokinetics and toxicity, allowing researchers to choose the optimal chemical space for their downstream screening applications.

Each release package contains:
* **`3D Database of Secondary Metabolites of Indonesian Biodiversity.xlsx`**: Comprehensive metadata containing Canonical SMILES, botanical taxonomy mapping, and physicochemical properties.
* **`admet_0.7.rar`**: Contains 14,115 "Safe" optimized 3D structures (threshold < 0.7) ready for broad virtual screening campaigns.
* **`admet_0.5.rar`**: Contains 7,785 "Ultra-safe" optimized 3D structures (threshold < 0.5) representing candidates with maximal predictive safety profiles.

---

## How to Use

1. Download the preferred `.rar` archive (`admet_0.5.rar` or `admet_0.7.rar`) based on your screening stringency requirements.
2. Extract the archive to your local working directory.
3. The structural files are universally compatible with major molecular modeling and docking software (e.g., AutoDock Vina, YASARA, Schrödinger, Discovery Studio).
4. Cross-reference the 3D structures with the provided Excel (`.xlsx`) metadata file to track the botanical species, taxonomy, and SMILES strings of origin.

---

## Citation

If you utilize this database in your academic research, please cite our official dataset repository:

> Nugraha, G. (2026). Nusantara-Ligand-DB: Comprehensive 3D Database of Indonesian Natural Products (v1.0.0) [Data set]. Zenodo. https://doi.org/10.5281/zenodo.22127902

*(Note: Intellectual Property Rights / HAKI officially registered under Kemenkumham with Registration No. EC002026156809).*
