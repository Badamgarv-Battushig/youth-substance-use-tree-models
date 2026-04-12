# Youth Substance Use Prediction using Tree-Based Models

## Overview

This project analyzes youth substance use using tree-based machine learning models.
The goal is to predict marijuana and alcohol use and identify the most important influencing factors.

The models applied include:
- Decision Trees
- Random Forest
- Boosting

These are used across binary classification, multi-class classification, and regression tasks.

## Objectives

- Predict marijuana use (binary classification)
- Predict levels of marijuana use (multi-class classification)
- Predict alcohol use frequency (regression)
- Compare model performance
- Identify key predictors of substance use

## Dataset

- youth_data.Rdata: https://github.com/Badamgarv-Battushig/youth-substance-use-tree-models/blob/main/data/youth_data.Rdata

The dataset contains:
- Demographic variables
- Behavioral factors
- Peer influence
- Substance use information

Note: The dataset was partially preprocessed. Additional cleaning was performed before modeling.

## Data Cleaning

- Replaced invalid codes with NA
- Removed missing values
- Used imputed variables when available

## Data Dictionary (Selected Variables)

### Binary Classification (Marijuana Use)

MRJFLAG   - Marijuana use (0 = No, 1 = Yes)
YOSELL2   - Selling-related behavior
YOFIGHT2  - Physical fights
IRSEX     - Sex
INCOME    - Household income
EDUSCHLGO - School enrollment
AVGGRADE  - Average grades
FRDMEVR2  - Friends used marijuana
PARCHKHW  - Parent checks homework
RLGATTD   - Religious attendance

### Multi-class Classification (Marijuana Levels)

STNDSMJ   - Marijuana use level
IRSEX     - Sex
INCOME    - Household income
EDUSCHLGO - School enrollment
AVGGRADE  - Average grades
YOFIGHT2  - Physical fights
FRDMEVR2  - Friends used marijuana
PARCHKHW  - Parent checks homework
RLGATTD   - Religious attendance

### Regression (Alcohol Use)

ALCYDAYS  - Alcohol use days
IRSEX     - Sex
INCOME    - Household income
EDUSCHLGO - School enrollment
AVGGRADE  - Average grades
YOFIGHT2  - Physical fights
FRDMEVR2  - Friends used marijuana
PARCHKHW  - Parent checks homework
RLGATTD   - Religious attendance

## Models Used

### Decision Tree
- Used for classification and regression
- Easy to interpret
- Helps explain variable importance

### Random Forest
- Ensemble of multiple trees
- Improves stability and reduces variance

### Boosting
- Sequential tree-based method
- Focuses on correcting previous errors

## Results

- Decision Tree (Binary): ~84.6% accuracy
- Random Forest (Binary): ~84.5% accuracy
- Boosting (Binary): ~84.6% accuracy
- Decision Tree (Multi-class): ~75.3% accuracy
- Regression Tree: MSE ≈ 2.70

## Key Findings

- Behavioral and peer-related variables were strong predictors
- Selling-related behavior was highly associated with marijuana use
- Binary classification performed better than multi-class classification
- Ensemble methods did not significantly outperform decision trees

## Ethical Considerations

- Predictions may be misused in decision-making
- Potential bias and unfair treatment
- Models show patterns, not causation
- Results should not be used to label individuals

## Technologies Used

- R
- rpart
- rpart.plot
- randomForest
- gbm

## Repository Structure

data/
  youth_data.RData

code/
  Practical_Homework_1.Rmd

report/
  Practice_Homework_1.pptx

README.md

## Future Work

- Perform hyperparameter tuning
- Apply cross-validation
- Improve multi-class model performance
- Explore additional predictors

## Author

Badamgarav Battushig  
DATA 5322 – Statistical Machine Learning II  
Seattle University

## License

This project is for academic purposes only.
