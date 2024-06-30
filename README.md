# 🏢Employee Turnover Prediction

## Introduction
This project aims to predict employee turnover within a company by analyzing various factors related to their work and satisfaction. The goal is to understand the key contributors to employee turnover and devise strategies to retain employees.

## Objectives
- Perform data quality checks.
- Conduct exploratory data analysis (EDA) to identify factors contributing to employee turnover.
- Cluster employees who left the company based on their satisfaction and evaluation.
- Handle class imbalance using the SMOTE technique.
- Train and evaluate models using k-fold cross-validation.
- Identify the best model and justify the evaluation metrics used.
- Suggest retention strategies for targeted employees.

## Dataset Description
The dataset contains the following columns:

| Column Name            | Description                                                 |
|------------------------|-------------------------------------------------------------|
| satisfaction_level     | Satisfaction level at the job of an employee                |
| last_evaluation        | Rating between 0 to 1, received by an employee at last evaluation |
| number_project         | Number of projects an employee is involved in               |
| average_monthly_hours  | Average number of hours in a month, spent by an employee at office |
| time_spend_company     | Number of years spent in the company                        |
| Work_accident          | 0 - no accident during employee stay, 1 - accident during employee stay |
| left                   | 0 indicates employee stays in the company, 1 indicates employee left the company |
| promotion_last_5years  | Number of promotions in the last 5 years                    |
| Department             | Department an employee belongs to                           |
| salary                 | Salary in USD                                               |

## Methodology
### Data Preparation
1. **Import Libraries and Load Dataset**:
   - Import necessary Python libraries such as pandas, seaborn, matplotlib, sklearn, and imbalanced-learn.
   - Load the dataset into a pandas DataFrame.

2. **Data Quality Check**:
   - Check for missing values and handle them appropriately.

### Exploratory Data Analysis (EDA)
1. **Understand Factors Contributing to Employee Turnover**:
   - Analyze various features to identify patterns and relationships with employee turnover.
   - Use visualizations to support the analysis.

### Clustering
1. **KMeans Clustering**:
   - Perform clustering on employees who left based on their satisfaction level and last evaluation.

### Handle Class Imbalance
1. **SMOTE Technique**:
   - Use SMOTE (Synthetic Minority Over-sampling Technique) to handle class imbalance in the dataset.

### Model Training and Evaluation
1. **K-Fold Cross-Validation**:
   - Train Logistic Regression, Random Forest Classifier and Gradient Boosting Classifier models using k-fold cross-validation and evaluate their performance.

2. **Model Evaluation**:
   - Identify the best model based on evaluation metrics.
   - Plot ROC curve and find ROC/AUC and confusion matrix for each model.

### Retention Strategies
1. **Categorize Employees**:
   - Categorize employees into four zones (safe, low risk, medium risk, high risk) based on their likelihood of leaving.
   - Suggesting retention strategies for each zone.

## Folder Structure
- `data/`: Contains the dataset files.
- `notebooks/`: Jupyter notebooks for data analysis, clustering, and model evaluation.
- `src/`: Python scripts for data processing, clustering, and model training.
- `api/`: Api code (if any).
- `models/`: Trained models and saved results.
- `docs/`: Output files including visualizations, model evaluation metrics, and plots.

## Installation and Usage
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/MariahFerns/Employee-Turnover-Prediction.git
   cd Employee-Turnover-Prediction

2. Install the required libraries:
   ```bash
   pip install -r requirements.txt

3. Run Jupyter Notebooks:
   Navigate to the notebooks/ folder and open the notebooks to explore data analysis and model development.

## Results and Findings
**EDA Insights:**
- Identified key factors contributing to employee turnover, such as satisfaction level, last evaluation, and average monthly hours.
- Found significant patterns and relationships between features and employee turnover.

**Clustering:**
- Successfully clustered employees who left the company into distinct groups based on satisfaction and evaluation.
- Visualized clusters to understand different employee profiles.

**Model Evaluation:**
- Evaluated multiple models and identified the best performing model.
- Plotted ROC curves and confusion matrices to compare model performance.

**Retention Strategies:**
- Categorized employees into four risk zones (safe, low risk, medium risk, high risk) based on their likelihood of leaving.
- Suggested targeted retention strategies for each zone to reduce employee turnover.

## Conclusion
This project provided valuable insights into employee turnover by analyzing various factors and identifying key contributors. The findings can help the HR department devise effective retention strategies and improve employee satisfaction.

