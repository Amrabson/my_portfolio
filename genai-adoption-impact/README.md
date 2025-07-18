# Forecasting and Explaining the Impact of GenAI Adoption Across Global Enterprises

An advanced data science project examining how generative AI (GenAI) adoption affects productivity, workforce structure, and employee experience in global enterprises.  
**Techniques:** Exploratory data analysis, feature engineering, NLP sentiment analysis, predictive modeling, and explainable AI (SHAP).

---

## Overview

- **Domain:** AI, productivity, workforce analytics, enterprise transformation  
- **Dataset:** [Enterprise GenAI Adoption & Workforce Impact (Kaggle)](https://www.kaggle.com/datasets/tfisthis/enterprise-genai-adoption-and-workforce-impact-data)  
- **Files Included:**  
  - `GenAI_Notebook.ipynb`: Jupyter notebook with all code, analysis, and visualizations  
  - `Enterprise_GenAI_Adoption_Impact.csv`: Source dataset  
  - `Explaining_the_impact_of_GenAI.pdf`: Full white paper with business context, methodology, and findings

---

## Key Steps

- **Data Preparation:**  
  - Imputation, normalization, categorical cleanup  
  - Feature engineering: job creation rate, adoption period, sentiment polarity  
- **EDA & Visualization:**  
  - Distributions, boxplots, correlation heatmaps, sentiment analysis, word clouds  
- **NLP:**  
  - Sentiment analysis of employee comments using TextBlob  
- **Predictive Modeling:**  
  - Random Forest and XGBoost (regression & classification)
  - Feature importance and SHAP for interpretability  
- **Validation:**  
  - Cross-validation, ROC-AUC, confusion matrix

---

## Results & Insights

- **No single variable strongly predicts GenAI productivity gains in the provided data.**
- **Employee sentiment is mostly neutral, but transitions and learning are common themes.**
- **Modeling accuracy is moderate; explainable AI (SHAP) confirms results are distributed and not driven by outliers.**
- **Key drivers:** Training hours, job creation rate, and employees impacted (weak effects).

---

## To Run

1. **Install requirements**  
   - Python 3.9+  
   - `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`, `xgboost`, `textblob`, `shap`

2. **Open and run the notebook:**  
   ```bash
   jupyter notebook GenAI_Notebook.ipynb
  (You can explore all code, EDA, modeling, and visualizations interactively.)

  ---

## References

- [Dataset on Kaggle](https://www.kaggle.com/datasets/tfisthis/enterprise-genai-adoption-and-workforce-impact-data)
- McKinsey, Gartner, HBR, Deloitte, WEF: See PDF for full citations.

---

## Author

Aharon Rabson  
[GitHub: @Amrabson](https://github.com/Amrabson)
