# Introduction

Following data archive encorporates everytihng needed to reproduce 2 studies.

Study 1 is an empirical data analysis. In this study, we first compare the distributional differences among groups of non-respondents, non-compliers, non-contributors, and donators using Kruskal-Wallis tests, applying Bonferroni correction to adjust for multiple comparisons. Next, binary logistic models are employed to identify variables associated with higher data donation rates, allowing for the examination of mean differences and interaction effects among predictors. We then utilize multinomial logistic regression with donators as the reference category to model the relationships between different response categories, aiming to identify group-specific effects. To address potential sample size imbalances, we create a balanced sample through random sampling and trimming, ensuring robust and unbiased analysis.

In Study 2, we aim to identify the most effective predictive modeling approach for using survey data to predict donation tendencies (DTD) among different types of non-donators. We apply a variety of predictive models to both empirical and simulated datasets, enabling a comparative analysis of their performance in real-world and controlled scenarios. Initially, we run the models on empirical data, followed by generating simulated data based on key characteristics influencing model performance. This dual approach allows us to evaluate how closely the simulated data replicate real-world patterns. Finally, we compare the performance of these models to determine which method provides the best predictive accuracy.

___

# Information About the Data

For Study 1, we utilize data from the LISS panel, a probability-based online household panel of the general population in the Netherlands, and data from the WhatsApp Data Donation project. Our study uses data from the 2023 waves of the LISS panel. More particularly, we use 1) LISS Core Study 4: Social Integration and Leisure, 2) LISS Core Study 7: Personality, 3) LISS Core Study 8: Politics and Values, 4) LISS Core background variables: Household Box. They are described in more details in the postprocessing/data folders in the attached tables. Described data is needed to run the analysis.

The WhatsApp Data Donation project, another data source incorporated in our research needed for both Study 1 and Study 2, involved 4,800 randomly selected panel members and collected data on device usage and phone activities in early 2023, with a focus on data donation behaviors. From this source, both DDPs and survey results were used, so reader should make sure they are available on the computer. 

For study 2, we use simulated data, which however uses data from the study 1 in a simulation process. It is provided in the Study 2 folder, but reader will not be able to simulate it himself unless he has access to the data utlizied in study 1. He will be, however, be able to run the analysis on the provided data. 
___

# Analysis Guide

We recommend to follow the following step-by-step algorithm for those who want to fully reproduce our study:

1) Gain access to the LISS panel and request access to the data donation study.

2) Run the scripts in the following order:
   
2.1. .../DTD-donation/Study 1/Pre-processing/Scripts/Explore_script_corestudies.Rmd - this script inputs raw data from the LISS core studies and saves its recoded and processed version. 

2.2. .../DTD-donation/Study 1/Pre-processing/Scripts/Explore_script_whatsappdat.Rmd  - this script inputs raw data from the WhatsApp data donation study and saves its recoded and processed version. 

2.3. .../DTD-donation/Study 1/Pre-processing/Scripts/Explore_script_fulldata.Rmd - this script joins and cleans the data from 2 previously mentioned sripts. 

2.4. .../DTD-donation/Study 1/Pre-processing/Scripts/Explore_script_DTD_preprocessing.Qmd - Needed for study 2. This script parses DDPs, saving actual number of contacts in the files available to reader.

All the studies require you to adjust input and output paths to your computer if you uploaded repository. Specify part to repository (.../DTD-donation) correctly in each script. They should handle saving data automatically. 

3) To reproduce Study 1, run:
   
3.1. .../DTD-donation/Study 1/Scripts/Analysis_script_1.Rmd - do not forget to adjust input paths, keeping in mind that you have uploaded repository correctly.
In the end, Save the resulting data as described in the script, as it will be needed for Study 2

4) To reproduce Study 2, run:
   
4.1. .../DTD-donation/Study 2/Scripts/Analysis_script_2.Rmd - do not forget to adjust input paths, keeping in mind that you have uploaded repository correctly.

5) Postprocessing is by default done in the end of presented scripts. As a result, outputing tables are saved and provided to the reader.  



