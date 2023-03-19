# TASK-5-SALES_PREDICTION 

## Let's go through the code step by step:

## 1.The first few lines import the necessary libraries such as pandas, numpy, matplotlib, seaborn, sklearn's train_test_split and LinearRegression.
## 2.The next line reads a CSV file "Advertising.csv" and stores it in a pandas dataframe called "data". The file contains information about advertising spendings on different media platforms and corresponding sales numbers.
## 3.The third line prints the first five rows of the dataframe using the head() method.
## 4.The fourth line checks if there are any missing values in the dataframe using the isnull() method and summing up the null values. Since there are no missing values, the output shows all columns with zero null values.
## 5.The next few lines create a heatmap using seaborn's heatmap() function to visualize the correlation between different features (TV, Radio, Newspaper) and the target variable (Sales).
## 6.Then, the independent and dependent variables are defined. The independent variable "x" contains all the columns except "Sales" and is stored as a numpy array. The dependent variable "y" contains only the "Sales" column and is also stored as a numpy array.
## 7.Next, the data is split into training and testing sets using the train_test_split() function from sklearn. 20% of the data is used for testing and 80% for training. The random_state argument is set to 42 to ensure the same split occurs every time the code is run.
## 8.The Linear Regression model is instantiated and then fit on the training data using the fit() method.
## 9.The predict() method is used to generate predictions on the testing data.

## Finally, the predicted sales are stored in a new pandas dataframe called "data" and printed to the console.

## In summary, this code reads data from a CSV file, creates a heatmap to visualize the correlation between features and target variable, trains a Linear Regression model on the training data, and then generates predictions on the testing data. The predicted sales are stored in a pandas dataframe and printed to the console.
