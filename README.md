# pyspark_Predict-survival-on-the-Titanic
the aim of this projrt is to use pyspark predict survival on the Titanic
## data analyse
we use heatmap and stastic analyse to choose the variable we can use
![image](https://github.com/kehanantoineLIU/pyspark_Predict-survival-on-the-Titanic/assets/125217787/9a454a91-a773-426f-9fd6-9598a5445544)
 |-- Pclass:  Ticket class   
 |-- Sex: Sex of passenger    
 |-- SibSp: siblings / spouses aboard the Titanic   
 |-- Parch: parents / children aboard the Titanic   
 |-- Fare:  Passenger fare  
 |-- Embarked: Port of Embarkation

## Pipeline
 Pipeline = Transformer + Estimator
 ## Data preprocessing(Transformer)
1. Use a VectorAssembler to put features into a feature vector column
2. Standardization
## Estimator
1. RandomForestClassifier
2. LogisticRegression
3. GBTClassifier

## Evaluation
1. BinaryClassificationEvaluator => calculate Accuracy
2. MulticlassClassificationEvaluator => calculate Precision & Recall
 ### 1. Logistic Regression
 Accuracy: 0.8077984817115254   
 Precision: 0.7868224123991876   
 Recall: 0.7884615384615385
 ### 2. Random Forest
 Accuracy: 0.8519355041094174   
 Precision: 0.7922956824596169   
 Recall: 0.7923076923076924
 ### 3. Gradient-Boosted Trees (GBT)
 Accuracy: 0.8389171215258171   
 Precision: 0.7823265491904545   
 Recall: 0.7846153846153846
### conclude
Accuracy: The Random Forest model has the highest accuracy of 0.852.

Precision: Random Forest and Logistic Regression have relatively high precision, both around 0.79, which means that a significant percentage of all samples predicted to survive did survive.

Recall: The recall of all models is close.

In this task, I think the most important thing is the recall of the models, because we are more concerned with the models correctly identifying survivors. But the recall of all the models is close, all I choose Random Forest as my final model here

