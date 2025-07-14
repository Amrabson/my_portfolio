# Student Depression Analysis

## Project Overview
This project aims to predict depression among university students using machine learning techniques, providing universities with a way to proactively support students at risk.

## Dataset and Features
- **Data Source:** [Kaggle Student Depression Dataset (27,901 records)](https://www.kaggle.com/datasets/adilshamim8/student-depression-dataset)
- **Features:** Age, gender, academic pressure, financial stress, sleep duration, dietary habits, suicidal thoughts, and more.
- **Target:** Depression status (binary classification, 1=Depressed, 0=Not Depressed)

## Project Files
- `StudentDepressionNotebook.ipynb`: Jupyter notebook for all code and analysis.
- `student_depression_dataset.csv`: The dataset used for analysis.
- `student_depression_rf_model.joblib`: Saved trained Random Forest model. *(Not included due to GitHub file size limits. Available upon request.)*
- `student_depression_eda_report.html`: Automated EDA profile report.
- `data dictionary.csv`: Data dictionary for all features.
- `StudentDepressionNotebook.pdf`: PDF report of the analysis.

## Methods
- Data Cleaning and Preprocessing
- Exploratory Data Analysis (EDA)
- Machine Learning Models:
  - Logistic Regression
  - Decision Trees
  - Random Forest
  - Gradient Boosting (Best performing model)
- Model Evaluation: Accuracy, Precision, Recall, F1-score, ROC-AUC
- Feature Importance and SHAP explainability

## Key Results
- Achieved approximately 85% accuracy with Gradient Boosting.
- Top predictive factors: suicidal thoughts, academic pressure, financial stress, age.
- No significant correlation found between gender and depression status.

## Installation
1. Clone the repo:
   ```bash
   git clone https://github.com/Amrabson/my_portfolio.git
   ```
2. Navigate to the project folder:
   ```bash
   cd my_portfolio/Student_Depression_Analysis
   ```

## Usage
- Open `StudentDepressionNotebook.ipynb` in Jupyter Notebook or JupyterLab.
- Follow the notebook cells to run data cleaning, EDA, modeling, and evaluation.
- Use `student_depression_rf_model.joblib` to load the pretrained model for predictions.

## License
This project is licensed under the MIT License.

## References
- [Kaggle: Student Depression Dataset](https://www.kaggle.com/datasets/adilshamim8/student-depression-dataset)

## Author
Aharon Rabson
