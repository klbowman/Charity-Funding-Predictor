# Predicting Charity Funding

TensorFlow neural network model to predict the success of funding for charitable organizations. 

## Overview

Alphabet Soup is a fictional non-profit foundation that has funded more than 34,000 organizations. Data from each organization, such as government classification, industry type, amount of funding requested and effectiveness of the funding, is included in the **chartiy_data.csv** file located in the **Resources** directory.   

The **nnModel.ipynb** file is used to import, clean, and process the data before employing a TensorFlow neural network model to predict if the money from each organization was used effectively (i.e., the organization was successful). The **AlphabetSoupCharity_Optimization.ipynb** file is used to optimize the neural network model to an accuracy score of 0.75.

## Results
* Data Preprocessing
  * **Target variable:** "IS_SUCCESSFUL" (Yes indicates that the organization used the money effectively)
  * **Features:** affiliation, classification, use case, organization type, status, income amount, special considerations, ask amount.
  * Identification columns were removed from the dataset during preprocessing.
* Compiling, Training, and Evaluating the Model
 * The most accurate model tested in this repository had 43 input features, two hidden layers (the first layer had 80 neurons, and the second layer had 30 neurons), and used ReLu and Sigmoid activation functions. The model is exported to the **AlphabetSoupCharity_Optimization.h5** file.
 * Target model performance (Accuracy = 0.75) was achieved.
 * Other efforts to improve model performance include binning the ASK_AMT column into 10 groups, and adjusting the number of neurons in each hidden layer. These efforts did not increase the accuracy score above 0.75. 

## Summary
Keras tuner was used to find the best model parameters, increasing the accuracy score to 0.76. The best model hyperparameters include a ReLu activation function, 11 input units, and 4 layers with 11, 6, 6, 26, and 21 neurons, respectively. This neural network model can predict, with 75% accuracy, if an organization requesting $5,000-$11,855 will use that money effectively. Reducing the number of features from 43 to 11, could increase the model's accuracy to 76%.  

## Getting Started

### Technologies Used 

* Jupyter Notebook
* Pandas 
* Scikit-learn
* TensorFlow 

### Installing

* Clone this repository to your desktop.
* To import and preprocess the data, and generate a neural network model, run the file **nnModel.ipynb** in Jupyter Notebook.
* To optimize the neural network model, run the **AlphabetSoupCharity_Optimization.ipynb** file in Jupyter Notebook.

## Author

Katlin Bowman, PhD

E: klbowman@ucsc.edu

[LinkedIn](https://www.linkedin.com/in/katlin-bowman/)
