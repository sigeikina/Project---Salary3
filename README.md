# Salary Prediction Project

http://127.0.0.1:5000/predict

### 1. Purpose

Salary is related to many factors. The goal of this project is to create a model that predicts a IT salary in EU depending on factors such as:

- age,
- gender,
- city,
- position,
- years of experience,
- main technology (occupation).

### 2. Data

The dataset for this Project is a CSV file obtained from Kaggle website (https://www.kaggle.com/parulpandey/2020-it-salary-survey-for-eu-region). The dataset provides information about IT salary in a different cities of Europe Union in 2020.

The original CSV file contains 23 columns and 1253 rows. Some columns have been renamed and cleaning has been completed to remove unnecessary columns and NaN values, dropping the number of columns from 23 to 8 and the number of rows from 1253 to 1091.

To understand better dataset, I have created some visualisations:

- Age bar chart shows that most people working in IT industry are between 27 to 34 years old.
- The box plot 'Age vs Seniority level' shows that people in a junior position are in their early 20, where is people in senior and leading position are over 30 years old (close to 40).
- Gender pie shows that in IT industry there are 87,5 % males and only 12 % are females.
- Bar chart ‘Gender vs Salary’ shows males salary is higher than females.
- Bar chart ‘City’ shows that the most popular city for IT specialist is Berlin.
- Bar chart ‘Position’ shows that 3 most popular position are Software Engineer, Backend Developer and Data Scientist.
- Bar chart ‘Position vs Salary’ shows that the highest salary is paid for Engineering Managers.
- Bar chart ‘Years of experience vs Salary’ shows that the highest salary is paid for people who have approximately from 10 up to 25 years of work experience.

### 3. Libraries

For this Project I have imported libraries such as Pandas, Numpy, Matplotlib, Seaborn.

To predict the salary, I have used Linear Regression model, which shows the relationship between the amount of salary and factors such as age, gender, city, position, years of experience, main technology.

Linear regression is a model that assumes a linear relationship between an explanatory variable (X) and a response variable (y). The model can predict value of y based on value of X. In this Linear Regression model the estimated salary is response variable (y) and the factors such as age, gender, city, position, years of experience, main technology are explanatory variable (X).

Prior to building Linear Regression model I have imported Scikit-learn library and used train_test_split function to split data into a training and test set (X_train, X_test, y_train, y_test = train_test_split(X, Y)). The training set is used to train the model whereas the test set is used assess the performance of the trained model in prediction the result.

### 4. Conclusion

Based on the Linear Regression model, I can conclude that IT salary grows with age and years of experience for both male and females. However, females' salary is lower even if the age, years of experience or other factors are the same as males.
