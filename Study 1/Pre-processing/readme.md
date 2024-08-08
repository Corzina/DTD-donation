# Obtain LISS Panel Core Studies Data

I do not own the data used in the empirical part of the article. To obrain it, reader should get access to the LISS Core Studies panel data, as described at https://www.lissdata.nl/use-the-panel

All the data should be downloaded and placed in the folder convenient for the reader, for example: ".../DTD-donation/Study 1/Data" 

A detailed overview of what is included in Core Studies data is avaiable in the codebooks here: https://www.dataarchive.lissdata.nl/study-units/view/1

Make sure to check, upload and unzip (if needed) the following files from related waves of LISS Core Studies:

1) HOME/LISS Data Archive/Background variables/Data Files/English 2024 March/avars_202403_EN_1.0p.zip

2) HOME/LISS Data Archive/Social Integration and Leisure/Data Files/Wave 15/English CSV file/cs23o_EN_1.0p.csv

3) HOME/LISS Data Archive/Personality/Data Files/Wave 15/English CSV file/cp23o_EN_1.0p.csv

Original names of the raw datasets can be kept. Scripts will be able to preprocess it and store the output needed for further steps. Make sure that you follow subsequence described in readme in the root folder, as othervise needed data will be missing.

# Obtain WhatsApp Donated Data

To obtain WhatsApp data, reader should personally contact Stein Jongerius (stein.jongerius@centerdata.nl) to request it, as it was not made publicly available yet. For the WhatsApp data, make sure to request, get and upload the following files, including donated DDPs. Make sure you request and receive the data which includes info (personal tokens) on non-respondents. There should be 4800 observations in total.

1) Main Data Donation file - L_Datadonation_main_1.0p.sav

2) Data Donation file with frame information on non respondents - L_Datadonation_with_non_respondents.sav 

3) A folder with donated DDPs - Pakketjes split 1 & 2

After it, specify the paths to the data used in the scripts to the folder on your computer where you store it. Refer the folder "Pakketjes split 1 & 2" in "explore_script_DTD_preprocessing.qmd". Please, take into account that names for the files provided by Stein Jongerius may differ, as the project is WIP.
