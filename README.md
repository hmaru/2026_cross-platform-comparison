# Supplementary Data: Cross-platform comparison of oral microbiome profiles under a unified reference database

This repository provides the official supplementary data and reproducible analysis scripts for the following publication:

> **Zheng J, Maruyama H, Okinaga T.** Cross-platform comparison of oral microbiome profiles under a unified reference database. *J Osaka Dent Univ* 2026; 60(1): 163-170. [https://doi.org/10.18905/jodu.60.1_163](https://doi.org/10.18905/jodu.60.1_163)

## Project Overview

The objective of this study is to evaluate the taxonomic resolution, diversity metrics, and platform-specific biases of the two major sequencing technologies (Illumina MiSeq vs. Oxford Nanopore Technologies). By employing a harmonized bioinformatics pipeline and standardized taxonomic nomenclature (HOMD/HMT), we provide a robust framework for assessing the cross-platform comparability of microbial community profiles.

## Analysis Workflow

The analysis is structured into five sequential Quarto (`.qmd`) modules:

1.  **[01_data_preprocessing.qmd](HOMD_16.03/01_data_preprocessing.qmd):** Import, cleaning, and taxonomic harmonization of Illumina (QIIME2) and Nanopore (EPI2ME) outputs.
2.  **[02_summary_table.qmd](HOMD_16.03/02_summary_table.qmd):** Summary of sequencing throughput and high-quality read counts per sample.
3.  **[03_alpha_diversity.qmd](HOMD_16.03/03_alpha_diversity.qmd):** Calculation and statistical comparison of Shannon diversity indices between platforms.
4.  **[04_sequencer_comparison.qmd](HOMD_16.03/04_sequencer_comparison.qmd):** Quantitative correlation analysis (Spearman) and identification of platform-specific taxonomic biases (Log2 Fold Change).
5.  **[05_taxonomic_assignment_rate.qmd](HOMD_16.03/05_taxonomic_assignment_rate.qmd):** Evaluation of taxonomic resolution and assignment rates across all hierarchical levels.

## How to View Results

The analysis results, including all figures and tables, are available as interactive HTML documents. You can view the rendered reports directly in your browser:

-   **[01: Data Preprocessing](https://hmaru.github.io/2026_cross-platform-comparison/HOMD_16.03/01_data_preprocessing.html)**
-   **[02: Sequencing Summary](https://hmaru.github.io/2026_cross-platform-comparison/HOMD_16.03/02_summary_table.html)**
-   **[03: Alpha Diversity](https://hmaru.github.io/2026_cross-platform-comparison/HOMD_16.03/03_alpha_diversity.html)**
-   **[04: Platform Comparison & Bias](https://hmaru.github.io/2026_cross-platform-comparison/HOMD_16.03/04_sequencer_comparison.html)**
-   **[05: Taxonomic Assignment Rate](https://hmaru.github.io/2026_cross-platform-comparison/HOMD_16.03/05_taxonomic_assignment_rate.html)**

## Software Requirements

The analysis was performed using **R (v4.x)** and **Quarto**. Key R packages include:
- `tidyverse` (Data manipulation)
- `vegan` (Ecological diversity)
- `gt` (Publication-quality tables)
- `patchwork` & `ggtext` (Advanced visualization)

## Author
**Hugo Maruyama**

## Citation
If you find this analysis or repository useful for your research, please cite our original publication:

**Zheng J, Maruyama H, Okinaga T.** Cross-platform comparison of oral microbiome profiles under a unified reference database. *J Osaka Dent Univ* 2026; 60(1): 163-170. [https://doi.org/10.18905/jodu.60.1_163](https://doi.org/10.18905/jodu.60.1_163)
