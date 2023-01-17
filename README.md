# Ensemble-technique-Quora-question-pair-similarities
# Abstract

Quora is more of a general-purpose Q and A platform.The repetition of questions is one of the issues that Quora has. The experience is ruined when a question is asked again, by both the questioner and the answerer. We can simply show the questioner the responses to the earlier question since it is a duplicate question. Additionally, for questions that are almost identical, the respondent may not repeat their response.
For instance there are certain questions as, "How can I become a doctor?" and "What should I do to become a doctor?".It is clear that both queries ask the same question. Although the questions are phrased differently, they both have the same objectives. Therefore, the answers to both questions will be the same. Therefore, we just need to display the responses to the first query. In this method, the person asking the question will receive the responses right away, and those who have already responded to the first question won't have to say it again.
Currently, Quora uses a Random Forest model to identify duplicate questions. By applying advanced techniques may be we can make it easier to find high quality answers to questions resulting in an improved experience for Quora writers, seekers, and readers.I have utilised machine learning models XGBoost, Linear SVM, Logistic Regression, Random Forest to handle this issue in this project. The error log loss functions of the machine learning approaches mentioned above were examined and contrasted and features extraction from the provided dataset using a variety of natural language processing (NLP) techniques, but there are undoubtedly more ways to enhance the performance of this model by using deep learning-based techniques, which will be the focus of my future work.
# Problem Statement
Determine whether Quora questions are duplicates of other questions that have already been posted.To provide prompt responses to questions that have already been addressed.
# Objective 
Our objective is to determine whether a set of questions contains duplicates or not.

# Data Over view [train.csv]

•	Class labels: 0, 1 
•	Total training data / No. of rows: 404290 
•	No. of columns: 6 
•	Dependent variable: is_duplicate 
•	No. of non-duplicate data points is 255027 
•	No. of duplicate data points is 149263 
1.	Exploratory Data Analysis: I started by performing exploratory data analysis on the "train.csv" data. This involved tasks like counting the amount of unique questions, looking for duplicates, counting the frequency of questions, and more. 
2.	Feature extraction: Executed feature extraction techniques such as the fuzz ratio, fuzz partial ratio, common word share, etc.
3.	Word2Vec Features Tokenizer: Apply Word2Vec Features to a dataset of two questions, and then combined each Word2Vec Feature with our Advanced Feature Set and Basic Feature Set. 
4.	TFIDF Weighted W2V vectorizer: Will be applying on a pair of questions dataset, which was then combined with our advanced feature set and basic feature set.
5.	Visualisation approaches: After doing feature extraction I apply several visualisation techniques.
6.	Machine learning algorithm: I use Machine learning algorithm such as logistic regression, Linear SVM and XGBoost Algorithm and try to discover best log-loss Score for both train and test dataset.
7.	Model development and evaluation: Using a confusion matrix, we compare the performance of several models once they have been trained.
8.	Model deployment: The chosen model is deployed in the environment using the Streamlit user interface.

