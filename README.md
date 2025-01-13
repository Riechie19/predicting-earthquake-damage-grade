# Predicting the 2015 Gorkha Earthquake Damage Grade Using Machine Learning Techniques
The ability to predict damages caused by earthquakes is important as an accurate damage grade 
prediction can help in identifying buildings that are at risk of collapsing, allowing appropriate 
safety measures to be implemented. This paper aims to use various machine learning based 
methods to predict the damage grade of the 2015 Gorkha earthquake scaling from 1 to 3. Data used 
in this paper will be the given training and testing data that are based on actual post-disaster 
datasets from Nepal. Accuracy of the machine learning model will be based on the obtained F1 
score. 

In our data pre-processing approach, we addressed potential outliers, checked for missing or 
duplicated values, and performed feature selection based on our understanding of the problem. We 
experimented with both label encoding and one-hot encoding for categorical data, with results 
compared subsequently. Additionally, data scaling was implemented using the MinMaxScaler 
technique to normalize feature values between 0 and 1. 

We tested various machine learning models suitable for classification tasks, including 
**Random Forest (RF)**, **K Nearest Neighbors (KNN)**, **AdaBoost**, and **LightGBM**. Each model 
was trained on four types of datasets: label-encoded original, one-hot encoded original, label
encoded with feature selection, and one-hot encoded with feature selection. A comparison of 16 
different F1 scores derived from these models was conducted. 

Our findings indicate that LightGBM outperforms other models in terms of F1 score. 
Specifically, the label-encoded original dataset yielded the best results for the LightGBM model. 
We hypothesize that this higher performance is due to each feature's significant contribution to 
predicting damage grade and the ordinal nature of the categorical features, making label encoding 
the more appropriate choice for this dataset. These results are thoroughly documented in this [paper](https://drive.google.com/file/d/1ISDvR6NVuFnQZDTDmHZFmWBJ7J_CU98I/view?usp=sharing).
