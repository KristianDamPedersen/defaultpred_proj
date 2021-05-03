# Predicting defaults on loans
The purpose of this project is to predict whether or not a loan applicant will defualt on their loan. It will output this both in a "yes or no" fashion, as well as a percentage chance. Hopefully this will help a bank screen applicants in a more efficient manner.

## Results

## Data
The dataset i'll be using is the "Loan Default Prediction" dataset from Kamal Das, uploaded to Kaggle.com
https://www.kaggle.com/kmldas/loan-default-prediction

## Key overview of each step
### Big picture decisions
#### Problem
Predicting whether or not an applicant will default on their loan
#### General model
Firstly, since we're working with labeled data, we will use a supervised model. Also since this is a dichotoumous outcome (yes or no), a logistic regression will be used as a baseline. Other models might be included to compare performances. Lastly, because our dataset is relatively manageable and we dont need to adjust to changes rapidly, we'll be using a plain old batch learning approach.
#### Performance measure
Performance measure will be the *accuracy* (percent/proportion of cases classified correctly) as well as *sensitivity* (The percent or proportion of 1s correctly classified, in this case the amount of correctly predicted defaults).
### Exploratory data analysis
### Data cleaning
### Modelbuilding 
### Productionization

## Problems and fixes
1. Trouble fitting multiple seaborn plots into matplotlib subplots, solution found at:
https://dev.to/thalesbruno/subplotting-with-matplotlib-and-seaborn-5ei8

2. Trouble creating a new variable column, that creates a ratio between income and bank balance. Solution found at: 
https://stackoverflow.com/questions/38032817/dividing-one-dataframe-column-by-another-division-by-zero/46942969

3. Ran into problems limiting decimal places when creating income_balance_ratio predictor. Solution found at:
https://stackoverflow.com/questions/54509060/limiting-the-number-of-decimal-places-in-python-pandas-table

4. Why i chose to recode high income_balance_ratios
https://www.tiaa.org/public/learn/personal-finance-101/how-much-of-my-income-should-i-save-every-month

5. A larger than i would admit amount of time was spent creating the distribution over income_balance_ratio between defaulted and non-defaulted individuals. The solution ended up being the "stat" argument from seaborns documentation. Can be found at:
https://seaborn.pydata.org/tutorial/distributions.html

