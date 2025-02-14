# 📘 Jasmonic and Salicylic Acid Pathways Shape the Rhizosphere Microbiome, affecting Aphid Herbivory and Soil-Mediated Insect-Plant Interactions

## 📝 Overview

This repository contains data and analysis scripts related to the manuscript **Jasmonic and Salicylic Acid Pathways Shape the Rhizosphere Microbiome, affecting Aphid Herbivory and Soil-Mediated Insect-Plant Interactions**. This project explores differences in stress-induced responses by both the JA and SA defense pathways in a set of plant-soil feedback experiments.

## 📂 Repository Contents

### 🔹 **Amplicon Data Preprocessing**

- `Amplicon_data_preprocesing/amplicon_data_preprocesing.Rmd`: R Markdown script for preprocessing 16S and ITS amplicon sequencing data. Start here before running Figure_2 and Figure_3 scripts.

### 🔹 **Data Files**

- `Data/amplicon_data/`: Contains 16S and ITS DADA2 pre-processed data, including mapping files, quality plots, taxonomy assignments, and phylogenetic trees.
- `Data/EPG_data/`: Contains EPG recordings of aphid behavioral responses from the low-density PSF experiment (`EPG_table.csv`, `EPG_time.csv`, etc.).
- `Data/phyloseq_objects/`: Stores processed phyloseq objects, with both experiments together (i.e. _Full) or in a list of the two experimnents (i.e. _ByExperiment). This is the input for all microbiome analyses.
- `Data/plant_data/`: Includes all of the plant response measurements, one dataframe per type of data (aphids, biomass, caterpillars, phytohormones, glucosinolates).

### 🔹 **Analysis Scripts**

- `Figure_1_Plant_responses_conditioning_phase.Rmd`: Code for Figure 1.
- `Figure_2_Stress_induced_changes_Bacteria.Rmd`: Code for Figure 2 (Bacterial changes due to stress).
- `Figure_3_Stress_induced_changes_Fungi.Rmd`: Code for Figure 3 (Fungal changes due to stress).
- `Figure_4_Plant_responses_feedback_phase.Rmd`: Code for Figure 4.
- `Figure_5_PSF_responses_to_low_aphid_sensity.Rmd`: Code for Figure 5.
- `Figures_S3_S4_S5_S6.Rmd`: Supplementary figure scripts.

### 🔹 **R_Results**

- `R_results/Fig_2_Stress_induced_changes_Bacteria/`: Differential abundance results and phylogenetic trees for 16S.
- `R_results/Fig_3_Stress_induced_changes_Fungi/`: Differential abundance results for ITS fungal communities.

## 📢 Contributing

If you find any issues or have suggestions for improvement, feel free to open an **issue** or submit a **pull request**!

## 📄 License

This project is released under the [MIT License](LICENSE).

