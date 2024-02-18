# PROJECT OVERVIEW
### <b> Project Title: </b> Optimize the Marketing Campaign using Logistic Regression

Build machine learning model that can predict the customer response of the marketing campaign to optimize the marketing campaign performance
- The dataset source is from Kaggle : https://www.kaggle.com/datasets/rodsaldanha/arketing-campaign
- The complete explanation about this project is available on PDF file: <br>
  https://github.com/mmalik17/Rakamin-Capstone-Project/blob/main/Project%20Presentation.pdf
- The complete Phyton code is available in this notebook link: <br>
  https://github.com/mmalik17/Rakamin-Capstone-Project/blob/main/Python_code.ipynb

# <b> Requirement for running the code </b>
Library needed to be installed: <br>
- Data Analysis: Numpy, Pandas, Matplotlib, Seaborn
- Data Preprocessing: Datetime, sklearn, scipy, imblearn
- Modelling : sklearn, shap, xgboost

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
## Data Understanding 
![column](https://github.com/mmalik17/marketing-campaign-analysis/blob/main/fig/Column-List.jpg?raw=true)
<br>
This table has 28 columns with 'Response' column is regarded as a label. Among 27 features, this table has 3 categorical columns and 24 numerical columns.
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
The modelling process use 6 kinds of ML model. 

- Modelling result without hyperparameter:
![Result](https://github.com/mmalik17/marketing-campaign-analysis/blob/main/fig/without-hyperparam.jpg?raw=true)
- Modelling result with hyperparameter:
![Result](https://github.com/mmalik17/marketing-campaign-analysis/blob/main/fig/with-hyperparam.jpg?raw=true)

## Model Evaluation
In this project, the most important machine learning metric is <b>Recall</b>. 

<b> Reasoning: </b> <br>
Big value of Recall means small amount of false negative. False negative means the ML model predicts the customer would response, while actually not. <br>
Big false negative will prevent the marketer from sending the campaign to potential customer. The impact is, there will be loss potential revenue

The model that have the greatest recall value is <b> Logistic Regression with Hyperparameter </b>

# <b> 4. Business Insight </b>
## Insight from Model
- From all of the models used, Logistic regression has the highest recall value of 84%.
- The precision value of the model is low (39%), this will result in an increase in campaign costs. 
- However, low precission is better than low recall because low recall means eliminating potential revenue

## Action Items  
The additional program that should be considered are: <br>
<b> 1. Loyalty Program: </b> Providing vouchers and product recommendations for old customers who have not shopped in a certain range to return to shopping <br>
<b> 2. Customer Experience via Catalog and Website shopping: </b> Optimizing product recommendations based on most buy and offering up-selling and cross-selling <br>
<b> 3. Vouchers for minimum spent: </b> vouchers / discounts that can be used for a limited period so that customers return to shopping
 
 # Contributors
 
 - Dhiaz Raflianza as Project Supervisor
 - Aminudin as Project Leader
 - Muchammad Malik
 - Muhammad Afif Hibban
 - Muhammad Nafiul Ahkam
 - Ramadhani Yovita Hapsari
 - Suci Rahmadiani
 - Suci Share Putri
