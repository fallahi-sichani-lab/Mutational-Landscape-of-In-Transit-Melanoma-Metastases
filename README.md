# README

## Overview
This repository contains the analysis code and data accompanying the manuscript:  

**“Characterizing the Mutational Landscape of In-Transit Melanoma Metastases”**  

The study characterizes the mutational landscape of in-transit melanoma (ITM) using the MSK-IMPACT sequencing dataset. We integrate **clinical/genomic comparisons, mutual information (MI) analysis, pairwise gene mutation analysis, and principal component analysis (PCA)** to define mutation patterns that distinguish ITM from primary tumors, regional lymph node metastases, and distant metastases.  

All figures in the manuscript can be reproduced directly from the scripts provided. The `Data/` folder includes all input files required to run these analyses.  

---

## Repository Structure

```
Clinical and Genomic Characteristics/
    Clinical_and_Genomic_Characteristics.Rmd   # Figures 2A, 2C, 2D
    Driver_Mutations.Rmd                       # Figure 2B

Data/                                          # Input data for all analyses
    mutation_df_*.rds
    *_pts.csv
    *_mi_results_*.csv
    highlights_*.csv
    dataframe_pca_genes.rds
    MSigDB_Hallmark_2020_table_intransit_vs_other.csv

Mutual Information Analysis (Individual Genes)/
    Mutual_Information_Individual_Genes.Rmd    # Figure 3A

Mutual Information Analysis (Paired Genes)/
    Pairwise_Mutation_Rank.Rmd                 # Figure 4A
    Mutual_Information_vs_Ratio_Plots...Rmd    # Figure 4B
    Mutual_Information_Subtype_Comparison.Rmd  # Figure 4C
    EnrichR.Rmd                                # Figure 4D
    Validation.Rmd                             # Figure 4E
    Parallel_Pairwise_Mutual_Information_Analysis.Rmd  # Data generation (Figure 4)

PCA Analysis/
    PCA_Analysis.Rmd                           # Figures 3B–3F
```

---

## Figure Mapping (Manuscript → Code)

- **Figure 2**
  - 2A, 2C, 2D → `Clinical_and_Genomic_Characteristics.Rmd`
  - 2B → `Driver_Mutations.Rmd`

- **Figure 3**
  - 3A → `Mutual_Information_Individual_Genes.Rmd`
  - 3B–3F → `PCA_Analysis.Rmd`

- **Figure 4**
  - 4A → `Pairwise_Mutation_Rank.Rmd`
  - 4B → `Mutual_Information_vs_Ratio_Plots_Including_WT.nb.Rmd`
  - 4C → `Mutual_Information_Subtype_Comparison.Rmd`
  - 4D → `EnrichR.Rmd`
  - 4E → `Validation.Rmd`
  - Data generation for Figure 4 → `Parallel_Pairwise_Mutual_Information_Analysis.Rmd`

---

## Citation
If you use this code or dataset, please cite the manuscript:  
> [Manuscript Title], [Authors], [Journal/Conference], [Year].
