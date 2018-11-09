# Machine-learning-on-unbalanced-dataset

## Problem Statement:
In this analysis, I intend to explore some of the data augmentation techniques applied to unbalanced classification problem. The problem consists of three classes (60.2% Type0, 26.2% Type1 and 13.5% Type2). The goal of the analysis is to learn how data augmentation techniques work on this problem, explore whether it always helps to classify instances accurately and how to avoid some of the conceptual pitfalls while applying machine learning on unbalanced datasets.


## Methodology:
Starting with exploratory data analysis by summary statistics and visualization, some of the data preprocessing techniques such as handling missing data and standardizing dataset was also applied. The various cases that were tested are as follows:
1) Unbalanced dataset (Base case)
2) Resampling minority classes
3) Synthetic Minority Oversampling Technique (SMOTE)
4) Downsampling majority with resampling minority
5) Cross validation before resampling
6) Cross validation before applying SMOTE

The following machine learning algorithm were tested:
1) Random Forest
2) Support Vector Machines
3) Logistic Regression


## Results and Conclusion:
- As seen in this analysis, different data augmentation techniques were tried alongside different machine learning algorithms.
- The main purpose of this analysis was not to portray the best data augmentation technique or the best performing machine learning algorithm on unbalanced dataset. Rather, I wanted to follow fundamentally strong and conceptually profound techniques which would give me a deeper insight into how the data augmentation techniques works in combination with some of the best machine learning algorithms.
- That goal is certainly achieved as it was seen that any data augmentation technique (resampling minority, SMOTE, downsampling + SMOTE) can still overfit our training data.
- The problem of overfitting was then resolved by creating a custom function which would cross validate first before applying the various data augmentation techniques.
- Although this does not single out a machine learning algorithm but it significantly reduces the overfitting.
- Conclusively, through this analysis I discovered how data augmentation techniques work and how to best use them with machine learning algorithm and overcome the common pitfalls that one might fall into, if they are not careful while applying these techniques.
