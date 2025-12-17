Spam Email Detection using ROC Curve Demo.

Description:

This demo implements a Spam Email Detection System using Roc Curve.
A Multinomial Naive Bayes classifier is trained on SMS data and evaluated using the ROC (Receiver Operating Characteristic) curve and AUC (Area Under Curve) score to measure how well the model distinguishes between spam and non-spam messages.

Aim:

To classify emails as Spam or Non-Spam (Ham) and evaluate the classifier’s performance using TPR and FPR plotted through an ROC curve.

Dataset

SMS Spam Collection Dataset

Source:
https://raw.githubusercontent.com/justmarkham/pycon-2016-tutorial/master/data/sms.tsv

Labels:

ham → 0

spam → 1

Naive Bayes Classifier:

Naive Bayes is a probabilistic machine learning algorithm based on Bayes’ Theorem.
It assumes that features are conditionally independent given the class label.

Why Naive Bayes for Spam Detection?

Works efficiently with text data

Fast training and prediction

Performs well even with high-dimensional data

Commonly used in email and SMS spam filtering

Multinomial Naive Bayes:

In this demo, Multinomial Naive Bayes is used because:

It is suitable for word frequency–based features

Works effectively with TF-IDF vectors

Technologies Used:

Python

Pandas

Scikit-learn

Matplotlib

NumPy

Workflow:

Load SMS dataset

Encode labels (ham/spam)

Split data (80% Training, 20% Testing)

Apply TF-IDF Vectorization

Train Multinomial Naive Bayes model

Evaluate using Accuracy, ROC Curve, and AUC

Model Evaluation:

Accuracy Score

ROC Curve

AUC (Area Under Curve)

ROC Curve Explanation:

TPR (True Positive Rate): Correctly detected spam messages

FPR (False Positive Rate): Ham messages incorrectly classified as spam

A curve above the diagonal line indicates better model performance

Results:

High accuracy on test data

ROC curve clearly above the random classifier line

Strong AUC score indicating effective spam detection

Conclusion:

The Naive Bayes classifier, combined with TF-IDF feature extraction, provides an efficient and accurate approach for spam email detection. ROC and AUC metrics confirm the model’s strong classification capability.
