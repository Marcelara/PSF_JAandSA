# 📘 Project Title

## 📝 Overview

This repository contains data and analysis scripts related to the **effect of stress on phytohormone concentrations**. The project explores differences in **JA and SA responses** compared to controls under various conditions.

## 📂 Repository Contents

### 🔹 **Amplicon Data Preprocessing**

- `Amplicon_data_preprocesing/amplicon_data_preprocesing.Rmd`: R Markdown script for preprocessing amplicon sequencing data.
- `Amplicon_data_preprocesing/uploading_raw_sequences/`: Contains raw sequence filenames and sample naming scripts.

### 🔹 **Data Files**

- `Data/amplicon_data/`: Contains 16S and ITS sequencing data, including mapping files, quality plots, taxonomy assignments, and phylogenetic trees.
- `Data/EPG_data/`: Contains electrophysiological recordings of plant responses (`EPG_table.csv`, `EPG_time.csv`, etc.).
- `Data/phyloseq_objects/`: Stores phyloseq objects (`ps_16S_Full.RData`, `ps_ITS_Full.RData`, etc.).
- `Data/plant_data/`: Includes plant response measurements (aphids, biomass, caterpillars, phytohormones).

### 🔹 **Figures and Analysis Scripts**

- `Figure_1_Plant_responses_conditioning_phase.Rmd`: Code for Figure 1.
- `Figure_2_Stress_induced_changes_Bacteria.Rmd`: Code for Figure 2 (Bacterial changes due to stress).
- `Figure_3_Stress_induced_changes_Fungi.Rmd`: Code for Figure 3 (Fungal changes due to stress).
- `Figure_4_Plant_responses_feedback_phase.Rmd`: Code for Figure 4.
- `Figures_S3_S4_S5_S6.Rmd`: Supplementary figure scripts.

### 🔹 **R Results & Statistical Analysis**

- `R_results/Fig_2_Stress_induced_changes_Bacteria/`: Differential abundance results and phylogenetic trees for 16S.
- `R_results/Fig_3_Stress_induced_changes_Fungi/`: Differential abundance results for ITS fungal communities.
- `PSF_JAandSA.Rproj`: R project file.

## 📊 Data Description

The dataset includes:

- **ID**: Unique identifier for each sample
- **Stress**: Different stress conditions applied
- **Phytohormone**: Measured phytohormone (e.g., JA, SA, ABA)
- **Concentration**: Measured phytohormone concentration (ng/g)
- **Other metadata** relevant to experimental conditions

## 📈 Analysis Workflow

1. **Preprocessing**: Import and clean the dataset.
2. **Normalization**: Transform counts to median-scaled values.
3. **Statistical Modeling**: Fit mixed models to assess treatment effects.
4. **Visualization**: Generate boxplots and statistical comparisons.

## 🛠️ Usage Instructions

To reproduce the analysis:

```r
# Install required packages
install.packages(c("phyloseq", "lme4", "emmeans", "ggplot2"))

# Run preprocessing script
source("Amplicon_data_preprocesing/amplicon_data_preprocesing.Rmd")

# Run statistical analysis
source("Figure_2_Stress_induced_changes_Bacteria.Rmd")
```

## 📢 Contributing

If you find any issues or have suggestions for improvement, feel free to open an **issue** or submit a **pull request**!

## 📄 License

This project is released under the [MIT License](LICENSE).

