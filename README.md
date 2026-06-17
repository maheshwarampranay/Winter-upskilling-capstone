# Winter Upskilling Capstone: HR Analytics Project

## 📋 Overview

This repository contains a comprehensive data science capstone project focused on analyzing employee data and building predictive models to help the HR department of **Salifort Motors** improve employee retention and satisfaction.

The project applies data-driven insights to address critical HR challenges: understanding why employees leave the company and predicting which employees are at risk of departure.

## 🎯 Project Objectives

The primary goals of this capstone project are to:

1. **Analyze** employee data collected by the HR department
2. **Identify** key factors contributing to employee turnover
3. **Build predictive models** to forecast which employees are likely to leave
4. **Provide actionable insights** to reduce employee attrition and improve retention strategies

By predicting employees likely to quit, the organization can:
- Identify factors that contribute to employee departures
- Implement targeted retention strategies
- Reduce the time-consuming and expensive process of recruiting and hiring new employees

## 📊 Dataset

The HR capstone dataset contains **14,999 employee records** with **10 features**:

| Feature | Description | Type |
|---------|-------------|------|
| `satisfaction_level` | Employee-reported job satisfaction level [0–1] | Float |
| `last_evaluation` | Score of employee's last performance review [0–1] | Float |
| `number_project` | Number of projects employee contributes to | Integer |
| `average_monthly_hours` | Average number of hours employee worked per month | Integer |
| `tenure` | How long the employee has been with the company (years) | Integer |
| `work_accident` | Whether or not the employee experienced an accident while at work | Binary |
| `left` | Whether or not the employee left the company | Binary (Target) |
| `promotion_last_5years` | Whether or not the employee was promoted in the last 5 years | Binary |
| `department` | The employee's department | Categorical |
| `salary` | The employee's salary level | Categorical |

**Data Source:** [Kaggle HR Analytics Dataset](https://www.kaggle.com/datasets/mfaisalqureshi/hr-analytics)

### Key Statistics

- **Total Records:** 14,999 employees
- **Employee Churn Rate:** ~23.8% (employees who left)
- **Missing Values:** None
- **Duplicate Records:** 3,008

## 📁 Project Structure

```
Winter-upskilling-capstone/
├── README.md                                          # Project documentation
├── Activity_Course_7_Salifort_Motors_project_lab.ipynb # Main analysis notebook
├── HR_capstone_dataset.csv                            # Employee dataset
└── (Additional analysis files as project develops)
```

## 🔍 Project Methodology

### PACE Framework

This project follows the **PACE Strategy** framework, which consists of four stages:

1. **Plan** - Define the business problem and objectives
2. **Analyze** - Explore and understand the data
3. **Construct** - Build and train predictive models
4. **Execute** - Evaluate models and present findings

### Key Analysis Steps

#### 1. **Data Exploration & Cleaning**
   - Load and inspect the dataset
   - Standardize column names to snake_case
   - Check for missing values and duplicates
   - Analyze data types and distributions

#### 2. **Exploratory Data Analysis (EDA)**
   - Understand variable relationships
   - Identify patterns and outliers
   - Analyze churn patterns by department, salary, and other factors

#### 3. **Feature Engineering**
   - Create meaningful features from existing variables
   - Handle categorical variables
   - Normalize/scale numerical features

#### 4. **Predictive Modeling**
   - Build classification models to predict employee turnover
   - Models may include:
     - Logistic Regression
     - Decision Trees
     - Random Forests
     - Gradient Boosting

#### 5. **Model Evaluation**
   - Evaluate using appropriate metrics (accuracy, precision, recall, F1-score, ROC-AUC)
   - Interpret feature importance
   - Provide business recommendations

## 📈 Key Insights (Preliminary)

Initial analysis reveals:

- **Low satisfaction levels** are strongly correlated with employee departure
- **High workload** (average monthly hours) combined with low satisfaction increases churn risk
- **Tenure patterns** show distinct employee segments with different churn behaviors
- **Limited promotions** (only ~2% promoted) may impact retention

## 🛠️ Technologies & Libraries

- **Python 3.x**
- **Pandas** - Data manipulation and analysis
- **NumPy** - Numerical computing
- **Matplotlib** - Data visualization
- **Seaborn** - Statistical data visualization
- **Scikit-learn** - Machine learning models
- **Jupyter Notebook** - Interactive development environment

## 📊 Data Cleaning Summary

- **Missing Values:** None detected ✓
- **Duplicate Records:** 3,008 duplicates removed
- **Column Standardization:** Applied snake_case convention
  - `Work_accident` → `work_accident`
  - `average_montly_hours` → `average_monthly_hours`
  - `time_spend_company` → `tenure`
  - `Department` → `department`

## 🎓 Learning Outcomes

Through this capstone project, you will learn:

1. End-to-end data science workflow
2. Exploratory data analysis (EDA) techniques
3. Data cleaning and preprocessing
4. Building and evaluating predictive models
5. Feature importance analysis
6. Business problem-solving with data
7. Communicating insights to stakeholders

## 📝 Deliverables

This project includes:

1. **Jupyter Notebook** - Complete analysis with code and visualizations
2. **Data Visualizations** - Charts and graphs directly related to insights
3. **Model Evaluation** - Performance metrics and model interpretation
4. **Business Recommendations** - Actionable insights for HR department
5. **Ethics Considerations** - Responsible AI practices in HR analytics

## 🔐 Ethical Considerations

When working with employee data, it's important to consider:

- **Privacy** - Protect individual employee information
- **Fairness** - Ensure predictions don't discriminate based on protected characteristics
- **Transparency** - Clearly communicate how models make predictions
- **Accountability** - Use insights responsibly for employee welfare, not just cost-cutting
- **Bias Detection** - Monitor for unintended consequences in different demographic groups

## 📚 How to Use This Repository

1. **Clone the repository:**
   ```bash
   git clone https://github.com/maheshwarampranay/Winter-upskilling-capstone.git
   cd Winter-upskilling-capstone
   ```

2. **Install required packages:**
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn jupyter
   ```

3. **Launch Jupyter Notebook:**
   ```bash
   jupyter notebook
   ```

4. **Open the main notebook:**
   - `Activity_Course_7_Salifort_Motors_project_lab.ipynb`

5. **Run cells sequentially** to reproduce the analysis

## 📖 References

- **Dataset Source:** [Kaggle - HR Analytics Dataset](https://www.kaggle.com/datasets/mfaisalqureshi/hr-analytics)
- **PACE Framework:** Google's problem-solving methodology
- **Machine Learning:** Scikit-learn Documentation
- **Data Visualization:** Matplotlib and Seaborn Documentation

## 👤 Author

**Pranay Maheshwar**
- Winter Upskilling Program - AY 2024-25

## 📄 License

This project is part of an educational program. Please refer to your institution's guidelines for usage and distribution.

## 🤝 Contributing

This is a capstone project for educational purposes. If you have suggestions or improvements, feel free to open an issue or submit a pull request.
