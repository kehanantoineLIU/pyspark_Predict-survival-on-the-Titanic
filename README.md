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

 ## Data preprocessing
1. Use a VectorAssembler to put features into a feature vector column
2. Standardization
 ## Building Classification Model
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
 
