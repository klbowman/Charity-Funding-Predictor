# Predicting Charity Funding

TensorFlow neural network model to predict the success of funding for charitable organizations. 

## Overview

Alphabet Soup is a fictional non-profit foundation that has funded more than 34,000 organizations. Data from each organization, such as government classification, industry type, amount of funding requested and effectiveness of the funding, is included in the **chartiy_data.csv** file located in the **Resources** directory.   

The **nnModel.ipynb** file is used to import, clean, and process the data before employing a TensorFlow neural network model to predict if the money from each organization was used effectively (i.e., the organization was successful). The neural network model in this file has 2 hidden layers and 100 epochs, and produces a model loss of 0.57 and accuracy score of 0.73. The model is exported to the **AlphabetSoupCharity.h5** file. The **AlphabetSoupCharity_Optimization.ipynb** file is used to improve the accuracy score of the neural network model.

## Results
* Data Preprocessing
  * Target variable: **IS_SUCCESSFUL** (Yes indicates that the organization used the money effectively)
  * Features: affiliation, classification, use case, organization type, status, income amount, special considerations, ask amount.
  * Identification columns were removed from the dataset during preprocessing.
* Compiling, Training, and Evaluating the Model
 * The most accurate model tested in this repository had 43 input features, two hidden layers (the first layer had 80 neurons, and the second layer had 30 neurons), and used ReLu and Sigmoid activation functions.
 * Target model performance (Accuracy = 0.75) was achieved.
 * Other efforts to improve model performance include binning the ASK_AMT column into 10 groups, and adjusting the number of neurons in each hidden layer. These efforts did not increase the accuracy score above 0.75. 

## Summary
Keras tuner was used to find the best model parameters, increasing the accuracy score to 0.76. The best model hyperparameters include a ReLu activation function, 11 input units, and 4 layers with 11, 6, 6, 26, and 21 neurons, respectively.


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
