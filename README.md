#  An Artificial Intelligence–Driven Multimodal Algorithm Predicts Immunotherapy and Targeted Therapy Outcomes in Clear Cell Renal Cell Carcinoma

##  Introduction

This repository supports our study on predictive modeling in **metastatic clear cell renal cell carcinoma (ccRCC)**. While **tyrosine kinase inhibitors (TKIs)** and **immune checkpoint inhibitors (ICIs)** have transformed treatment, challenges such as toxicity and eventual resistance remain.

![graphical abstract](Figure/GA actual.svg)


##  Summary

- **Cohorts**: Integrated transcriptomic data from **16 independent cohorts** (`n = 4,143` patients)
- **Discovery**: Identified **five harmonized immune tumor microenvironment (HiTME) subtypes**
- **Validation**: Confirmed HiTME classification using **multiplex immunofluorescence (mIF)**
- **Model**: Developed a **machine learning–based predictive framework** combining:
  - Genomic alterations  
  - Transcriptomic features  
  - Tumor microenvironment (TME) patterns  
- **Application**: Predicts response to **ICI** and **TKI** therapies  
- **Clinical relevance**: Enables **retrospective clinical validation** and paves the way for **prospective trials**

---

##  Repository Structure

```text
├── data/                          # Preprocessed expression and annotation data
│   ├── ccrcc_tki_0.1.pickle       # Trained TKI model
│   └── ccrcc_io_0.3.pickle        # Trained IO model
├── IO_model.ipynb                 # Jupyter notebook for IO model analysis and visualization
├── TKI_model.ipynb                # Jupyter notebook for TKI model analysis and visualization
├── portraits/                     # Helper functions and pipelines
├── requirements.txt               # Python package dependencies
├── make_tme_environment.sh        # Shell script for environment setup
└── README.md                      # Project summary and instructions

```

## Setup

```
git clone https://github.com/BostonGene/RCC.AI_TKI_IO.Hsieh.git
cd RCC.AI_TKI_IO.Hsieh
bash make_tme_environment.sh
```

## Citation
For more information visit [BostonGene’s Scientific portal](https://science.bostongene.com/).
