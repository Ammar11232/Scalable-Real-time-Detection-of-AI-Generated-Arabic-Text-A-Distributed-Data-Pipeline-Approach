# Scalable-Real-time-Detection-of-AI-Generated-Arabic-Text-A-Distributed-Data-Pipeline-Approach
---

#  Overview of Project

This project aims to develop a scalable system for detecting AI-generated Arabic text using big data and machine learning techniques. With the rapid advancement of large language models (LLMs), distinguishing between human-written and AI-generated content has become increasingly difficult, raising concerns about authenticity and reliability. To address this challenge, this project utilizes Apache Spark for distributed data processing and implements a complete pipeline that includes text preprocessing, feature engineering, model training, and real-time streaming. The system combines both stylometric features, such as repeated letter patterns and sentence count, with advanced TF-IDF representations to capture linguistic and statistical characteristics of the text. Several machine learning models were trained and evaluated, including Logistic Regression, Support Vector Machines (SVM), and XGBoost. Experimental results indicate that Logistic Regression achieved the best balanced performance, effectively classifying both human-written and AI-generated text. In addition, a real-time streaming pipeline was implemented using Spark Structured Streaming to simulate live detection scenarios. Overall, this project demonstrates the effectiveness of combining big data frameworks with machine learning models for detecting AI-generated Arabic content in both offline and real-time environments.

---

#  Description of Task

The main task of this project is to develop a scalable system for detecting AI-generated Arabic text using big data technologies and machine learning techniques. The project focuses on building an end-to-end pipeline that processes raw Arabic text, extracts meaningful features, and trains classification models to distinguish between human-written and AI-generated content.

The implementation consists of several key stages:

- **Data Acquisition and Integration:**  
  Collecting Arabic abstracts from multiple sources, including both human-written and AI-generated text, and combining them into a unified dataset.

- **Text Preprocessing:**  
  Applying Arabic-specific preprocessing techniques such as normalization, diacritic removal, tokenization, stopword removal, and stemming to clean and standardize the text.
  
- **Feature Engineering:**  
  Extracting both:
  - Stylometric features (e.g., repeated letter patterns and sentence count)
  - Statistical features using TF-IDF representation

- **Model Training and Evaluation:**  
  Training multiple machine learning models including Logistic Regression, Support Vector Machine (SVM), and XGBoost, and evaluating their performance using metrics such as accuracy and F1-score.

- **Real-Time Streaming:**  
  Implementing a streaming pipeline using Spark Structured Streaming to simulate real-time text classification.

- **Scalability Analysis:**  
  Evaluating system performance by analyzing throughput and latency under different resource configurations.

The goal of this task is to build a system that is not only accurate but also scalable and capable of handling both batch and real-time data processing.

---

#  Data Collection

We utilize a substantial dataset comprising 41,940 Arabic research abstracts, which includes:

- **AI-generated abstracts produced using various large language models (LLMs)**
- **Human-written abstracts**

### Dataset Summary

| Split | Count |
|-------|--------|
| AI | 33552 |
| Human | 8388 |
| Training | 29358 |
| Validation | 6291 |
| Test | 6291 |
| Total Samples | 41940 |

---
#  Results Models

##  Baseline model

| **Model**                     | **Accuracy** | **F1-score** |
|-------------------------------|--------------|--------------|
| Logistic Regression           |     0.96     |     0.96     |


##  Machine Learning Model

| **Model**              | **Accuracy** |  **F1-score** |
|------------------------|--------------|---------------|
| Linear SVM             | 0.96         | 0.96          |
| XGBoost                | 0.89         | 0.88         | 
