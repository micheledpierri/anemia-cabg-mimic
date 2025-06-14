# Anemia & CABG Outcomes – MIMIC-IV Study

[![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

⚠️ This repository contains only code and metadata. Patient-level data from MIMIC-IV are not stored here, in compliance with PhysioNet policies.

##  Project Summary

This project explores the relationship between anemia and postoperative complications in patients undergoing Coronary Artery Bypass Grafting (CABG) using the MIMIC-IV clinical database. Both structured data (labs, demographics, ICD codes) and unstructured data (discharge summaries) are analyzed.

## Repository Structure

```
anemia-cabg-mimic/
├── data/                   # NO DATA: only instructions for retrieval
│   └── README.md
├── scripts/                # Python scripts for extraction and analysis
├── results/                # Tables, plots, exportable results
│   ├── figures/
│   └── tables/
├── references/             # Bibliography (BibTeX format)
├── .gitignore
├── LICENSE
├── README.md
└── requirements.txt
```

## Analysis Pipeline

- Cohort selection (CABG ICD codes)
- Anemia classification (ICD and lab values)
- Lab value extraction (first post-admission labs)
- Postoperative course parsing from discharge notes
- Complication identification (structured + NLP)
- Statistical testing (Mann–Whitney, chi-square, logistic models)

## References

- Johnson AEW et al. (2020). *MIMIC-IV (version 2.0)*. PhysioNet. https://doi.org/10.13026/s6n6-xd98  
- WHO Hemoglobin thresholds (2023).  

## Requirements

To install dependencies:

```bash
pip install -r requirements.txt
```


## Data Access Disclaimer

This project uses data from the [MIMIC-IV](https://physionet.org/content/mimiciv/) database. Access requires credentialing and a Data Use Agreement (DUA) through PhysioNet.  
**No protected health information (PHI)** or raw data are stored in this repository.

## Author & Contact

Michele Danilo Pierri – Cardiac Surgeon & Data Scientist  
This repository reflects personal research views only and is not affiliated with any clinical institution.  
info@micheledanilopierri.com  
[LinkedIn](https://www.linkedin.com/)  
[ORCID](https://orcid.org/)  


## License

Distributed under the [MIT License](LICENSE).
