\# Youth Substance Use Prediction using Tree-Based Models



\## Overview

This project analyzes and predicts youth substance use using tree-based machine learning models. The goal is to identify patterns in marijuana and alcohol use and determine which factors are most influential.



The models applied include Decision Trees, Random Forest, and Boosting across binary classification, multi-class classification, and regression tasks.



\## Objectives

\- Predict marijuana use through binary classification

\- Predict levels of marijuana use through multi-class classification

\- Predict alcohol use frequency through regression

\- Compare model performance

\- Identify key predictors of substance use



\## Dataset

The dataset used is `youth\_data`, which contains:

\- Demographic variables

\- Behavioral factors

\- Peer influence

\- Substance use information



The dataset was partially preprocessed, and additional cleaning was performed before modeling.



\## Data Cleaning

\- Replaced invalid codes `91`, `93`, `94`, `97`, and `98` with `NA`

\- Removed missing values

\- Used imputed variables when available



\## Data Dictionary (Selected Variables)



\### Binary Classification (Marijuana Use)

\- `MRJFLAG` – Marijuana use (0 = No, 1 = Yes)

\- `YOSELL2` – Selling-related behavior

\- `YOFIGHT2` – Physical fights

\- `IRSEX` – Sex

\- `INCOME` – Household income

\- `EDUSCHLGO` – School enrollment

\- `AVGGRADE` – Average grades

\- `FRDMEVR2` – Friends used marijuana

\- `PARCHKHW` – Parent checks homework

\- `RLGATTD` – Religious attendance



\### Multi-class Classification (Marijuana Levels)

\- `STNDSMJ` – Marijuana use level

\- `IRSEX` – Sex

\- `INCOME` – Household income

\- `EDUSCHLGO` – School enrollment

\- `AVGGRADE` – Average grades

\- `YOFIGHT2` – Physical fights

\- `FRDMEVR2` – Friends used marijuana

\- `PARCHKHW` – Parent checks homework

\- `RLGATTD` – Religious attendance



\### Regression (Alcohol Use)

\- `ALCYDAYS` – Alcohol use days

\- `IRSEX` – Sex

\- `INCOME` – Household income

\- `EDUSCHLGO` – School enrollment

\- `AVGGRADE` – Average grades

\- `YOFIGHT2` – Physical fights

\- `FRDMEVR2` – Friends used marijuana

\- `PARCHKHW` – Parent checks homework

\- `RLGATTD` – Religious attendance



\## Models Used



\### Decision Tree

\- Used for classification and regression

\- Easy to interpret

\- Helps explain variable importance and tree paths



\### Random Forest

\- Ensemble of many decision trees

\- Improves stability and reduces variance



\### Boosting

\- Sequential tree-based method

\- Focuses on correcting previous prediction errors



\## Results

\- \*\*Decision Tree (Binary):\*\* \~84.6% accuracy

\- \*\*Random Forest (Binary):\*\* \~84.5% accuracy

\- \*\*Boosting (Binary):\*\* \~84.6% accuracy

\- \*\*Decision Tree (Multi-class):\*\* \~75.3% accuracy

\- \*\*Regression Tree:\*\* MSE ≈ 2.70



\## Key Findings

\- Behavioral and peer-related variables were strong predictors

\- Selling-related behavior was highly associated with marijuana use

\- Binary classification performed better than multi-class classification

\- Ensemble methods did not significantly outperform the decision tree in this case



\## Ethical Considerations

\- Predictions may be misused in decision-making

\- There is potential for bias and unfair treatment

\- Models identify patterns, not causation

\- Results should be used for insight, not for labeling individuals



\## Technologies Used

\- R

\- `rpart`

\- `rpart.plot`

\- `randomForest`

\- `gbm`



\## Repository Structure

\- `data/`

&#x20; - `youth\_data.RData`



\- `code/`

&#x20; - `Practical\_Homework\_1.Rmd`



\- `report/`

&#x20; - `Practice Homework 1.pptx`



\- `README.md`



\## Future Work

\- Perform hyperparameter tuning

\- Apply cross-validation

\- Improve multi-class model performance

\- Explore additional predictors



\## Author

Badamgarav Battushig  

DATA 5322 – Statistical Machine Learning II  

Seattle University



\## License

This project is for academic purposes.

