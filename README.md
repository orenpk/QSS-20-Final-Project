**STARTling Disparities: Racial Gaps in the START Program**
 
This project explores the impact of the COVID-19 pandemic on children and families with intellectual and developmental disabilities (IDD), using data from the START (Systemic, Therapeutic, Assessment, Resources, and Treatment) program in NH. Here's an overview of the Jupyter Notebooks used in the analysis:


[00_data_cleaning.ipynb](https://github.com/orenpk/QSS-20-Final-Project/blob/393fe1d5082fc3fc1626f22e5f92f0b3809ebef1/code/00_data_cleaning.ipynb)


Input: Raw SIRS Demographics, SIRS ABC, and FEIS datasets.

Purpose: Cleans and prepares the data for analysis. This includes standardizing race/ethnicity categories, merging the SIRS datasets, and merging the combined SIRS dataset with the FEIS dataset.

Output: Cleaned and merged datasets (sirs_demo_abc_clean.csv and feis_sirs_demo_merged.csv) for subsequent analysis.


[01_demographic_disparities_analysis.ipynb](https://github.com/orenpk/QSS-20-Final-Project/blob/393fe1d5082fc3fc1626f22e5f92f0b3809ebef1/code/01_demographic_disparities_analysis.ipynb)


Input: Cleaned and merged datasets (sirs_demo_abc_clean.csv).

Purpose: Conducts a difference-in-differences analysis to assess changes in adverse childhood experiences (ACEs) and behavioral health before and after the pandemic onset. It also examines disparities in enrollment rates in START services by race/ethnicity.

Output: Statistical results and visualizations (tables, figures) highlighting any significant changes or disparities related to ACEs, behavioral health, and enrollment.


[02_feis_analysis.ipynb](https://github.com/orenpk/QSS-20-Final-Project/blob/393fe1d5082fc3fc1626f22e5f92f0b3809ebef1/code/02_feis_analysis.ipynb)

Input: Cleaned and merged dataset (feis_sirs_demo_merged.csv).

Purpose: Performs topic modeling using Latent Dirichlet Allocation (LDA) on open-ended survey responses about service needs and advice. It also quantifies and visualizes changes in satisfaction with services before and after the pandemic.

Output: Identified topics, topic prevalence over time and by race/ethnicity, visualizations (heatmap, forest plot) of satisfaction changes, and relevant statistics.


**Important Note: These notebooks are designed to be run sequentially. The output of one notebook serves as the input for the next.**
