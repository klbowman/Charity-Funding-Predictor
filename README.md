# Predicting Charity Funding

TensorFlow neural network model to predict the success of funding for charitable organizations. 

## Description

Alphabet Soup is a fictional non-profit foundation that has funded more than 34,000 organizations. Data from each organization, such as government classification, industry type, amount of funding requested and effectiveness of the funding, is included in the **chartiy_data.csv** file located in the **Resources** directory.   

LendingClub is a peer-to-peer lending services company that allows individual investors to partially fund personal loans as well as buy and sell notes backing the loans on a secondary market. LendingClub offers their previous data through an API. Data from 2019 & 2020 is used in this repository to create machine learning models **(Logistic Regression model and Random Forest Classifier)** that predict the credit risk of loans from the first quarter of 2020.

The **Resources** directory contains two CSV files of data used to train and test the models. The GenerateData.ipynb file in the **Generate** directory is used to download data from LendingClub and output two CSV files that are undersampled, to give an even number of high risk and low risk loans. In the original dataset, only 2.2% of loans are categorized as high risk. To get a truly accurate model, special techniques need to be used on imbalanced data. Undersampling is one of those techniques.

Models are trained and tested in the Credit Risk Evaluator.ipynb Jupyter Notebook file. The pd.get_dummies() function is used to convert categorical data to numeric columns in test and train datasets. Logistic regression and random forest classifier models are fitted with scaled and unscaled data for comparison. With scaled data, the logistic regression models scores higher in predicting credit risk. 

## Getting Started

### Technologies Used 

* Jupyter Notebook
* Pandas 
* Scikit-learn 

### Installing

* Clone this repository to your desktop.
* To generate new data, navigate to the Generator directory and run GenerateData.ipynb.
* To build models, navigate to the home directory and run Credit Risk Evaluator.ipynb.

### Data Sources

* LendingClub (2019-2020) Loan Stats. Retrieved from: https://resources.lendingclub.com/

## Author

Katlin Bowman, PhD

E: klbowman@ucsc.edu

[LinkedIn](https://www.linkedin.com/in/katlin-bowman/)