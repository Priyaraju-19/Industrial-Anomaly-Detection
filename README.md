# Industrial-Anomaly-Detection
# Industrial Anomaly Detection Project

## Overview
The Industrial Anomaly Detection project aims to develop a system capable of identifying unusual behavior in industrial equipment data. By detecting anomalies early, this system can help prevent equipment failure, reduce downtime, and improve operational efficiency. This README provides an overview of the project, including its primary goal, specific tasks, execution workflow, and other relevant details.

## Primary Goal
The primary goal of this project is to develop an anomaly detection system for industrial equipment. The system's objective is to identify deviations from normal equipment behavior using sensor data and prevent equipment failure, reduce downtime, and improve operational efficiency.

## Specific Tasks
1. **Data Generation/Preprocessing**: Generate synthetic data or preprocess real sensor data to simulate industrial equipment behavior. This involves handling missing values, noise reduction, and data scaling.
2. **Anomaly Detection Model**: Develop an anomaly detection model capable of identifying deviations from normal equipment behavior. Common techniques include statistical methods and machine learning algorithms.
3. **Model Evaluation**: Assess the performance of the anomaly detection model using appropriate evaluation metrics such as precision, recall, F1-score, and ROC curves.
4. **Visualization & Reporting**: Visualize the results of the anomaly detection system and create reports to provide insights into unusual behavior patterns.

## Execution Workflow
1. **Data Preprocessing**: 
   - Load sensor data from a CSV file.
   - Perform Moving Average Smoothing technique to reduce noise in the data.
   - Preprocess the data by handling missing values, removing outliers using Interquartile Range (IQR), and converting timestamps to appropriate formats.
   - Perform one-hot encoding for categorical variables.

2. **Model Training and Evaluation**:
   - Split the data into training and testing sets.
   - Use Synthetic Minority Over-sampling Technique (SMOTE) to handle class imbalance.
   - Train an Isolation Forest model using GridSearchCV to find the best hyperparameters.
   - Evaluate the model's performance using ROC AUC score and other relevant metrics.

3. **Visualization and Reporting**:
   - Visualize the results of anomaly detection using appropriate plots such as ROC curves.
   - Create a report summarizing the findings, including insights into unusual behavior patterns and recommendations for action.

## Others
- **Libraries Used**: numpy, pandas, matplotlib, seaborn, scikit-learn, imbalanced-learn.
- **Model Selection**: Isolation Forest was chosen due to its effectiveness in detecting anomalies in high-dimensional data and its ability to handle class imbalance.
- **Data Augmentation**: SMOTE was used to handle class imbalance by oversampling the minority class.
- **Hyperparameter Tuning**: GridSearchCV was employed to tune the hyperparameters of the Isolation Forest model.
- **Model Evaluation**: ROC AUC score was chosen as the primary evaluation metric to assess the model's ability to distinguish between normal and anomalous behavior.

## Conclusion
The Industrial Anomaly Detection project provides a systematic approach to develop an anomaly detection system for industrial equipment. By leveraging machine learning techniques and appropriate evaluation metrics, the system can effectively identify unusual behavior patterns, enabling timely intervention to prevent equipment failure and improve operational efficiency.
