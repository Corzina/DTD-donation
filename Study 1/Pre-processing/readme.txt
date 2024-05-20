# Obrain LISS Panel and WhatsApp data

To obrain data, reader should:

1) get access to the LISS Core Studies panel data, as described at https://www.lissdata.nl/use-the-panel

2) personally conract Stein Jongerius (stein.jongerius@centerdata.nl) from centerdata to request WhatsApp data, as it is not made publicly available yet. 

All the data, including donated DDPs, should be downloaded placed in the following folder: ".../DTD-donation/Study 1/Data" 

A detailed overview of what should be the part of the data is avaiable in the codebooks here: https://www.dataarchive.lissdata.nl/study-units/view/1

Make sure to check, upload and unzip (if needed) the following files from related waves of LISS Core Studies:

1) HOME/LISS Data Archive/Background variables/Data Files/English 2024 March/avars_202403_EN_1.0p.zip

2) HOME/LISS Data Archive/Social Integration and Leisure/Data Files/Wave 15/English CSV file/cs23o_EN_1.0p.csv

3) HOME/LISS Data Archive/Personality/Data Files/Wave 15/English CSV file/cp23o_EN_1.0p.csv

4) HOME/LISS Data Archive/Politics and Values/Data Files/Wave 15/English CSV file/cv23o_EN_1.0p.csv

Original names of the raw datasets can be kept. Scripts will be able to preprocess it and store the output needed for further steps. Make sure that you follow subsequence described in readme in the root folder, as othervise needed data will be missing.

Next, for the WhatsApp data, make sure to request, get and upload the following files in the ".../DTD-donation/Study 1/Data/" folder:

1) Main Data Donation file - L_Datadonation_main_1.0p.sav

2) Data Donation file with frame information on non respondents - L_Datadonation_with_non_donators.sav

3) A folder with donated DDPs - Pakketjes split 1 & 2

After it, specify the paths to the data used in the scripts.
