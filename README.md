# COVID-19_Severity_Prediction
predict the severity of COVID-19 based on the symptoms

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

```
File Name: COVID_ver3.ipynb
Data: covid_sym.csv
```

### Prerequisites

```
Python 3
```

### Installing Packages

```
Pandas
Numpy
Matplotlib.pyplot
Sklearn  

```

## Running the codes

```
Run each section in the file named COVID_ver3.ipynb in the COVID folder. 
Each section in the notebook is labelled, and there are comments explaining the code.
```

### Break down into end to end tests


First we read in the data and do exploratory data analysis to understand the data better. We looked at the missing values as the proportions of variables. Next, we did pre-processing in order to transform the severity levels into a binary variable. Then we begin building a logistic regression model and identify the feature importance of a severe case. After that we built a random forest model, and then compared multiple algorithms' accuracy scores in order to determine the best one. We then use clustering as a supervised model to identify the number of clusters, which is two that represent the target variable. Then we compare the true label and clustered label to calculate the accuracy. After seeing that Random Forest had the highest accuracy score, we tuned that model by altering the hyperparameters with the goal of improving the model. We evaluated the model with the best hyperparameters and then graphed the AUC curve and calculated the score. Lastly, we used the random forest predictive model to predict the severity level of 5 new patients and got the results.


The best model is `Random Foreser Classifier`

The scores are\
`accuracy`: 0.88\
`recall`: 0.9\
`precision`: 0.9\
`F1-score`: 0.9

## Authors

* **Eric Wu** 
* **Elisabeth Webb**
* **Ben DeLeon**
* **Calix Carrington**

## License

This project is licensed under the LMU MSBA program

## Summary

The goal of this project was to use what we have learned in our machine learning class to answer a predictive question about Coronavirus. Our question was to predict an incoming Coronavirus patient's severity based on their symptoms. We answered this question by building a random forest model that was able to predict a patient's severity with 87% accuracy. We also found the characteristics that contribute most to critical and deceased cases using logistic regression.
