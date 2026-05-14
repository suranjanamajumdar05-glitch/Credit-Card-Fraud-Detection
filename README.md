# Credit Card Fraud Detection using Machine Learning
## Project Overview
Credit card fraud has become one of the major challenges in the financial sector. Fraudulent transactions cause significant financial losses to banks and customers. This project focuses on detecting fraudulent credit card transactions using Machine Learning algorithms.
The dataset used in this project is highly imbalanced, containing very few fraud transactions compared to genuine transactions. To solve this issue, SMOTE (Synthetic Minority Oversampling Technique) has been used for balancing the dataset.
The project includes:
- Data preprocessing
- Exploratory Data Analysis (EDA)
- Data balancing using SMOTE
- Machine Learning model training
- Model evaluation
- Graphical visualization of results

# Objectives
- Detect fraudulent credit card transactions accurately
- Handle imbalanced transaction data
- Compare multiple machine learning models
- Improve fraud detection performance using SMOTE
- Analyze transaction patterns through visualization

# Dataset Description
The dataset contains transactions made by European credit card holders.
### Dataset Information
1.  Time - Time elapsed between transactions
2.  Amount - Transaction amount
3.  V1-V28 - PCA transformed confidential features
4.  Class - Target variable (0 = Genuine, 1 = Fraud)
### Dataset Statistics
- Total Transactions: 284,807
- Fraud Transactions: 492
- Genuine Transactions: 284,315

The dataset is highly imbalanced.

# Technologies Used
## Programming Language
- Python
## Libraries Used
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Imbalanced-learn (SMOTE)
## Tools Used
- VS Code
- Jupyter Notebook

# Project Workflow
## Step 1: Data Collection
The dataset is loaded and inspected.
## Step 2: Data Preprocessing
- Missing value checking
- Feature scaling
- Dropping unnecessary columns
## Step 3: Exploratory Data Analysis
Visual analysis of transaction patterns and fraud distribution.
## Step 4: Handling Imbalanced Data
SMOTE is applied to balance fraud and non-fraud transactions.
## Step 5: Model Training
Multiple Machine Learning models are trained.
## Step 6: Model Evaluation
Models are evaluated using different performance metrics.

# Machine Learning Models Used
## 1. Logistic Regression
Used as a baseline classification model.
## 2. Decision Tree Classifier
Used for rule-based classification.
## 3. Random Forest Classifier
Used for improved accuracy and fraud detection performance.

# Evaluation Metrics
The following metrics are used to evaluate model performance:
1. Accuracy - Overall correctness
2. Precision - Correct fraud predictions
3. Recall - Ability to detect fraud
4. F1 Score - Balance of precision and recall
5. ROC-AUC Score - Classification performance

# SMOTE Technique
SMOTE (Synthetic Minority Oversampling Technique) is used to balance the highly imbalanced dataset by generating synthetic fraud samples.
### Benefits of SMOTE
- Improves fraud detection
- Prevents model bias
- Improves Recall and F1 Score

# Graphical Visualizations
## 1. Fraud vs Non-Fraud Transaction Distribution
This graph shows the imbalance between genuine and fraudulent transactions.
<img width="750" height="558" alt="image" src="https://github.com/user-attachments/assets/7ad85ea6-71d0-43e7-9f6c-361d39345580" />

## 2. Correlation Heatmap
The heatmap shows correlations between different transaction features.
<img width="1502" height="1259" alt="image" src="https://github.com/user-attachments/assets/be647c40-cd33-46b4-b9ca-0197b3668121" />

## 3. Transaction Amount Distribution
This graph shows the distribution of transaction amounts.
<img width="877" height="468" alt="image" src="https://github.com/user-attachments/assets/7e9a2a50-9442-4bd7-8f3f-21d844083580" />

## 4. Confusion Matrix
The confusion matrix visualizes correct and incorrect predictions made by the Random Forest model.
<img width="537" height="433" alt="image" src="https://github.com/user-attachments/assets/efae0f7b-c936-4286-b3e8-8843599a7377" />

## 5. Feature Importance Graph
This graph displays the top important features used by the Random Forest model for fraud detection.
<img width="855" height="545" alt="image" src="https://github.com/user-attachments/assets/46e90a5a-c160-4045-a905-e47fe7fc158e" />

# Model Performance Comparison
Model                   Accuracy   Precision  Recall    F1 Score  ROC AUC
1. Logistic Regression  0.948904   0.974374   0.922266  0.947604  0.948957
2. Decision Tree        0.998408   0.997756   0.999070  0.998413  0.998407
3. Random Forest        0.989114   0.997839   0.980395  0.989040  0.989132

# Conclusion
This project demonstrates how Machine Learning can be effectively used for detecting fraudulent credit card transactions. By handling imbalanced data using SMOTE and applying classification algorithms, the system achieves efficient fraud detection performance.
Random Forest provided the best performance among all models used in this project.
