Customer Churn Prediction Using Random Forest

### Project Overview
This project uses Machine Learning to predict whether a customer is likely to leave a telecommunications company. It uses the Random Forest Classifier to learn patterns from customer information such as tenure, contract type, monthly charges, and subscribed services.

The goal is to help businesses identify customers who may leave and take steps to improve customer retention.

### Objectives
- Analyze customer data using Exploratory Data Analysis (EDA).
- Clean missing and inconsistent values.
- Convert categorical data into numerical features.
- Train a Random Forest classification model.
- Evaluate model performance using accuracy, precision, recall, F1-score, and a confusion matrix.

### Technologies Used
- Python
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

### Dataset
Dataset: IBM Telco Customer Churn

Source: Download from Kaggle

The dataset contains customer information, including tenure, monthly charges, contract details, services, and churn status.
- No — the customer stayed.
- Yes — the customer left.
The dataset used in this project contained 7,032 customer records after cleaning.

### Project Workflow
1. Data Loading: Loaded the dataset using Pandas.
2. Data Cleaning: Converted TotalCharges to numeric values and handled missing values.
3. EDA: Examined the distribution of customers who stayed and left.
4. Feature Preparation: Separated the input features (X) from the target (y).
5. Train-Test Split: Used an 80:20 split for training and testing.
6. Encoding: Converted categorical variables using OneHotEncoder.
7. Model Training: Trained a Random Forest Classifier with 100 decision trees.
8. Evaluation: Measured accuracy and reviewed the classification report and confusion matrix.

### Model Performance
The model achieved the following results on the test dataset:

Metric	                    Result
Accuracy	                78.89%
Precision — Churn	        63%
Recall — Churn	            50% 
F1-score — Churn         	56%

### Confusion Matrix
[[922 111]
 [186 188]]


	            Predicted: Stayed	    Predicted: Left          
Actual: Stayed	922	                    111
Actual: Left	186	                    188

Result analysis: The model correctly identified 188 customers who left. However, it missed 186 customers who actually left. Improving churn recall is an important opportunity for future development.

### Project Structure
Customer-Churn-Prediction/
│
├── Customer Prediction_Random_Forest.ipynb
├── README.md
└── NEW-Telco-Customer-Churn.csv



### How to Run the Project
Step 1: Clone or download this repository.

Step 2: Install the required libraries.
pip install pandas matplotlib seaborn scikit-learn jupyter


Step 3: Place the CSV dataset in the project folder.

Step 4: Open Jupyter Notebook.
jupyter notebook


Step 5: Open Customer_Churn_Prediction_Random_Forest.ipynb and run the notebook cells in order.

### Future Improvements
- Improve recall for customers likely to leave.
- Tune Random Forest hyperparameters.
- Compare Random Forest with Logistic Regression and other classifiers.
- Analyze feature importance to understand factors associated with churn.
- Build a simple web application to demonstrate predictions.

### Key Learnings
Through this project, I practiced:
- Data preprocessing and cleaning
- Exploratory Data Analysis
- Categorical feature encoding
- Supervised Machine Learning
- Random Forest classification
- Model evaluation and confusion matrix interpretation

### Conclusion
This project demonstrates an end-to-end beginner-level Machine Learning workflow for customer churn prediction. The Random Forest model achieved 78.89% accuracy, providing a baseline for further experimentation and improvement.