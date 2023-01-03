# NLP Project | Supervised Learning with Quora Dataset | By Josh Ho

## Project Objectives
1. Use a supervised machine learning model to predict the whether a question is a duplicate from a previously answered question
2. Deply NLP classification model using NLTK methods like tokenization, lammetization, and sklearn modules like TF-IDF, and several classifiers suitable for classification tasks

## EDA 
1. Number of Characters in Each Question
* Applicant income data was heavily right skewed, with the vast majority (500+) of applicants making $18000 or less dollars.

2. Number of  Words in Each Question
* Applicants who graduated from post-secondary education tend to make almost $2000 more on than applicants who do not.

3. Top Stopwords
* Sorts applicant incomes by the property they reside in, and whether they are married (yes or no) and self employed (yes or no).

4. Top Words
* Male applicants who graduated make more than males who have not graduated, and females in general. Whereas females in general make more than males who did not graduate.

## Process
1. Load Dataset
2. Data Exploration (EDA)
3. Data Cleaning (Imputing missing values, removing punctuation, tokenization, lammetization, removing numbers and special characters, dropping and renaming columns)
4. Data Preprocessing (Feature engineering, scaling numeric features)
5. Model Building (Setting up train and test sets, model predictions, model evaluation and scoring)

## Results/Demo
Used 4 different classifiers with engineered dataset, including:
- Logistic Regression
- K-Nearest Neighbor
- Multinomial Naive Bayes
- Random Forest

Used K-Folds cross validation and ROC AUC score to evaluate and measure models performance.

All 4 models train and test sets achieved a score of >70%, with random forest performing the most effectively.

Random Forest Results
- Train Score: 79.56%
- Test Score: 77.56%

## Challenges 
The largest challenge was cleaning the dataset, as it was considerably large (400000+ rows) with many different attributes. I had to explore the dataset in-depth and address special characters, digits, which method of normalization to use, and processing tokenization of the text. Ultimately ensuring that my data was cleaned consistently and effectively. Although the process was arduous and time-consuming, the result from an uncleaned, messy, and incosistent dataset to one that was clean, standardized, and ready to use for modeling was a great delight to see.

## Future Goals
Future goals would be to build a pipeline to optimize the entire process in use for future binary text classification tasks. This would also provide the ability to optimize several different models with Grid Search and see if I could improve the models ability to perform. Overall, this was a very fun and interesting project!