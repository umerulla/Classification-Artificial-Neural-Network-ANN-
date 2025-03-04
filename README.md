# Classification-Artificial-Neural-Network-ANN-

Overview
This project aims to predict Customer Satisfaction (CSAT) scores for a leading e-commerce platform using deep learning techniques. By leveraging an Artificial Neural Network (ANN), the model provides actionable insights to help improve service quality and customer experience.

Key Features
Data Preprocessing:

Cleaned an 85K+ record dataset by addressing missing values (using mode, median, and mean imputation), outlier treatment, and dropping irrelevant columns.
Applied one-hot encoding for categorical variables to ensure the model receives robust numerical inputs.
Feature Engineering & Selection:

Engineered new features such as Response_Time_seconds, day numbers, and weekdays from order and survey dates to capture key customer interaction patterns.
Utilized Variance Inflation Factor (VIF) and correlation analysis to remove redundant features and ensure minimal multicollinearity.
Performed exponential transformations on skewed features to achieve a more Gaussian-like distribution.
Data Scaling & Balancing:

Standardized numerical features using StandardScaler.
Balanced the imbalanced dataset (approximately 85:15 ratio) using SMOTE, ensuring the model performs robustly across all satisfaction classes.
Model Development & Evaluation:

Built an ANN using TensorFlow and Keras, incorporating multiple Dense layers with Batch Normalization, Dropout (rate 0.5), and L2 regularization.
Employed 3-fold Stratified Cross-Validation with EarlyStopping and a custom LearningRateScheduler to optimize training.
Evaluated the model using precision, recall, F1-score, and ROC-AUC metrics—achieving a mean training accuracy of 77.9% and a mean test accuracy of 75.01%.
Installation & Usage
Installation:
Install the required packages by running:
bash
Copy
Edit
pip install tensorflow==2.17.1 keras-tuner==1.4.7 scikeras statsmodels imbalanced-learn
Usage:
Run the provided Jupyter Notebook or Python script to reproduce the preprocessing, model training, and evaluation steps.
Conclusion
This project demonstrates the effectiveness of deep learning for customer sentiment analysis on e-commerce data. The ANN model not only delivers robust predictive performance but also provides insights into critical factors influencing customer satisfaction, enabling data-driven decisions for enhancing customer retention and service quality.

