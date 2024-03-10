# deep-learning-challenge
# Module 21 Deep Learning Alphabet Soup Challenge
-
# Alphabet Soup Analysis Overview
The purpose of this project is to create a tool for  Alphabet Soup to help select applicants for funding with the best chance of success in their ventures. 
The provided dataset was used to create a binary classifier using a machine learning program to predict whether applicants will be successful if funded by Alphabet Soup.
The provided dataset included more than 34,000 organizations that have received funding from Alphabet Soup over the years. 
The following information was provided in the dataset for use in the program to predict probability of success with at least 75% accuracy:
EIN and NAME—Applicants
APPLICATION_TYPE—Alphabet Soup application type
AFFILIATION—Affiliated sector of industry such as Independent or Company Sponsored
CLASSIFICATION—Government organization classification
USE_CASE—Use case for funding such as Product Development, Preservation, Healthcare, etc.
ORGANIZATION—Organization type such as Association, Co-operative or Trust
STATUS—Active status
INCOME_AMT—Income classification
SPECIAL_CONSIDERATIONS—Special considerations for application
ASK_AMT—Funding amount requested
IS_SUCCESSFUL—Was the money used effectively

# Alphabet Soup Analysis Results
## Data Preprocessing
- The focus of this model is to predict the probability of success for an applicant if they receive funding.
- The IS_SUCCESSFUL data was the target variable used for the model.
- The other columns were used as feature variables for the model except the EIN column.  I originally also removed the NAME column as suggested in the instructions.  However, the accuracy increased when I included the NAME column and binned the NAME data.
- The EIN column was removed since it was only introducing noise into the model and was not needed to predict the probability of success for funding.
- I used binning/bucketing with the APPLICATION_TYPE, CLASSIFICATION, and NAME columns to combine the rare occurrence categories to optimize the model.
- The categorical data was converted into numeric data using get_dummies.
- The data was split into training and testing data and scaled for a more balanced distribution

## Compiling, Training, and Evaluating the Model
I did 5 optimizations to get to the target of over 75% accuracy.
See the Analysis Report for details
Alphabet Soup Analysis.pdf
Alphabet Soup Analysis.pptx

# Summary
Overall, by using machine learning, we can predict with almost 79% accuracy which campaigns will be successful.  This will help us fund campaigns more efficiently. 
It would be ideal to continue to try other models to improve the accuracy even more.   
The greatest gains in accuracy were gained from adding layers and neurons and including the NAME data.  Continuing to adjust the layers, neurons and binning could further increase the prediction accuracy.
The Tanh model could also be used to try to increase the accuracy since it will normalize the data.

# Files Included
Alphabet Soup Analysis.pdf
Alphabet Soup Analysis.pptx
## Deep_Learning_Challenge Folder
- Starter_Code - starter code
- M19_Deep_Learning_RG - my original code
- AlphabetSoupCharity_Optimization - 1st optimization
- AlphabetSoupCharity_Optimization2 - 2nd optimization
- AlphabetSoupCharity_Optimization3 - 3rd optimization
- AlphabetSoupCharity_Optimization4 - 4th optimization
- AlphabetSoupCharity_Optimization5 - 5th optimization
## HDF5 Folder
- These are saved with .keras instead of .h5 due to recommendation since the h5 is legacy and was not working
- AlphabetSoupCharity - original model
- AlphabetSoupCharityOpt1 - optimization 1 file
- AlphabetSoupCharityOpt2 - optimization 2 file
- AlphabetSoupCharityOpt3 - optimization 3 file
- AlphabetSoupCharityOpt4 - optimization 4 file
- AlphabetSoupCharityOpt5 - optimization 5 file

# Resources
I received help from the following
- Instructor - Rufel Estrada
- TA - Manuel Eduardo Sotelo Cervante
- Tutor - Geronimo Perez






