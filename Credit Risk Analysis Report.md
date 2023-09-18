# Credit Risk Classification

## Description
This analysis employs a range of machine learning techniques to train and assess the effectiveness of Logistic Regression Models in determining the creditworthiness of borrowers. The models were trained using diverse methods, and their performances were compared to ascertain the superior model. The predictive variables in the model are designated as either 0 (indicating a healthy loan) or 1 (indicating a high-risk loan).

## Steps
During the model construction process, the dataset was partitioned into features and labels, further divided into training and testing sets.

Machine Learning Model 1 was constructed by initializing a logistic regression model, training it with the original training sets (X_train, y_train), fitting it to these training sets, and subsequently generating predictions.

Machine Learning Model 2 was created by resampling the original training data using the RandomOverSampler module. It involved initializing a logistic regression model, fitting the resampled training sets (X_resample, y_resample) to the model, and generating predictions.

Each model's performance was assessed using the balance accuracy score, the confusion matrix, as well as precision, recall, and f1-score metrics outlined in the classification report.


## Results
- **Machine Learning Model 1:**

Model 1, trained on the original data, yields an accuracy of 94.4% in predicting the two labels. The model excels at predicting healthy loans, boasting precision and recall scores of 1.00 for this category. However, its performance in predicting high-risk loans could be enhanced. The precision score for high-risk loans stands at 0.87, signifying that only 87% of actual high-risk loans were correctly predicted. The recall score for high-risk loans is 0.89, indicating that the model identified only 89% of all high-risk loans in the dataset.

- **Machine Learning Model 2:**

Model 2, trained on the resampled data, achieves an accuracy of 99.6% in predicting the two labels. The model demonstrates proficiency in predicting healthy loans, maintaining precision and recall scores of 1.00 for this category. The precision score for high-risk loans remains at 0.87, but the recall score has improved to 1.00, indicating that the model can now identify all high-risk loans in the dataset.

## Summary  
Based on the analysis, it is evident that Model 2 outperforms Model 1 in predicting high-risk loans and attains an overall higher accuracy in predicting both labels. Specifically, Model 2 achieves a relatively high precision in predicting high-risk loans while correctly identifying all high-risk loans in the dataset—a noteworthy performance in this context. Therefore, it is recommended to utilize Model 2 for identifying high-risk loans and achieving overall improved accuracy in label prediction.
