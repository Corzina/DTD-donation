# Introduction

Following data archive encorporates everytihng needed to reproduce analysis used in our paper: "Selectivity in Donated Digital Trace Data: Mechanisms of Nondonation at Different Stages of the Data Donation Process". In the first part of the study, we utilize binary logistic model to identify variables associated with higher data donation rates. We then utilize multinomial logistic regression with donators as the reference category to model the relationships between different response categories (non-respondents, non-compliers, non-contributors, and donators), aiming to identify group-specific effects. Then, we check whether 2 types of Digital Trace Data, number of contacts and number of group chats in WhatsApp, can be predicted with the same set of predictors, which allows us to identify confounders introducing nondonation bias. Finally, we examine differenes in predicted values for different types of non-donators, which allows us to assess size of the bias in donated data.  

___

# Information About the Data

For our study, we utilize data from the LISS panel, a probability-based online household panel of the general population in the Netherlands. Our research uses data from the Wave 15 (2023) of the LISS Core studies. More particularly, we use 1) LISS Core Study 4: Social Integration and Leisure, 2) LISS Core Study 7: Personality, and 3) LISS Core background variables: Household Box. Variables used are described in more details in the postprocessing/data folders in the attached tables. 

The WhatsApp Data Donation study was also conducted on the LISS panel. It involved 4,800 randomly selected panel members and collected data on device usage and phone activities in early 2023, with a focus on data donation behaviors. From this source, both DDPs and survey results were used, so reader should make sure they are available on the computer. 
___

# Analysis Guide

We recommend to follow the following step-by-step algorithm for those who want to fully reproduce our study:

1) Gain access to the LISS panel and request access to the data donation study. Request and store the raw data, as described in .../Pre-processing/Readme.txt

2) Run the scripts in the following order:
   
2.1. .../DTD-donation/Study 1/Pre-processing/Scripts/Explore_script_corestudies.Rmd - this script inputs raw data from the LISS core studies and saves its recoded and processed version. 

2.2. .../DTD-donation/Study 1/Pre-processing/Scripts/Explore_script_whatsappdat.Rmd  - this script inputs raw data from the WhatsApp data donation study and saves its recoded and processed version. 

2.3. .../DTD-donation/Study 1/Pre-processing/Scripts/Explore_script_fulldata.Rmd - this script joins and cleans the data from 2 previously mentioned sripts. 

2.4. .../DTD-donation/Study 1/Pre-processing/Scripts/Explore_script_DTD_preprocessing.Qmd - This script parses DDPs, saving actual number of contacts in the files available to reader.

All the scripts require you to **adjust input and output paths** on your computer. You are required to specify path to repository (.../DTD-donation) correctly in the beginning and end of each script, depending on where you want to store the data. 

3) To reproduce the study, then run:
   
3.1. .../DTD-donation/Study 1/Scripts/Analysis_script.Rmd - do not forget to adjust input paths, keeping in mind that you have uploaded repository correctly.

4) Postprocessing is by default done in the end of presented scripts. As a result, outputing tables are saved and provided to the reader.  



