# Stock-Price-Sentiment-Analysis-using-News-Headlines

**Step 1: Data Acquisition and Preprocessing**

- Begin by obtaining the dataset. Our dataset has information on 4353 companies. The columns include the date, 25 news headlines for each company, and a binary label indicating stock price movement (1 for up, 0 for no change or down).

- Load the dataset into a Pandas DataFrame.

**Step 2: Exploratory Data Analysis**

- Preprocess the dataset, including cleaning and formatting. Ensure that date columns are in datetime format and that the text data is free of any inconsistencies.

- Perform EDA to get more insights into your dataset 
  
**Step 3: Text Preprocessing**

- For each set of news headlines related to a company, you may perform text preprocessing. This can include tokenization, removal of stopwords, and other text cleaning steps.
  
**Step 4: Feature Extraction (Bag of Words Model)**

- Utilize the Bag of Words (BoW) model to convert the processed text data into a numerical format that machine learning algorithms can understand.

- Create a BoW representation for each set of news headlines for each date. This involves creating a vocabulary of unique words from all headlines and representing each document as a vector of word counts.

**Step 5: Target Variable**

- The binary label indicating stock price movement serves as your target variable. This label will be used to train and evaluate the Random Forest classifier.

**Step 6: Data Splitting**

- Split the dataset into training and testing sets. Allocate a portion of the data for training (e.g., 80%) and the remaining portion for testing (e.g., 20%).

**Step 7: Building Random Forest Model**

- Define and create a Random Forest classifier. Random Forest is a suitable choice for binary classification tasks.

- Configure hyperparameters such as the number of trees in the forest, tree depth, and other relevant parameters using Hyper-parameter tuning.

**Step 8: Model Training**

- Train the Random Forest classifier using the training dataset, which consists of BoW representations of news headlines and corresponding binary labels (stock price movement).

**Step 9: Prediction**

- Use the trained Random Forest model to make predictions on new, unseen data. Provide the BoW representation of news headlines for a given date.

**Step 10: Model Evaluation**

- Evaluate the model's performance on the testing dataset to assess its ability to classify whether the stock price will go up or not.

- Use evaluation metrics such as accuracy, precision, recall, F1-score, and the confusion matrix to assess the model's performance.

**Step 11: Result Interpretation**

- Interpret the model's predictions for trading decisions. For example, if the model predicts a high likelihood of the stock price going up, it may suggest a buy signal, and vice versa.
