ESC403 Project: Deciding Factors for the US Election in 2016

Authors: Casimir Herold, Linus Gasser, Rieke Goebel

______________________________________________
STRUCTURE
----------------------------------------------
This Lab is divided into four main parts: 
    1. Code 
    2. data 
    3. research
    4. results

______________________________________________
Code
----------------------------------------------
There are often two versions of the code - one for 2016 and then a copied version to also test to predict the 2016 election using 2012 and before (baseline) variables.


_________
00project_proposal
contains our first EDA for the project proposal as well as some codes to create plots for the final presentation
_________
01EDA
code for EDA for the plots in the final presentation
_________
02datacleaning / 06datacleaning_2012
here, the data is cleaned based on the years, Na, dont know, time, variables, ...
After the feature selection, the original df should be selected for the needed features and then re-run through the data cleanin (as needed)
_________
03RandomForest_targetTrumpClinton / 07RandomForest_targetTrumpClinton_2012
contains the RF model as well as the feature selection using gini and permutation to score them.
_________
04cramersV_models_lightGBM_LinearRegression / 08cramersV_models_lightGBM_LinearRegression_2012
selects features based on cramers V and trains both the LR and the lighGBM models. 
_________
05featureselection_score / 09featureselection_score_2012
combines all the feature scores from cramers v, gini, and permuation to one feature score.
After, a selection based on the context of the variables can be done. 
_________
10neural_net
is the code that was written to test the neural net on our data. 
In the second chunk in line 2, the variable name can be changed between 2016 and 2012 to run the NN for the respective predictor variables



______________________________________________
Data 
----------------------------------------------
the data folder contains the original data frame and any and all output dataframes as .csv files that come from the different notebook
source data can be downloaded here: https://www.kaggle.com/datasets/democracy-fund/2016-voter-survey



______________________________________________
Research
----------------------------------------------

+++Finally, the Meta data/ info quide to the data set is deposited here+++ 


______________________________________________
Results
----------------------------------------------
In results, the different plots can be found as images. 
they are dvided into sub-folders based on either their use or in the code they were created in. 



______________________________________________
NOTES
----------------------------------------------
the code is generally documented to the best of our abilities. 

When starting the code and only having the original file in the data folder, RF and CV have to be run iterative with data cleaning as they build on each other.