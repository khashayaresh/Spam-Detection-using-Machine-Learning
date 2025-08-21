# Spam Detection using Machine Learning

This repository contains the implementation and report for a **Spam Detection** project, completed as part of **CS 530: Data Mining (Spring 2024)**.  
The project applies multiple machine learning algorithms to classify emails as **spam** or **ham (not spam)** using text mining and classification techniques.  

---

## Project Overview
Spam emails pose a significant challenge in digital communication, leading to wasted time, security risks, and financial losses. The goal of this project is to build and compare machine learning classifiers for **automatic spam detection**.  

We evaluate models on their ability to:
- Accurately classify spam vs. non-spam emails.  
- Minimize false positives (legitimate emails marked as spam).  
- Balance **precision**, **recall**, and **F1 score**.  

---

## Methodology
1. **Dataset**
   - The dataset consists of labeled emails (spam vs. ham).  
   - Preprocessing includes text cleaning, tokenization, stopword removal, and feature extraction.  

2. **Models Implemented**
   - Naïve Bayes: MultinomialNB, GaussianNB, BernoulliNB  
   - Logistic Regression  
   - Support Vector Machines (SVM)  
   - Random Forest Classifier  
   - Gradient Boosting Machine (GBM)  

3. **Evaluation Metrics**
   - Accuracy  
   - Precision  
   - Recall  
   - F1 Score  
   - ROC-AUC  

---

## Results Highlights
- **BernoulliNB**  
  - Highest Recall (**97.22%**) → best at catching spam.  
  - Strong F1 Score (**92.63%**) and ROC-AUC (**98.9%**).  
- **Logistic Regression & Random Forest**  
  - Balanced Precision & Recall, making them reliable in practice.  
- **GaussianNB**  
  - High Recall but lower Precision → more false positives.  
- **Trade-offs**  
  - Simple models (Naïve Bayes) are **fast & interpretable** but risk false positives.  
  - Complex models (SVM, Random Forest, GBM) are **more accurate** but slower and resource-intensive.  


---

## Repository Contents
- `Spam Detecting.ipynb` → Jupyter Notebook with code for preprocessing, training, and evaluation.  
- `Spam Detecting.pdf` → Full project report with methodology, results, and discussion.  
- `Spam Filtering Data.csv` → Email dataset used for training and testing (to be added).  

