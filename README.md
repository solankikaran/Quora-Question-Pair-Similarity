# Quora Question Pair Similarity
## Problem Statement
- Given questions on Quora, determine if they're duplicates of one another.
- This could be useful to quickly provide answers for questions which have already been answered
- Task is to predict if two questions are duplicates or not
## Business Objectives and Constraints
- Cost of misclassification is high
- Using probability (of pair of questions being duplicate) as a measure will be nice so that we can choose a threshold of choice.
## Data Overview
1. train.csv contains 5 columns: </br>
- qid1 - id of question 1 </br>
- qid2 - id of question 2 </br>
- question1 - english text of question 1 </br>
- question2 - english text of question 2 </br>
- is_duplicate - target column which indicates whether pair of questions are similar or not
## Type of Machine Learning Problem
- It is a binary classification problem. Given a pair of questions, we need to predict if they are duplicate or not.
## Performance Metric
- Log-loss (Primary KPI)
- Confusion Matrix
