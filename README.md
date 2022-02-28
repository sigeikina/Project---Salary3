# Salary Prediction Project

### 1. Purpose

Salary is related to many factors. The goal of this project is to create a model that predicts a IT salary in EU depending on factors such as:

- age,
- gender,
- city,
- position,
- years of experience,
- main technology (occupation).

### 2. Data

The dataset for this Project is a CSV file used from Kaggle website (https://www.kaggle.com/parulpandey/2020-it-salary-survey-for-eu-region). The dataset provides information about IT salary in a different cities of Europe Union in 2020. CSV file has 23 columns and 1253 rows.

### 3. Libraries

For this Project I have used Python Pandas library to read csv data, I have used Pandas read_csv function to read the csv file. I have also imported other libraries such as Numpy (for performing mathematical functions), Matplotlib (for visualisation purpose), Seaborn (an additional visualisation tool).

To predict the salary, I have used Linear Regression model, which shows the relationship between the amount of salary and factors such as age, gender, city, position, years of experience, main technology.

Linear regression is a model that assumes a linear relationship between an explanatory variable (X) and a response variable (y). The model can predict value of y based on value of X. In this Linear Regression model the estimated salary is response variable (y) and the factors such as age, gender, city, position, years of experience, main technology are explanatory variable (X).

Prior to building Linear Regression model I have imported Scikit-learn library and used train_test_split function to split data into a training and test set (X_train, X_test, y_train, y_test = train_test_split(X, Y)). The training set is used to train the model whereas the test set is used assess the performance of the trained model in prediction the result.

### 4. Conclusion

Based on the Linear Regression model, I can conclude that IT salary grows with age and years of experience for both male and females. However, females' salary is lower even if the age, years of experience or other factors are the same.
