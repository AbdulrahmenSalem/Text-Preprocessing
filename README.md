# Text-Preprocessing
The provided code consists of a Python class called TextPreprocessing, which has several methods for text data cleaning, vectorization, Naive Bayes modeling, and transformation of data


# Clean(self, df): 
This method takes a DataFrame as an input, makes a deep copy of it, and cleans the text data in all columns of the DataFrame. The cleaning process involves removing unwanted characters, URLs, and numbers, lowercasing, lemmatizing, and removing stop words. The cleaned DataFrame is returned.



# Vactorization(self, df, target_name) : 
This method takes a DataFrame and a target column name as inputs, creates a copy of the DataFrame, and performs vectorization of the text data using the pos_freq and neg_freq dictionaries generated by the Vactorize method. It returns a new DataFrame where each text column is replaced with two new columns representing the frequency of positive and negative words.

# fit_transform(self, df, target_name) : 
This method takes a DataFrame and a target column name as inputs, performs data cleaning and vectorization using the Clean and Vactorization methods, and returns the transformed DataFrame.

# Naive_Bayes(self, df, target_name): 
This method takes a DataFrame and a target column name as inputs, performs data cleaning and vectorization using the Clean and Vactorize methods, and applies Naive Bayes algorithm to predict the target variable. It returns the predicted target variable for the input DataFrame.
