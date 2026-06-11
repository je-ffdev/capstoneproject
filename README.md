# The Geography of Preventable Death in England
### Mortality inequality by deprivation, ethnicity and region

![Python](https://img.shields.io/badge/Python-3.14-blue?style=flat-square) ![Pandas](https://img.shields.io/badge/Pandas-2.x-150458?style=flat-square) ![Data](https://img.shields.io/badge/Data-ONS%20Official%20Statistics-003087?style=flat-square) ![Certificate](https://img.shields.io/badge/Google-Data%20Analytics%20Certificate-4285F4?style=flat-square)

---

## Overview

This project analyses mortality inequality across England using official ONS data covering **30 major physical health conditions** across the post-COVID period (March 2021 – January 2023). It examines how premature death is distributed across three dimensions: **socioeconomic deprivation**, **ethnicity**, and **geography** — and how these factors interact.

The analysis produces four original findings with direct policy relevance, presented through a Python notebook, an interactive HTML dashboard, and a professional executive summary.

---

## Key Findings

**Finding 1 — Deprivation is the strongest driver of premature mortality**
People in the most deprived areas face 86% higher all-cause mortality than the least deprived. COPD shows the steepest gradient at 4.69× — nearly five times the mortality rate of the least deprived decile — driven by smoking, occupational exposure, and housing conditions.

**Finding 2 — Ethnicity creates condition-specific vulnerabilities**
Bangladeshi communities show lower all-cause mortality than White British (0.94×) — consistent with the Healthy Immigrant Effect — yet face dramatically higher mortality from Diabetes (3.74×) and Asthma (3.95×), pointing to targeted biological and structural disadvantage rather than generalised poor health.

**Finding 3 — Deprivation does not explain the South Asian diabetes gap**
Even in the wealthiest deprivation quintile, Bangladeshi diabetes mortality (379.4 per 100,000) is over **5× higher** than White British in the same quintile (75.5). Poverty reduction alone is insufficient — targeted clinical and community interventions are required.

**Finding 4 — The North-South mortality divide is severe and persistent**
The North East records all-cause mortality of 2,041 per 100,000 — nearly double London's 1,058. COPD and Lung Cancer rates in the North East are over 4× higher than in the capital, reflecting the long-term health legacy of deindustrialisation and concentrated deprivation.

---

## Repository Structure

```
capstoneproject/
│
├── nhs_analysis.ipynb                          # Full annotated analysis notebook
├── NHS_Mortality_Inequality_Executive_Summary.docx   # Policy brief
├── dashboard.html                              # Interactive dashboard
└── README.md
```

---

## Data Source

**ONS — Inequalities in mortality involving common physical health conditions, England**
- Period: 21 March 2021 to 31 January 2023
- Geographic coverage: England
- Granularity: Deprivation decile, ethnic group, NHS region
- Metric: Age-standardised mortality rate per 100,000 person-years
- Link: [ons.gov.uk](https://www.ons.gov.uk/peoplepopulationandcommunity/healthandsocialcare/healthinequalities)

Age-standardised rates are used throughout to ensure comparisons reflect genuine health disparities rather than differences in age structure across groups.

---

## Methods

| Step | Tool | Detail |
|---|---|---|
| Data loading | Python / Pandas | Multi-sheet Excel ingestion with dtype handling |
| Cleaning | Pandas | Numeric coercion, suppressed value handling (ONS 'z' codes) |
| Analysis | Pandas | Rate ratio calculation, deprivation × ethnicity cross-tabulation |
| Visualisation | Chart.js / HTML | Interactive dashboard, heatmap, regional comparison |
| Reporting | Word (docx) | Professional executive summary |

---

## How to Run

```bash
# Clone the repository
git clone https://github.com/je-ffdev/capstoneproject.git
cd capstoneproject

# Install dependencies
pip3 install pandas openpyxl jupyter

# Launch the notebook
jupyter notebook nhs_analysis.ipynb
```

Download the ONS dataset and place it in the project root before running. The notebook documents the exact file and sheet names expected.

---

## Skills Demonstrated

- Real-world data cleaning and preparation with Pandas
- Multi-dimensional statistical analysis (deprivation, ethnicity, geography)
- Cross-tabulation and rate ratio methodology
- Interactive data visualisation
- Evidence-based analytical writing at policy brief standard
- End-to-end project delivery from raw data to stakeholder output

---

## Author

**jeff-dev**
[github.com/je-ffdev](https://github.com/je-ffdev)

---

*Data: ONS Crown Copyright. Analysis and interpretations are the author's own.*
