# 16S rRNA Gene Sequencing Platform Comparison: Illumina MiSeq vs. Oxford Nanopore Technologies

This repository contains the full analysis workflow for comparing 16S rRNA gene sequencing data generated from **Illumina MiSeq** (short-read) and **Oxford Nanopore Technologies (ONT)** (long-read) platforms, specifically focusing on the characterization of oral microbiomes.

## Project Overview

The objective of this study is to evaluate the taxonomic resolution, diversity metrics, and platform-specific biases of the two major sequencing technologies. By employing a harmonized bioinformatics pipeline and standardized taxonomic nomenclature (HOMD/HMT), we provide a robust framework for assessing the cross-platform comparability of microbial community profiles.

## Analysis Workflow

The analysis is structured into five sequential Quarto (`.qmd`) modules:

1.  **[01_data_preprocessing.qmd](HOMD_16.03/01_data_preprocessing.qmd):** Import, cleaning, and taxonomic harmonization of Illumina (QIIME2) and Nanopore (EPI2ME) outputs.
2.  **[02_summary_table.qmd](HOMD_16.03/02_summary_table.qmd):** Summary of sequencing throughput and high-quality read counts per sample.
3.  **[03_alpha_diversity.qmd](HOMD_16.03/03_alpha_diversity.qmd):** Calculation and statistical comparison of Shannon diversity indices between platforms.
4.  **[04_sequencer_comparison.qmd](HOMD_16.03/04_sequencer_comparison.qmd):** Quantitative correlation analysis (Spearman) and identification of platform-specific taxonomic biases (Log2 Fold Change).
5.  **[05_taxonomic_assignment_rate.qmd](HOMD_16.03/05_taxonomic_assignment_rate.qmd):** Evaluation of taxonomic resolution and assignment rates across all hierarchical levels.

## How to View Results

The analysis results, including all figures and tables, are available as pre-rendered HTML documents. You can view them directly in your browser:

-   [01: Data Preprocessing](HOMD_16.03/01_data_preprocessing.html)
-   [02: Sequencing Summary](HOMD_16.03/02_summary_table.html)
-   [03: Alpha Diversity](HOMD_16.03/03_alpha_diversity.html)
-   [04: Platform Comparison & Bias](HOMD_16.03/04_sequencer_comparison.html)
-   [05: Taxonomic Assignment Rate](HOMD_16.03/05_taxonomic_assignment_rate.html)

## Software Requirements

The analysis was performed using **R (v4.x)** and **Quarto**. Key R packages include:
- `tidyverse` (Data manipulation)
- `vegan` (Ecological diversity)
- `gt` (Publication-quality tables)
- `patchwork` & `ggtext` (Advanced visualization)

## Author
**Hugo Maruyama**

## Citation
*(Please update this section with the relevant publication details when available)*
