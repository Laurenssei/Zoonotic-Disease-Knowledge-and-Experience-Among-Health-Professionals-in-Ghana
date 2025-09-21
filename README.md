
# Knowledge and Perception of Zoonotic Diseases among Healthcare Professionals in Ghana

📄 Full Report: [View Analysis](Knowledge and Perception of Zoonotic Diseases among Healthcare Professionals, Ghana.html)

## Overview
This project evaluates the knowledge levels and perceptions of zoonotic diseases and One Health concepts among 152 healthcare professionals in rural Ghana, focusing on associations with professional roles. Drawing from a 2025 survey in Tolon and Nyankpala districts, the analysis assesses general and disease-specific knowledge, reliability of scales, and experiences with zoonotic encounters, collaborations, and training. By employing statistical tests to explore profession-based differences, the study reveals strengths in prioritized zoonoses awareness and gaps in engagement, informing targeted interventions to enhance zoonotic disease surveillance and One Health integration in resource-limited settings.

## Dataset Summary
- **Source**: Primary survey data from healthcare professionals in Tolon and Nyankpala districts, Ghana (2025).
- **Sample Size**: 152 respondents.
- **Key Variables**: Demographics (age, sex, profession, experience, location, animal ownership); knowledge scores (general zoonosis, prioritized zoonoses, specific diseases, One Health; 66 items total); experience indicators (encounters, workshops, collaborations, training, public education; binary and categorical).
- **Note**: Raw data is not included due to confidentiality. Please contact me for collaboration requests.

## Objectives
- Assess knowledge of general zoonoses, prioritized diseases in Ghana, five selected zoonoses (anthrax, rabies, brucellosis, trypanosomiasis, tuberculosis), and One Health principles.
- Examine associations between knowledge levels and healthcare professions (nurses, medical doctors, biomedical scientists, pharmacists).
- Evaluate experiences with zoonotic disease encounters, collaborations, public education, and training by profession.
- Identify reliability of knowledge scales using Cronbach's alpha and highlight significant demographic and experiential patterns.


## Methods
- Descriptive statistics (means, frequencies, cross-tabulations) and visualizations (boxplots, stacked bar plots, heatmaps) for profiling knowledge and experiences.
- Reliability analysis using Cronbach's alpha for knowledge scales (overall α=0.88).
- Inferential tests: ANOVA for continuous knowledge scores, Fisher's exact and Kruskal-Wallis for categorical/binary associations by profession.
- Non-parametric adjustments for violations (e.g., low expected counts, sparsity) to handle imbalanced data and small subgroups.

## Key Findings
- General zoonosis knowledge is moderate (mean 1.53/3, 46.1% high), while prioritized zoonoses (mean 6.53/9, 87.5% high) and One Health (mean 9.18/14, 78.9% high) are strong; rabies knowledge leads among specific zoonoses (mean 4.02/8), brucellosis lags (mean 2.06/7).
- Significant profession-based differences in brucellosis (p=0.032) and trypanosomiasis (p=0.011) knowledge scores, with medical doctors and biomedical scientists outperforming nurses; One Health armed conflict knowledge favors medical doctors (p=0.006).
- Engagement is low overall (e.g., workshops 7.2%, collaborations 5.9%), but significant for zoonosis training (p=0.004, biomedical scientists at 87.5%) and encounters with trypanosomiasis (p<0.001) and tuberculosis (p=0.001), nurse-dominated.
- Nurses (88.8% of sample) drive most experiences ( 34.1% zoonotic encounters, 30.4% rabies), while medical doctors show highest knowledge but lowest engagement; rabies dominates all activities.



## How to Reproduce the Analysis
### Requirements
- R (version 4.0 or higher)
- RStudio
- R packages: tidyverse, ggplot2, dplyr, psych (for Cronbach's alpha), stats (for ANOVA/Fisher's exact)

### Steps
1. Clone this repository.
2. Open the `.Rmd` in RStudio.
3. Install required packages if not already installed (e.g., `install.packages(c("tidyverse", "psych"))`).
4. Knit the R Markdown file to generate the HTML report.
Data not included due to confidentiality. Please contact me for collaboration requests.

## Repository Structure
├── analysis.Rmd         # R Markdown source file  
├── analysis.html        # Knitted HTML report  
├── README.md            # Project description  

## License / Citation
This project is for academic and research purposes. Please cite appropriately if referenced, e.g., Sei, Lawrence. (2025). Knowledge and Perception of Zoonotic Diseases among Healthcare Professionals in Ghana.



