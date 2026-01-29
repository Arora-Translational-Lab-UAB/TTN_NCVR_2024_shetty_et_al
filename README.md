# TTNtv, Cardiovascular Risk Factors, and Risk of AF and HF

This repository contains the analysis code and statistical pipelines for the study: **"Titin truncating variants, cardiovascular risk factors and the risk of atrial fibrillation and heart failure"** (Published in *Nature Cardiovascular Research*, 2024).

## 📌 Project Overview
Truncating variants in the *Titin* gene (**TTNtv**) are the most common genetic cause of dilated cardiomyopathy (DCM) and are prevalent in patients with atrial fibrillation (AF). This study investigates whether the clinical expression of these variants is modified by traditional cardiovascular risk factors (CVRFs) using a large-scale "genomics-first" approach in the **UK Biobank**.

### Key Research Questions:
1. Does the presence of high percent spliced-in (hiPSI) TTNtvs increase the risk of incident AF and HF in the general population?
2. Can a favorable cardiovascular risk profile (Ideal CV Health) mitigate the genetic predisposition conferred by TTNtv?
3. How do these associations differ across diverse ancestral backgrounds, specifically in Black/African-American individuals?

---

## 📊 Key Findings

| Metric | Result Summary |
| :--- | :--- |
| **Primary Risk** | **TTNtv carriers** have a significantly higher risk of incident heart failure (HF) and atrial fibrillation (AF) compared to non-carriers. |
| **Risk Modification** | A **favorable CVRF profile** (low SBP, non-smoking, healthy BMI) partially offsets the high genetic risk of TTNtv. |
| **Ancestry** | The study highlights that Black individuals with TTNtv are at a particularly high risk for these outcomes, emphasizing the need for equitable genomic screening. |
| **Clinical Utility** | Genetic risk is not destiny; aggressive management of modifiable risk factors is critical for TTNtv carriers to prevent clinical disease. |

---

## 🛠 Analysis Pipeline
The repository is structured to reflect the UK Biobank analysis workflow:

1.  **Exome Processing:** Identifying hiPSI TTNtv carriers from UK Biobank whole-exome sequencing (WES) data.
2.  **CVRF Scoring:** Categorizing participants by "Ideal," "Intermediate," or "Poor" cardiovascular health based on blood pressure, BMI, and smoking status.
3.  **Association Testing:** * Logistic regression for cross-sectional associations.
    * Cox Proportional Hazards models for incident AF and HF outcomes.
4.  **Interaction Analysis:** Statistical testing for additive or multiplicative interactions between genetic variants and lifestyle factors.

---

## 🚀 Getting Started

### Prerequisites
* **Language:** R (Version 4.x)
* **Key Packages:** `survival`, `tidyverse`, `rms`, `data.table`, `ggplot2`

### Data Access
This code is designed for use with **UK Biobank** data. Users must have an approved Application ID to access the underlying phenotype and exome files.

---

## 📖 Citation
If you utilize this code or the study findings, please cite:
> *Arora, P., et al. (2024). Titin truncating variants, cardiovascular risk factors and the risk of atrial fibrillation and heart failure. Nature Cardiovascular Research.*

**Lab:** Arora Translational Lab, University of Alabama at Birmingham (UAB)
