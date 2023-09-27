
# 📚 Letter Prediction

## Overview

This project focuses on building a Support Vector Machine (SVM) to recognize black-and-white rectangular pixel displays as one of the 26 capital letters in the English alphabet. The character images are derived from 20 different fonts, and each letter is randomly distorted to create a dataset of 20,000 unique stimuli.

These stimuli are converted into 16 primitive numerical attributes, including statistical moments and edge counts. These attributes are then scaled to integer values ranging from 0 to 15. The training process typically involves using the first 16,000 items to create a predictive model. Subsequently, this model is employed to categorize the remaining 4,000 items into their respective letter categories.


# 📊 Data Exploration

The dataset, which consists of 20,000 records, is loaded from a CSV file.
There are no missing values in the dataset.
The dataset primarily consists of integer data types.

# 📊 Data Statistics

Mean Values for attributes range from approximately 3 to 8.
Standard Deviations vary from about 1 to 2.7.
The dataset has a minimum value of 0 and a maximum value of 15 for all attributes.
The data is summarized in the form of percentiles, providing insights into attribute distribution.

# 🧾 Accuracy Measurement

The accuracy of the SVM model is calculated using the following formula:

Accuracy = (Number of Correct Predictions / Total Predictions) * 100

The accuracy of this model on the test dataset is approximately 97.45%.

# 🔀 Data Splitting

The dataset is divided into training and testing sets:

Training features (x_train): The first 16,000 records.
Testing features (x_test): The remaining 4,000 records.
Training labels (y_train): Corresponding letter labels for the training data.
Testing labels (y_test): Corresponding letter labels for the test data.

# 🧠 SVM Model

The SVM model is implemented with specific parameters:
Gamma (γ) value: 0.025 (controls the smoothness of the decision boundary).
Regularization term (C): 3 (controls the acceptance of error in testing data).
The model is trained using the training features and labels.

# 📈 Confusion Matrix

A confusion matrix is generated to assess the model's performance. It displays the true positive, true negative, false positive, and false negative values for each letter category.

# 🔥 Heatmap Visualization

The confusion matrix is visualized using a heatmap, providing a clear overview of the model's performance in categorizing the letters.

# 📊 Performance Metrics

Various performance metrics such as precision, recall, and F1-score can be derived from the confusion matrix to further evaluate the model's accuracy.
## 🔗 Links
[![portfolio](https://img.shields.io/badge/view_my_notebook-000?style=for-the-badge&logo=github&logoColor=white)](https://nbviewer.org/github/Harinivas44/Letter_Prediction/blob/main/SVM.ipynb)
