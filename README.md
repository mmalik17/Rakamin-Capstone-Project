# PROJECT OVERVIEW
- Build machine learning model that can predict the customer response of the marketing campaign 
- The dataset source is from Kaggle : https://www.kaggle.com/datasets/rodsaldanha/arketing-campaign

# CONTENTS
<b> Requirement for running the code </b> <br>
Library needed to be installed

<b> 1. Business Understanding </b>
- Background Problems
- Purpose
- Scope

<b> 2. Data Understanding and Preparation </b>
- Feature that available
- Exploratory Data Analysis
- Data Preprocessing

<b> 3. Machine Learning Modelling </b>
- Modelling Process
- Model Evaluation

<b> 4. Business Insight </b>
- Evaluation
- Action Items  

# <b> Requirement for running the code </b>

# <b> 1. Business Understanding </b>
## Background Problems
The campaign carried out by a retail company was less effective, as seen from the campaign response which only reached 14.91%. As a results, the profit obtained is not optimal.

## Purpose
- Goals: Optimizing profits by creating more targeted marketing campaigns.
- Objective: Create machine learning models to predict customers who are most likely to receive certain promotions so as to make campaigns more targeted and get optimal profits
- Business Metrics : Profitability

## Scope
The model only can give the result whether customer responses the campaign or not, but cannot explain the reason behind the customer response

Machine learning Output : Customer response label from given customer characteristic

# <b> 2. Data Understanding and Preparation </b>
## Feature that available

## Exploratory Data Analysis
## Data Preprocessing
- Drop all missing value because the number of missing value is only 1.07% of the number of row
- Create new feature such as kidsorteen, generation, campaign result, and total spending
- Label encode the marital status and year customer
- One-Hot Encoding for education adn generation column
- Split data train with data test
- Drop outlier with Z-score
- feature transformation with logistic transformation and normalisation
- Handle imbalance class with random oversampling technique

# <b> 3. Machine Learning Modelling </b>
## Modelling Process
## Model Evaluation

# <b> 4. Business Insight </b>
## Evaluation
## Action Items  
