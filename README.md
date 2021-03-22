# Documentation for "expanded_baseline_vars" Data Set 
# Date: 03/02/2021
# Author: Yizhe (Crystal) Xu 
# Purpose: I expanded the original "baseline.csv" with 30 more variables to conduct the analyses that are listed under the NHLBI R01 grant Aim 2 (SPRINT data) 
# Details:

The original version of this data set is stroed at "/labs/shahlab/datasets/BioLINCC/SPRINT/datasets/SPRINT_2019a.zip/SPRINT-POP/data/baseline.csv". There are 30 columns in this original baseline data set. 

The expanded version of this baseline variable data set (named "expanded_baseline_vars.csv") is stored at (...Jason, please fill this in after you move the data set to a fixed location). There are 63 columns in total with 30 original columns, 3 re-coded columns of the original variables, and 30 newly added columns. 

The additional 30 variables are pulled from several data sets in the "/labs/shahlab/datasets/BioLINCC/SPRINT/datasets/SPRINT_2019a.zip/SPRINT/data" folder. The details are given in the following list: 

- "bl_meds_vars_summary": this is a summarized medication data set using the following 3 original data sets in the "/labs/shahlab/datasets/BioLINCC/SPRINT/datasets/SPRINT_2019a.zip/SPRINT/data/csv" folder:

   - "bl_meds_physexam.csv", "bl_medsphys4m.csv", and "incl_excl.csv". 
   - Eight medication (binary) variables are extracted, in which the mapping were done using the ATC index given by WHOCC <a href='https://www.whocc.no/atc_ddd_index/'>
   
- "labs.sas7bdat": two lab variables are extracted ["RESULT_K", "RESULT_NA"]
- "incl_excl.sas7bdat": one variable is extracted ["CORONARYREVAS"]
- "bp_manage_base.sas7bdat": two variables are extracted ["DIZZY", "SEATHEART"]
- "bl_history.sas7bdat": 17 co-morbidities at basline are extracted ["PVD","PTSD","RHEARTHRITIS","THYROIDDIS","ULCER","GOUT","HIPPROB","OSTEOARTHRITIS","BPH",
                                                                     "LOWBKPAIN","ATRIALFIB","LIVEWITHOTHERS","DEPRESS","ANXIETY","ANEMIA","ALCOHOL","CANCER"]
                      
# Missing Data:

The original "baseline.csv" data set has 6% of the rows with missing data. After the 30 more variables are added, the missing rate increased to 7.5%, meaning that we have complete data on all 63 columns for 92.5% of the rows/patients. 
