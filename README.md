Financial Fraud Prevention : A Machine Learning- Based Risk Analysis System

Credit card fraud is a critical financial issue that requires effective detection mechanisms to minimize losses. This project utilizes machine learning techniques, specifically logistic regression, to classify fraudulent and legitimate transactions using the **Credit Card Fraud Detection** dataset.  

**Dataset Overview**  
The dataset contains credit card transactions, with features representing different aspects of the transaction, such as time, amount, and various anonymized numerical values obtained through PCA transformation. The key target variable, Class, indicates whether a transaction is fraudulent (1) or legitimate (0).  

**Data Preprocessing**  
1. **Loading the Dataset**: The dataset is imported into a Pandas DataFrame, and exploratory analysis is conducted to understand its structure, missing values, and class distribution.  
2. **Class Imbalance Handling**: Since fraudulent transactions are significantly fewer than legitimate ones, a random undersampling technique is applied. A subset of legitimate transactions (equal to the number of fraudulent ones) is selected to create a balanced dataset.  
3. **Feature Selection**: The Class column is separated from the features to form X (independent variables) and Y (target variable).  

**Model Training & Evaluation**  
1. Splitting Data: The dataset is split into training (80%) and testing (20%) sets using stratified sampling to maintain class proportions.  
2. Logistic Regression: A logistic regression model is trained to distinguish fraudulent transactions from legitimate ones.  
3. Performance Metrics: The model achieves an accuracy of 94.9% on training data and 91.8% on test data.  

**Conclusion**  
The logistic regression model demonstrates high accuracy in detecting fraudulent transactions. However, given the imbalanced nature of real-world fraud detection datasets, additional techniques such as SMOTE (Synthetic Minority Over-sampling Technique) or more complex models like Random Forests or Neural Networks could be explored for improved performance.  

