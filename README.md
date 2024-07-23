# Credit-Card-Fraud-Anomaly

Reflection on Credit Card Fraud Detection Project
Project Goal: Develop a machine learning model using historical credit card transaction data to predict whether future transactions are legitimate or fraudulent.
Source: Kaggle Credit Card Fraud Dataset


## Project Overview

In this project, I aimed to build a machine learning model to detect fraudulent credit card transactions. My approach involved:

- **Data Preparation:** I handled an imbalanced dataset by creating a balanced sample with equal numbers of normal and fraudulent transactions.
- **Feature and Target Variable Separation:** I split the dataset into independent variables (features) and the target variable (fraud or not fraud).
- **Model Training:** I used logistic regression as the classifier and faced some challenges related to the convergence of the algorithm.
- **Evaluation:** I assessed the model's performance using accuracy metrics on both training and test datasets.


## Results

- **Accuracy on Training Data**: 94.92%

- **Accuracy on Test Data:** 91.88%


## Reflection

**1. Model Performance:**

- **Training Accuracy (94.92%):** The high accuracy on the training data indicates that the model fits the training set well. This is expected as the model was tuned and trained specifically on this data.
- **Test Accuracy (91.88%):** The model performs slightly worse on the test data compared to the training data. This drop is normal and indicates that the model is generalizing well to unseen data, although there might still be room for improvement.
  

**2. Data Handling:**

- **Balancing the Dataset:** By creating a balanced dataset, I addressed the class imbalance issue, which is crucial for fraud detection. Imbalance can lead to models that are biased towards the majority class (non-fraudulent transactions).
- **Stratified Splitting:** Ensuring that both training and test sets have proportional representations of both classes helped maintain the integrity of the model evaluation.


**3. Model Convergence:**

- The convergence warning highlighted the need for tuning hyperparameters and potentially scaling the data. Increasing the number of iterations and scaling the data helped resolve this issue and likely contributed to better model performance.

**4. Accuracy Metrics:**

- Accuracy is a good starting point but can be misleading in imbalanced datasets. In practice, other metrics such as Precision, Recall, F1-Score, and ROC-AUC should be considered, especially for fraud detection where false negatives (missed frauds) are costly.

**5. Next Steps:**

- **Hyperparameter Tuning:** Experimenting with different models and hyperparameters could further improve performance. Trying algorithms like Random Forests, Gradient Boosting, or Neural Networks might yield better results.
- **Feature Engineering:** Investigating additional features or refining existing ones could provide more information to the model and enhance its predictive power.
- **Evaluation Metrics:** Incorporating additional metrics, such as precision, recall, and the F1 score, would provide a more comprehensive assessment of the model's performance in detecting fraudulent transactions.

## Conclusion

The project successfully demonstrated the ability to create a robust model for detecting fraudulent credit card transactions. While the model performs well with high accuracy, continuous improvements and evaluations are necessary to handle real-world scenarios effectively. Addressing class imbalance, exploring advanced algorithms, and refining feature engineering will be key to achieving even better performance.
