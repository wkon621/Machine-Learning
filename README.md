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
I decided to use Root Mean Square Error to measure the success of my model given this is a regression problem with a numerical dependent variable. The established baseline model is based off "difference from average revenue". The baseline model has a RMSE just a little bit less than 1 million, indicating it does not have the ability to predict revenue from unseen movie dataset. 

| Model  | RMSE |
| ------------- | ------------- |
| Baseline  | 993408.070  |
| Linear Regression  | 2.427  |
| Decision Tree  | 3.252  |
| Gradient Boosting  | 0.013  |
| neural Network  | 2.182  |

After comparing the performance of each model, I predicted the revenue from the test dataset using the saved model, and saved the predictions as CSV file. Moreover, I also predicted the movie revenue with a smiple nerual networks with 2 layers but the RMSE is far behind the graident boosting model. As the last step, I wanted to know which features play the most important role in prediciting movie revenue. budget, popularity, runtime, and cast counts play the most important role in the model.

## Conclusion
To sum up, I  developed a model that predicts movie revenue based on different features. After performing the exploratory data analysis, I created a baseline model, fitted three models, and outputed their root mean squared errors for comparsion against one another. The best performing model is the gradient boosting model. I saved the best model, and predicted the revenue of test data with it. The results of the prediction and feature importance are all saved in csv file.Future iterations of this analysis may incorporate more features, such as imdb score, rotten tomatoes, and whether the copyright has been bought by foreign studios. 


## Data set
This is a dataset from Kaggle and you can find both the train and test data in the zip file 


Thank you

