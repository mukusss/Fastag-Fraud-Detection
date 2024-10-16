**Fastag Fraud Detection **
**Overview**
This project is focused on developing a machine learning-based system to detect fraudulent transactions within the Fastag electronic toll collection system. Fastag uses electronic tags attached to vehicles, allowing automatic toll payments as they pass through toll booths. The project leverages advanced machine learning techniques to enhance the security and integrity of digital toll payments, ensuring timely identification of suspicious activities.
**Table of Contents**
Project Overview
Dataset Description
Technologies Used
Project Workflow
Results
How to Run
Future Enhancements
Contributing
License
**Project Overview**
The objective of this project is to build a robust fraud detection model that accurately identifies fraudulent transactions based on historical data of Fastag transactions. Fraudulent activities can disrupt the toll collection system, and this machine learning model helps in early detection and prevention of such incidents.

**Dataset Description**
The dataset used for this project consists of various features related to Fastag transactions, including:
**Transaction_ID:** Unique identifier for each transaction.
**Timestamp:** Date and time of the transaction.
**Vehicle_Type:** Type of vehicle involved in the transaction.
**FastagID:** Unique identifier linked to each vehicle's Fastag.
**TollBoothID:** Identifier for the toll booth.
**Lane_Type:** Type of lane used for the transaction.
**Vehicle_Dimensions:** Dimensions of the vehicle.
**Transaction_Amount:** Amount of money involved in the transaction.
**Geographical_Location:** Location details of the transaction.
**Vehicle_Speed:** Speed of the vehicle during the transaction.
**Fraud_indicator:** Binary indicator (0/1) representing whether the transaction was flagged as fraudulent or not (target variable).

**Technologies Used**
**Programming Language:** Python
**Libraries:**
 ** Data Analysis:** pandas, numpy
 ** Data Visualization:** matplotlib, seaborn
 ** Machine Learning:** scikit-learn
 ** Model Evaluation:** Classification report, confusion matrix, accuracy, precision, recall, F1 score.

**Project Workflow**
**Data Preprocessing:**
Handled missing values through imputation methods.
Categorical variables (e.g., vehicle type, lane type) were converted into numerical form using encoding techniques.

**Data Balancing:**
The dataset had an unequal distribution of fraudulent and non-fraudulent transactions. This imbalance was addressed using resampling techniques to ensure the model could effectively detect fraud.

**Modeling:**
  **Logistic Regression:** Used as a baseline classifier.
 ** Random Forest Classifier:** To improve accuracy and handle complex patterns in the data.
  **Gradient Boosting Classifier:** Applied to capture subtle patterns that may indicate fraudulent activities.

**Model Evaluation:**
Evaluated model performance using key metrics like accuracy, precision, recall, and F1 score.
Created a confusion matrix to visualize the classification results.

**Visualization:**
Plotted the distribution of transactions and the performance of different models for a better understanding of results.

**Results**
The final fraud detection model achieved a high level of accuracy and effectively balanced precision and recall, ensuring minimal false positives and false negatives.
Visualizations such as heatmaps, bar charts, and confusion matrices were used to present the model's performance and the distribution of fraudulent vs non-fraudulent transactions.

**Future Enhancements**
  **Feature Engineering:** Exploring additional features, such as the vehicle’s past transaction history or additional geographical data, could further enhance fraud detection accuracy.
  **Real-Time Fraud Detection:** Integrating the model into a real-time detection system that flags suspicious transactions as they occur.
 ** Deployment:** Deploy the model using Flask or Django to create a web interface for monitoring fraud detection results.
