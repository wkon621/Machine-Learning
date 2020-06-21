# Movie-Revenue-Prediction

Predicting movie revenue using Linear Regression, Random Forest, Gradient Boosting and Neural Network.


## Introduction
What are some important factors that make a newly debuted movie profitable? Is it simply based on the budget, cast, languages, or its more complicated than that? I would like to investigate this question using existing movie data and its associated revenue with the first movie dates back to 1930. After exploring the data, I will develop a model and plot which features are the most important in determining movie revenue of newly premier movie. The language of this data science project problem is Python, using packages such as pandas, numpy, matplotlib, seaborn, and sklearn.

## Data Preprocessing 
This is a dataset that requires a lot of preprocessing. A lot of the features are json type string objects composed of list of dictionaries. I preprocessed most of these features into categorical varaible. For example, a datapoint with a link in its homepage varaible will be transformed to binary feature (1 as with hompage 0 as without homepage). 

## Exploratory Data Analysis

It is not a surprise that average movie reveneu is positively correlated with year. Recently released movie has higher revenue; however, one could factor in inflation, buying power for further consideration. 

After exploring the categorical variables and their relationships to the revenue variable, I took a closer look at numerical variables. Firstly, I was curious about the distribution of the dependent variable- revenue. I transformed the revenue variable with log becasue the original does not follow a normal distribution. 

Based on the correlation matrix, budget does have a strong correlation with revenue while runtime has a weak positive correlation with revenue.

## Modeling
I decided to use Root Mean Square Error to measure the success of my model given this is a regression problem with a numerical dependent variable. The established baseline model is based off "difference from average revenue"

| Model  | RMSE |
| ------------- | ------------- |
| Content Cell  | Content Cell  |
| Content Cell  | Content Cell  |
| Content Cell  | Content Cell  |
| Content Cell  | Content Cell  |

## Data set
This is a dataset from Kaggle and you can find both the train and test data in the zip file 



Thank you

