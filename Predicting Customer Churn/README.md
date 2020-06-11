# Predicting-Customer-Churn

Dataset description :

The dataset I am using is derived from **IBM Sample Datasets.**

Context of the dataset- It has columns about customer's demographic information, different types of services they are availing from the telecom company in question and customer churn(that is whether or not the customer leaves). This data is relevant to one whole month and our target variable is churn=1 (Yes) meaning the customer left the company

So, on the basis of information contained in the predictor variables, our goal is to identify customers who may tend to leave in order to focus on customer retention programs

Metric used for evaluating models- **Recall score**

Explanation: _Since this is a customer churn prediction problem, we cannot afford to lose customers by classifying True Positives as Negatives- that is we need to minimise the number of False Negatives(customers who will leave (churn=1) but are classified as customers who won't leave(churn=0)). That is why I used recall, since it focusses on minimising False Negatives._

NOTE: False Positives won't cost the company as large as a leaving customer would. On the other hand, it benefit the company only since it will keep it's service-quality up to the mark for a sample that was falsely classified as positive.

Best model based on recall score: **Cost Sensitive Random Forest Classifier**

Recall score: 0.78

Test accuracy: 0.72

NOTE: Best model based on test accuracy is cost sensitive logistic regression model with accuracy=0.81 and recall=0.51
