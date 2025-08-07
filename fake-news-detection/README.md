# Automated Fake News Detection Using Machine Learning & BERT

A comprehensive data science project for distinguishing fake and real news articles using both classic machine learning (TF-IDF, Logistic Regression, Random Forest) and advanced deep learning (BERT, Hugging Face Transformers).  
Techniques: EDA, text preprocessing, feature engineering, predictive modeling, and explainable AI (SHAP).

---

## Overview

- **Domain:** Natural Language Processing, News Media Analytics, Misinformation Detection  
- **Dataset:** Fake and Real News Dataset ([Kaggle link](https://www.kaggle.com/datasets/clmentbisaillon/fake-and-real-news-dataset))

---

## Files Included

- `FakeNewsDetection.ipynb`: Jupyter notebook with all code, analysis, and visualizations  
- `Automated-Fake-News-Detection-Using-Machine-Learning-BERT.pdf`: Full report with business context, methods, and findings  
- *(Place `Fake.csv` and `True.csv` in the folder for reproducibility)*

---

## Key Steps

**Data Preparation:**  
- Cleaning, deduplication, null handling  
- Feature engineering: combining title + text, stopwords, lemmatization

**EDA & Visualization:**  
- Label distribution, word frequencies, word clouds

**Text Preprocessing:**  
- Lowercasing, tokenization, stopword removal, lemmatization

**Predictive Modeling:**  
- Classical ML: TF-IDF + Logistic Regression, Random Forest  
- Deep Learning: BERT fine-tuning with Hugging Face Transformers  
- Model comparison: accuracy, ROC-AUC, confusion matrix

**Explainable AI:**  
- SHAP feature importance and token analysis

---

## Results & Insights

- **Classical models:**  
  Logistic Regression & Random Forest achieve high baseline accuracy (up to ~97%)
- **BERT:**  
  Fine-tuned BERT matches classical model accuracy and excels at nuanced examples (given sufficient compute)
- **SHAP:**  
  Important words and phrases are surfaced for each class, enhancing transparency
- **General finding:**  
  Automated models can reliably classify fake vs. real news on benchmark data; explainability is key for trust

---

## To Run

1. **Install requirements:**  
   - Python 3.8+  
   - `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`, `nltk`, `tqdm`, `transformers`, `torch`, `shap`, `wordcloud`
2. **Add data:**  
   - Place `Fake.csv` and `True.csv` in your working directory
3. **Open and run the notebook:**
   - jupyter notebook FakeNewsDetection.ipynb

---

## References

- [Kaggle Fake and Real News Dataset](https://www.kaggle.com/datasets/clmentbisaillon/fake-and-real-news-dataset)
- Devlin et al., “BERT: Pre-training of Deep Bidirectional Transformers for Language Understanding” (2018)
- See PDF for full citations

---

## Author

Aharon Rabson  
GitHub: [@Amrabson](https://github.com/Amrabson)
