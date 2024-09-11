# ds_module_20_supervised_learning

In this assignment we fitted a logistic regression model to a dataset to train and evaluate a model based on loan risk. Our dataset included historical lending activity from a peer-to-peer lending services company. 

The purpose of our analysis was to use our model to identify the creditworthiness of borrowers.

Here is a break down of the results of our model:

To evaluate how well our model predicted both loan labels, we can look at the metrics in our classification report:

Precision: This indicates the accuracy of positive predictions. Our value of 1 for healthy loans indicates perfect accuracy for this class. .86 for our high-risk loans means that 86% of predicted high-risk loans were actually high-risk. There are some false positives.

Recall: This measures how well the model identifies actual positive cases. .99 indicates that 99% of the actual healthy loans were correctly identified by the model. There were very few false negatives. The model correctly identified 94% of the actual high-risk loans, indicating a strong ability to detect high-risk loans.
    
F1-Score: This is the harmonic mean of precision and recall, providing a balance between the two. The F1-score being 1.00 reflects a perfect balance between precision and recall for this class. The F1-score of 0.90 shows a good balance between precision and recall for this class, although it's not as high as for the healthy loans.

Support: We clearly have imbalanced classification in that we have many more observations to train our model for healthy loans & not enough to gain a high level of confidence in our high-risk loans. 

Conclusion: The logistic regression model performs exceptionally well in predicting healthy loans, with perfect precision and a very high recall. For high-risk loans, while the precision is slightly lower, the recall remains high, indicating that the model is effective in identifying most high-risk loans. Overall, the model shows strong performance across both classes, but due to imbalanced classification, we lose confidence in our models ability to be used to determine high-risk laons.