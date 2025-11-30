# wsss-rs-bibliometric-repro# WSSS-RS Bibliometric Reproducibility

This repository contains the data and code used to reproduce the bibliometric analysis and plots in our survey on **weakly supervised semantic segmentation for remote sensing imagery (WSSS-RS)**.

> **Note:** This repository is intended to support transparency and reproducibility of the bibliometric part of the survey. It is not a standalone software package.

---

## 1. Repository structure

A suggested structure (you can adjust to match your actual folders):

```text
.
├── data_raw/
│   ├── wos_export_2025-10-XX.txt / .csv
│   ├── scopus_export_2025-10-XX.csv
│   ├── ieee_xplore_export_2025-10-XX.csv
│   └── README_data_raw.md
├── data_processed/
│   ├── merged_records.csv           # merged + deduplicated corpus
│   ├── included_studies.csv         # final list of 95 included papers
│   ├── excluded_counts_by_reason.csv
│   └── vosviewer_input_keywords.txt # input files for VOSviewer
├── scripts/
│   ├── 01_parse_and_merge.R
│   ├── 02_deduplicate_records.R
│   ├── 03_prepare_vosviewer_input.R
│   ├── 04_generate_bibliometric_plots.R
│   └── utils_biblio.R
├── vosviewer/
│   ├── keyword_cooccurrence_map.vos
│   ├── authors_map.vos
│   └── README_vosviewer.md
├── figs_reproduced/
│   ├── fig7_publication_trends.png
│   ├── fig8_authors_journals.png
│   ├── fig9_keyword_network.png
│   └── fig10_coauthorship_network.png
└── README.md

