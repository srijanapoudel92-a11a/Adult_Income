Adult Income Classification
1. Dataset and Problem

This project uses the Adult/Census Income dataset. It contains information about people, such as age, education, job, and working hours.

The main goal is to predict whether a person's income is ≤50K or >50K.

2. What I Did

I loaded the dataset using Pandas and used EDA to understand the data, find missing values, check duplicates, and see how income is distributed.

I cleaned the data by replacing ? with missing values, filling missing categorical values, and removing duplicate rows and rows with missing income.

3. Feature Engineering

I created new features to help the models learn from the data:

Net capital: Calculates the difference between capital gain and capital loss.

Age group: Divides people into different age groups.

Working-hour group: Divides people based on their weekly working hours.

4. Preprocessing

The dataset has both numbers and text, so I prepared the data for the models using:

One-Hot Encoding: Changes text data into numbers.

StandardScaler: Scales numerical data.

I used a Pipeline to combine these steps with the models.

5. Model Training and Evaluation

I trained and compared three machine-learning models:

Logistic Regression

Decision Tree

Random Forest

I divided the data into 80% training data and 20% testing data. I also used five-fold cross-validation to check model performance.

I compared the models using accuracy, precision, recall, and F1 score. I used a classification report and confusion matrix to check the selected model's results.

6. Model Saving

I selected the model with the highest F1 score and saved it using Joblib. Then, I loaded the saved model and tested it on sample data.

7. Key Findings

The dataset contains both numbers and text, so data preprocessing is important.

More people in the dataset earn ≤50K than >50K.

The three models gave different results.

The confusion matrix helped me see how many income predictions were correct and incorrect.
