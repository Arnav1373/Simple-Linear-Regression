#Simple Linear Regression Project
Modelling the linear relationship between head size and brain weight of different users.
       

# The contents of this project are divided into following topics which are listed as follows:-

## Table of Contents
1. Introduction
2. Linear Regression
3. Independent and dependent variable
4. Simple Linear Regression (SLR)
5. About the dataset
6. Exploratory data analysis
7. Mechanics of Simple Linear Regression
8. Regression metrics for model performance i. RMSE ii. R2 Score
9. References
       

## 1. Introduction
In this project, I build a Simple Linear Regression model to predict the relationship between the head size and the brain weight of different users. I discuss the basics of linear regression and its implementation in Python programming language using Scikit-learn. Scikit-learn is the popular machine learning library of Python programming language.

       

## 2. Linear Regression
Linear Regression is a statistical technique which is used to find the linear relationship between dependent and one or more independent variables. This technique is applicable for Supervised Learning Regression problems where we try to predict a continuous variable. Linear Regression can be further classified into two types – Simple and Multiple Linear Regression.

       

## 3. Independent and Dependent Variables
In this project, I refer Independent variable as Feature variable and Dependent variable as Target variable. These variables are also recognized by different names as follows: -

Independent variable
Independent variable is also called Input variable and is denoted by X. In practical applications, independent variable is also called Feature variable or Predictor variable. We can denote it as: - Independent or Input variable (X) = Feature variable = Predictor variable

Dependent variable
Dependent variable is also called Output variable and is denoted by y. Dependent variable is also called Target variable or Response variable. It can be denote it as follows: -

Dependent or Output variable (y) = Target variable = Response variable

       

## 4. Simple Linear Regression (SLR)
Simple Linear Regression (or SLR) is the simplest model in machine learning. It models the linear relationship between the independent and dependent variables.

In this project, there is one independent or input variable which is denoted by X. Similarly, there is one dependent or output variable which is denoted by y. We want to build a linear relationship between these variables. This linear relationship can be modelled by mathematical equation of the form:-

			Y = c   + m*X    -------------   (1)
In this equation, X and Y are called independent and dependent variables respectively, m is the coefficient for independent variable and c is the constant term. m and c are called parameters of the model.

For simplicity, we can compare the above equation with the basic line equation of the form:-

    			y = ax + b       ----------------- (2)
We can see that

slope of the line is given by, a = m, and

intercept of the line by b = c.

In this Simple Linear Regression model, we want to fit a line which estimates the linear relationship between X and Y. So, the question of fitting reduces to estimating the parameters of the model m and c.

## 5. About the dataset
The data set has been imported from the econometrics website with the following url-

https://www.kaggle.com/datasets/jemishdonda/headbrain

This data set contains Sales and Advertising expenditures for a dietary weight control product. It contains monthly data for 36 months. The variables in this data set are Sales and Advertising.

       

## 6. Exploratory data analysis
First, I import the dataset into the dataframe with the standard read_csv () function of pandas library and assign it to the df variable. Then, I conducted exploratory data analysis to get a feel for the data. I checked the dimensions of dataframe with the shape attribute of the dataframe. I viewed the top 5 rows of the dataframe with the pandas head() method. I viewed the dataframe summary with the pandas info() method and descriptive statistics with the describe() method.

       

## 7. Mechanics of Simple Linear Regression
The mechanics of Simple Linear Regression model starts with splitting the dataset into two sets – the training set and the test set. We instantiate the regressor lm and fit it on the training set with the fit method. In this step, the model learned the correlations between the training data (X_train, y_train). Now the model is ready to make predictions on the test data (X_test). Hence, I predict on the test data using the predict method.

       

## 8. Regression metrics for model performance
Now, it is the time to evaluate model performance. For regression problems, there are two ways to compute the model performance. They are RMSE (Root Mean Square Error) and R-Squared Value. These are explained below:-

i. RMSE
RMSE is the standard deviation of the residuals. So, RMSE gives us the standard deviation of the unexplained variance by the model. It can be calculated by taking square root of Mean Squared Error. RMSE is an absolute measure of fit. It gives us how spread the residuals are, given by the standard deviation of the residuals. The more concentrated the data is around the regression line, the lower the residuals and hence lower the standard deviation of residuals. It results in lower values of RMSE. So, lower values of RMSE indicate better fit of data.

ii. R2 Score
R2 Score is another metric to evaluate performance of a regression model. It is also called coefficient of determination. It gives us an idea of goodness of fit for the linear regression models. It indicates the percentage of variance that is explained by the model. Mathematically,

R2 Score = Explained Variation/Total Variation

In general, the higher the R2 Score value, the better the model fits the data. Usually, its value ranges from 0 to 1. So, we want its value to be as close to 1. Its value can become negative if our model is wrong.

       

## 9. References
The concepts and ideas in this project have been taken from the following websites and books:-

i. Machine learning notes by Andrew Ng

ii. https://en.wikipedia.org/wiki/Linear_regression

iii.https://en.wikipedia.org/wiki/Simple_linear_regression

iv https://en.wikipedia.org/wiki/Ordinary_least_squares

v. https://en.wikipedia.org/wiki/Root-mean-square_deviation

vi. https://en.wikipedia.org/wiki/Coefficient_of_determination

vii https://www.statisticssolutions.com/assumptions-of-linear-regression/

viii.Python Data Science Handbook by Jake VanderPlas

ix. Hands-On Machine Learning with Scikit Learn and Tensorflow by Aurilien Geron

x. Introduction to Machine Learning with Python by Andreas C Muller and Sarah Guido
