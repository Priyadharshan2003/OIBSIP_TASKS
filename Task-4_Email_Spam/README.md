# TASK-4 EMAIL SPAM PREDICTION 

## 1.First, import the required libraries:

### pandas: for reading and manipulating the csv file containing the email data.
### numpy: for creating arrays that will store the email class and message data.
### CountVectorizer: for converting the text data into a matrix of token counts.
### train_test_split: for splitting the data into training and testing sets.
### MultinomialNB: for implementing the Naive Bayes algorithm.

##  2.Read the CSV file containing the email data using the pandas read_csv() method. The file path is given as an argument to the method, along with the encoding type to be used (in this case, 'latin-1').

## 3.Use the head() method to display the first 5 rows of the data to verify that it has been read correctly.

## 4.Select only the "class" and "message" columns from the data using data[["class", "message"]]. This will create a new DataFrame with only these two columns.

## 5.Convert the "class" and "message" columns into numpy arrays using np.array() and store them in the variables x and y respectively.

## 6.Create an instance of the CountVectorizer class called cv.

## 7.Use the fit_transform() method of the CountVectorizer object to fit and transform the "class" data into a matrix of token counts called X.

## 8.Split the data into training and testing sets using the train_test_split() method. Here, the data is split into 67% training data and 33% testing data. The random_state argument is set to 42 to ensure that the split is always the same, which makes the results reproducible.

## 9.Create an instance of the MultinomialNB class called clf.

## 10.Use the fit() method of the MultinomialNB object to train the model on the training data.

## 11.Ask the user to enter a message using the input() function and store it in a variable called sample.

## 12.Use the transform() method of the CountVectorizer object to convert the user input message into a matrix of token counts called data.

## 13.Use the predict() method of the MultinomialNB object to predict whether the user input message is spam or not. This is done by passing the data matrix as an argument to the predict() method.

## 14.Print the predicted class label to the console using the print() function.

## That's it! The code reads in email data from a CSV file, trains a spam detector model using the Naive Bayes algorithm, and makes predictions on user input messages.
