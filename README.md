# Zoonotic Disease Knowledge and Experience Among Health Professionals in Ghana

## Data Overview
This repository contains an R-based analysis of zoonotic disease knowledge and experience among 152 health professionals in rural Ghana (Tolon and Nyankpala) as of June 1, 2025. The dataset includes demographic characteristics, general zoonosis knowledge, prioritized zoonoses knowledge, knowledge of five specific zoonoses (Anthrax, Rabies, Brucellosis, Trypanosomiasis, Tuberculosis), One Health knowledge, and experience with zoonotic diseases and One Health activities. The sample is predominantly Nurses (88.8%), with small groups of Biomedical Scientists (5.3%), Pharmacists (3.3%), and Medical Doctors (2.6%).

**Dataset**: 152 respondents, 121 variables including:
- **Demographics**: Age (mean: 31.09 years), sex (57.2% female), profession, years of experience (mean: 3.61 years), location (79.6% Tolon), animal ownership (59.9% Yes).
- **Knowledge Scales**:
  - General Zoonosis (0–3, mean: 1.53, Cronbach’s α = 0.88).
  - Prioritized Zoonoses (0–9, mean: 6.53).
  - Five Zoonoses (Anthrax, Rabies, Brucellosis, Trypanosomiasis, TB; 0–7/8, means: 2.06–4.02).
  - One Health (0–14, mean: 9.18).
- **Experience**: Workshops (7.2% Yes), collaboration (5.9% Yes, Rabies-only), encounters (33.6% Yes, mostly Rabies), public education (9.2% Yes, mostly Rabies), training (One Health: 21.1% Yes, Zoonosis: 35.5% Yes).

**Key Observations**:
- **Demographics**: Significant differences in age (p=0.004) and location (p=0.003) by profession. Nurses are younger (mean: 30.4 years) and mostly in Tolon (84%). Medical Doctors are older (mean: 42.3 years) and mostly in Nyankpala (75%).
- **Knowledge**: Strong for prioritized zoonoses (87.5% high) and One Health (78.9% high), moderate for general zoonosis (46.1% high). Rabies knowledge is highest (mean: 4.02/8), Brucellosis lowest (mean: 2.06/7).
- **Experience**: Low engagement in workshops, collaboration, and public education, with Rabies dominating (28.3% encounters, 5.9% collaboration, 8.6% education). Biomedical Scientists lead in training, Nurses in encounters.

**Limitations**: Nurse-dominated sample (135/152) reduces power for other professions. Sparse data for non-Rabies outcomes and small non-Nurse groups limit analyses. Unadjusted confounders (e.g., age, location) may influence results.

## Relationships
The analysis examines associations between profession and various outcomes using ANOVA, Fisher’s exact tests, and Kruskal-Wallis tests due to small sample sizes and low expected counts.

### Profession vs. Knowledge
- **General Zoonosis Knowledge** (zoonosis_knowledge_total/cat):
  - ANOVA: F(3,148)=0.239, p=0.869 (not significant).
  - Fisher’s (high/low): p=0.965.
  - Observation: No profession-based differences. Nurses show widest score range (0–3), Medical Doctors and Biomedical Scientists slightly higher medians (1–2), but small samples (n=4, n=8) limit power.
- **Prioritized Zoonoses Knowledge** (prioritized_zoonoses_knowledge_total/cat):
  - ANOVA: F(3,148)=1.399, p=0.246 (not significant).
  - Fisher’s (high/low): p=0.793.
  - Observation: Medical Doctors score highest (median ~8), but no significant differences. Nurses dominate counts (118/133 high).
- **Five Zoonoses Knowledge**:
  - **Anthrax**: ANOVA p=0.421, Fisher’s p=1.0 (not significant). Nearly invariant (151/152 inadequate).
  - **Rabies**: ANOVA p=0.505, Fisher’s p=1.0 (not significant). Highest scores (mean: 4.02/8), but 150/152 inadequate.
  - **Brucellosis**: ANOVA p=0.0318 (significant). Medical Doctors/Biomedical Scientists > Nurses. All inadequate.
  - **Trypanosomiasis**: ANOVA p=0.0107 (significant). Medical Doctors/Biomedical Scientists > Nurses. All inadequate.
  - **TB**: ANOVA p=0.12 (not significant). Medical Doctors score high (all 6), but no significant differences.
- **One Health Knowledge** (one_health_knowledge_total/cat):
  - ANOVA: F(3,148)=1.4448, p=0.2321 (not significant).
  - Fisher’s (high/low): p=0.357.
  - Individual Issues: Significant for armed_conflict_one_health (p=0.006, Medical Doctors 100% Correct), others p=0.17–0.881 (not significant).
  - Observation: Medical Doctors (mean: 12.50) and Pharmacists (100% high) excel, but small samples limit significance.

### Profession vs. Experience
- **General Experience**:
  - Zoonosis Training: Fisher’s p=0.004 (significant). Biomedical Scientists (87.5% Yes) > Nurses (34.1% Yes).
  - Others (workshops, collaboration, encounters, public education, One Health training): p=0.105–1.0 (not significant).
  - Observation: Biomedical Scientists lead in training, Nurses in encounters (34.1% Yes).
- **Collaboration**:
  - collab_rabies: Fisher’s p=1.0, Kruskal-Wallis p=0.754 (not significant). Nurse-only (6.7% Yes, Rabies-only).
  - Others (Anthrax, Brucellosis, Trypanosomiasis, TB): All 0, no analysis possible.
- **Encounters**:
  - encounter_trypanosomiasis: Kruskal-Wallis p=0.000 (significant). Nurse-only (1 Yes).
  - encounter_tuberculosis: Kruskal-Wallis p=0.001 (significant). Nurse-only (3 Yes).
  - encounter_rabies: p=0.277, encounter_anthrax: p=0.969 (not significant). Rabies most encountered (Nurses: 30.4%, Biomedical Scientists: 25%).
  - encounter_brucellosis: All 0.
- **Public Education**:
  - educate_rabies: Fisher’s p=1.0, Kruskal-Wallis p=0.62 (not significant). Nurse-only (8.6% Yes, Rabies-only).
  - Others: All 0.

**Key Trends**:
- Significant differences: Brucellosis/Trypanosomiasis knowledge (Medical Doctors/Biomedical Scientists > Nurses), armed conflict knowledge (Medical Doctors > Nurses), zoonosis training (Biomedical Scientists > Nurses), Trypanosomiasis/TB encounters (Nurses > Others).
- Nurses dominate due to sample size (n=135), driving encounters/collaboration/education.
- Rabies dominates engagement (28.3% encounters, 5.9% collaboration, 8.6% education).
- Medical Doctors show high knowledge, low engagement; Pharmacists minimal involvement.

## Zoonotic Analysis
- **Knowledge Strengths**: Rabies (mean: 4.02/8, 92.8% correct prioritization), Anthrax (83.6% correct prioritization), and One Health (mean: 9.18/14) are strongest. Brucellosis is weakest (mean: 2.06/7, all inadequate).
- **Engagement**: Low across workshops (7.2%), collaboration (5.9%), and education (9.2%). Rabies dominates, with Nurses leading due to sample size. Biomedical Scientists excel in training (87.5% zoonosis, 50% One Health).
- **Encounters**: 33.6% report encounters, primarily Rabies (28.3%), with rare cases of Trypanosomiasis (0.7%), TB (2.0%), Anthrax (1.3%). Nurses drive encounters, followed by Biomedical Scientists (Rabies only).
- **Visualizations**:
  - **Boxplots**: Show Medical Doctors’ high knowledge medians, Nurses’ wide spread.
  - **Stacked Bar Plots**: Highlight Nurse-dominated, low “Yes” proportions for engagement.
  - **Dodged Bar Plots**: Confirm Nurses’ exclusive Rabies collaboration/education.
  - **Heatmap**: Visualizes Nurses’ dominance in Rabies encounters, sparse non-Rabies encounters.

## Association or Relationships Analysis
- **Statistical Methods**:
  - **ANOVA**: Used for numeric knowledge scores (e.g., zoonosis_knowledge_total, one_health_knowledge_total).
  - **Fisher’s Exact Test**: Used for categorical outcomes due to low expected counts (<5).
  - **Kruskal-Wallis Test**: Used for binary collaboration/encounter/education variables.
- **Significant Associations**:
  - Brucellosis knowledge scores: p=0.0318, Medical Doctors/Biomedical Scientists > Nurses.
  - Trypanosomiasis knowledge scores: p=0.0107, Medical Doctors/Biomedical Scientists > Nurses.
  - Armed conflict One Health knowledge: p=0.006, Medical Doctors > Nurses.
  - Zoonosis training: p=0.004, Biomedical Scientists > Nurses.
  - Trypanosomiasis encounters: p=0.000, Nurses > Others.
  - Tuberculosis encounters: p=0.001, Nurses > Others.
- **Non-Significant Associations**: General zoonosis knowledge, prioritized zoonoses knowledge, One Health knowledge (overall), Rabies/Anthrax knowledge, most experience variables (e.g., workshops, collaboration).
- **Challenges**: Small non-Nurse sample sizes (Medical Doctors: 4, Pharmacists: 5) and sparse data (e.g., 0–9.2% Yes for collaboration/education) reduce power. Invariant categorical outcomes (e.g., all inadequate for Brucellosis/TB) limit tests.

## Conclusion
The analysis reveals strong knowledge of prioritized zoonoses (87.5% high) and One Health (78.9% high), with moderate general zoonosis knowledge (46.1% high) among rural Ghanaian health professionals. Rabies is the best-understood and most engaged zoonosis, while Brucellosis knowledge is weakest. Significant profession-based differences include:
- Medical Doctors and Biomedical Scientists excel in Brucellosis and Trypanosomiasis knowledge.
- Medical Doctors show perfect armed conflict One Health knowledge.
- Biomedical Scientists lead in zoonosis training (87.5% Yes).
- Nurses dominate Trypanosomiasis and Tuberculosis encounters.

Engagement in zoonosis-related activities is low, with Nurses driving most outcomes due to their large sample size (88.8%). Pharmacists show minimal involvement. Sparse data and small non-Nurse samples limit detection of differences, and unadjusted confounders (e.g., age, location) may influence results.

**Recommendations**:
- **Targeted Training**: Enhance Nurses’ knowledge of Brucellosis and Trypanosomiasis.
- **Engagement Opportunities**: Increase workshops and collaboration for Medical Doctors and Pharmacists.
- **Rabies Focus**: Leverage existing Rabies knowledge/encounters for public health campaigns.
- **Further Research**: Adjust for confounders (age, location) and increase sample sizes for non-Nurses to improve power.

## Installation
- **R Version**: 4.0+ recommended.
- **Packages**:
  ```R
  install.packages(c("dplyr", "ggplot2", "stats"))
