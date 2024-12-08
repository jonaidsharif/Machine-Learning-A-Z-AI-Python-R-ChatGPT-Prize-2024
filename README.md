# For Python learners, summary of Object-oriented programming: classes & objects

Please find below a clear explanation of what these concepts are:

A class is the model, or a blueprint, of something we want to build. For example, if we make a house construction plan that gathers the instructions on how to build a house, then this construction plan is the class.

An object is an instance of the class. So if we take that same example of the house construction plan, then an object is simply a house. A house (the object) that was built by following the instructions of the construction plan (the class).
And therefore there can be many objects of the same class, because we can build many houses from the construction plan.

A method is a tool we can use on the object to complete a specific action. So in this same example, a tool can be to open the main door of the house if a guest is coming. A method can also be seen as a function that is applied onto the object, takes some inputs (that were defined in the class) and returns some output.


## Coding Exercise 1: Importing and Preprocessing a Dataset for Machine Learning
In this exercise, you will explore data preprocessing with Python.

Instructions:



Import the necessary Python libraries: You will need the pandas library for this exercise. Also import numpy and train_test_split from sklearn.model_selection.

Load the Iris dataset: The Iris dataset is stored in a CSV file named 'iris.csv'. Use the pandas function read_csv to load this file and store it in a DataFrame. Assign the DataFrame to a variable named dataset.

Identify the features and the dependent variable: The features (independent variables) in the Iris dataset are the lengths and widths of the petals and sepals, and the dependent variable is the species of the Iris. The features are stored in all columns except the last one in your DataFrame, and the dependent variable is stored in the last column.

Create the matrix of features (X) and the dependent variable vector (y): Use the iloc indexer in pandas to select these subsets of the data and store them in variables X and y respectively. You should use the .values attribute to extract the data as numpy arrays.

Print X and y: Finally, print the matrix of features (X) and the dependent variable vector (y) to verify their creation. You can use the print function for this.




## Coding Exercise 2: Handling Missing Data in a Dataset for Machine Learning
1. Import the necessary Python libraries for data preprocessing, including the `SimpleImputer` class from the scikit-learn library.

2. Load the dataset into a pandas DataFrame using the `read_csv` function from the pandas library. The dataset name is 'pima-indians-diabetes.csv'

3. Identify missing data in your dataset. Print out the number of missing entries in each column. Analyze its potential impact on machine learning model training. This step is crucial as missing data can lead to inaccurate and misleading results.

4. Implement a strategy for handling missing data, which is to replace it with the mean value, based on the nature of your dataset. Other strategies might include dropping the rows or columns with missing data, or replacing the missing data with a median or a constant value.

5. Configure an instance of the `SimpleImputer` class to replace missing values with the mean value of the column.

6. Apply the `fit` method of the `SimpleImputer` class on the numerical columns of your matrix of features.

7. Use the `transform` method of the `SimpleImputer` class to replace missing data in the specified numerical columns.

8. Update the matrix of features by assigning the result of the `transform` method to the correct columns.

9. Print your updated matrix of features to verify the success of the missing data replacement.

