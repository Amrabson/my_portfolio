# Big Data Pipeline for Student Mental Health Analysis

A full-stack big data engineering and analytics project using **NiFi, HDFS, Hive, PySpark, and HBase** on the "Student Mental Health Analysis" dataset from Kaggle.  
This project demonstrates the end-to-end construction of a real-world data pipeline, from ingestion through machine learning to storage and analytics, focusing on educational and medical data.

---

## Project Overview

- **Domain:** Student mental health during online learning (medical/education)
- **Dataset:** [Student Mental Health Analysis](https://www.kaggle.com/datasets/utkarshsharma11r/student-mental-health-analysis)
- **Pipeline:** NiFi → HDFS → Hive → PySpark (ML) → HBase

---

## Pipeline Stages

1. **Data Ingestion (Apache NiFi):**
   - Automated retrieval of the CSV dataset from a public GitHub repo into HDFS.
   - Used NiFi processors (`InvokeHTTP`, `UpdateAttribute`, `PutHDFS`) for robust data flow.
2. **Data Lake (HDFS):**
   - Centralized storage of raw dataset files.
3. **Data Warehouse (Hive):**
   - External Hive table for efficient querying and SQL-based preprocessing.
   - Managed CSV parsing, header handling, and data type specification.
4. **Big Data Analytics (PySpark):**
   - Queried Hive tables from Spark, handled header quirks, and performed EDA.
   - Built ML models (logistic regression, random forest) to predict academic performance changes based on stress level, screen time, sleep duration, and physical activity.
   - Evaluated model accuracy and feature importance.
5. **Model Metrics Storage (HBase):**
   - Stored final model accuracy in HBase for persistent, rapid retrieval using HappyBase.

---

## Key Results

- **Model:** Logistic Regression (and Random Forest as secondary)
- **Target:** Predicting academic performance changes
- **Accuracy:** ~43%
- **Insights:** The chosen features provide some predictive value but highlight the complexity of student mental health; more features or sophisticated models are likely required.

---

## Issues & Resolutions

- **PySpark header row:** Filtered header row manually due to Hive/Spark limitation.
- **NiFi HDFS permissions:** Fixed via configuration and Hadoop permissions.
- **HBase Thrift:** Resolved zookeeper/RegionServer startup issues with manual restarts.

---

## References

- [Dataset on Kaggle](https://www.kaggle.com/datasets/utkarshsharma11r/student-mental-health-analysis)

---

## Author

Aharon Rabson  
[GitHub: @Amrabson](https://github.com/Amrabson)
