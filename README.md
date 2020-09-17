# Predicting Wine Quality

This aim of this project was to accurately predict the quality of a range of different red wines based upon their chemical features. I completed this project to practice the skills and techniques I had learned after completing Jose Portilla's "Python for Data Science Bootcamp" course on [Udemy](https://www.udemy.com/course/python-for-data-science-and-machine-learning-bootcamp/learn/lecture/17739846?start=0). I was able to produce a range of models for the two questions asked within this project, with the best performing model obtaining 85% accuracy on the test set used.

## Table of Contents

* [Technologies](#technologies)
* [Exploratory Data Analysis](#exploratory_data_analysis)
* [Data Preprocessing and Model Building](#data_preprocessing_and_model_building)
* [Model Performance](#model_performance)

## Technologies

This project was created using a Jupyter Notebook with the following package versions installed:

* Python: 3.7.7
* Imbalanced-Learn: 0.7.0
* Numpy: 1.19.1
* Pandas: 1.1.0
* Seaborn: 0.10.1
* Scikit-Learn: 0.23.1
* Matplotlib: 3.2.2

## Exploratory Data Analysis

Each of the 11 independent variables within the dataset was analysed against the target variable. I analysed the correlations amongst the indenpendant variables. Below are some of the highlights from the EDA.

![alt text](https://github.com/sykes14596/Red_Wine_Quality/blob/master/Images/Correlation_Matrix.png "Correlation Matrix")
![alt text](https://github.com/sykes14596/Red_Wine_Quality/blob/master/Images/target_variable_countplot.png "Target Variable Countplot")
![alt text](https://github.com/sykes14596/Red_Wine_Quality/blob/master/Images/Correlation_to_target_variable.png "Correlation to Target Variable")

## Data Preprocessing and Model Building

Some variables were removed from the dataset in order to minimise the risk of multicolinearity. Due to the extremely unbalanced dataset, two different problems were solved. First, models were created to determine whether a wine was "good", which equated to having a rating of at least 6, or "bad", equating to having a rating of at most 5. This converted the problem into a binary classification problem. 

Second, the SMOTE technique was used to created synthetic instances of each of the minority classes in order to achieve a perferctly balanced dataset. This lead to the problem becoming a multiclass classification problem. 

In each problem type, I created 5 different models to practice producing the necessary code required to implement them. The models implemented were:

* Logistic Regression,
* Decision Tree,
* Random Forest,
* Support Vector Machines,
* XGBoost.

