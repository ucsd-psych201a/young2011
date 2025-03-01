# Replication of Study 1A by Liane Young and Rebecca Saxe (2011, Cognition)

## Overview
This repository contains materials for the replication of **Study 1A** from Young & Saxe (2011), which investigates the role of intent in moral judgments across different moral domains. The study follows a **2 (intent: intentional vs. accidental) × 3 (domain: harm, incest, ingestion) between-subjects design**.

## Project Structure
```
├── data/                     # Raw and cleaned datasets
├── scripts/                  # R scripts for analysis and visualization
├── results/                  # Output files, figures, and summary statistics
├── Final_Project_Report.Rmd  # Main replication report in R Markdown
├── README.md                 # This file
```

## Getting Started
### Requirements
To reproduce the analysis, install the following R packages:
```r
install.packages(c("tidyverse", "ggplot2", "car"))
```

### Running the Analysis
1. **Download the repository**: Clone using the command below or download manually.
   ```sh
   git clone https://github.com/ucsd-psych201a/young2011
   ```
2. **Load the dataset**: The dataset is available in `data/moral_judgment_data.csv`.
3. **Run the scripts**:
   - Data cleaning: `scripts/data_cleaning.R`
   - ANOVA analysis: `scripts/anova_analysis.R`
   - Visualization: `scripts/plot_results.R`
4. **Generate the final report**:
   - Run `Final_Project_Report.Rmd` in RStudio or use:
     ```r
     rmarkdown::render("Final_Project_Report.Rmd")
     ```

## Results Summary
- **Harm vs. Incest:** Significant intent × domain interaction (**p < 0.05**), replicating original findings.
- **Incest vs. Ingestion:** No significant interaction (**p > 0.05**), consistent with prior work.
- **Harm vs. Ingestion:** Significant difference (**p < 0.05**), reinforcing harm-purity distinction.

## Contributors
- **Belynda Herrera** (bpherrera@ucsd.edu)
- **Cassie Wang** (tiw037@ucsd.edu)
- **Kexin Jiang** (k3jiang@ucsd.edu)
- **Seyi Lawal** (slawal@ucsd.edu)

## Citation
If using this work, please cite:
> Young, L., & Saxe, R. (2011). *When ignorance is no excuse: Different roles for intent across moral domains.* Cognition, 120(2), 202-214. https://doi.org/10.1016/j.cognition.2011.04.005

## License
This project is released under the **MIT License**.
