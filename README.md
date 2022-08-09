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

## Analysis
- Distribution of duplicate and non-duplicate questions
![1](https://user-images.githubusercontent.com/44356744/183634452-369b570b-e314-4e4f-8d9e-93afbbbd6f68.png)

- Distribution of number of times a question was asked  
![2](https://user-images.githubusercontent.com/44356744/183634446-4e7d2853-cc14-4165-9a32-0262df0656f1.png)
