# News Category Classification

Machine Learning project for multi-class news category classification using traditional Machine Learning, Transformer Embeddings, and Deep Learning approaches.

---

# Course Information

* **Course:** Machine Learning (CO3107)
* **Semester:** Semester 2
* **Academic Year:** 2025 - 2026
* **Faculty:** Faculty of Computer Science and Engineering
* **University:** Ho Chi Minh City University of Technology (HCMUT)
* **Vietnam National University - Ho Chi Minh City**

---

# Instructor

* **Instructor:** PhD.Trương Vĩnh Lân

---

# Team Members

| Full Name            | Student ID |
| -------------------- | ---------- |
| Huỳnh Huy Hoàng      | 2311041    |
| Trần Nguyễn Đức Hưng | 2311359    |
| Phan Gia Phúc        | 2312709    |
| Nguyễn Gia Khiêm     | 2211572    |
| Nguyễn Mạnh Trung    | 2313674    |

---

# Project Objective

The objective of this project is to build a machine learning system capable of automatically classifying news articles into corresponding categories using Natural Language Processing (NLP) techniques.

The project explores and compares multiple approaches, including:

* Traditional Machine Learning methods
* TF-IDF and Bag-of-Words representations
* Transformer-based embeddings
* Deep Learning architectures

The final goal is to evaluate the effectiveness of each approach on multi-class news classification tasks.

---

# Dataset

Dataset: **News Category Dataset**

* Source: HuffPost News
* Time range: 2012 - 2022
* Total samples: ~209,000
* Original categories: 42

After preprocessing, the project keeps the **Top 15 most frequent categories** to reduce class imbalance and improve training stability.

Dataset link:

https://www.kaggle.com/datasets/rmisra/news-category-dataset

---

# Project Pipeline

## 1. Exploratory Data Analysis (EDA)

* Category distribution
* Text length analysis
* Vocabulary analysis
* TF-IDF keyword extraction
* N-gram analysis

---

## 2. Data Preprocessing

* Missing value handling
* Duplicate removal
* Text cleaning
* Lowercasing
* URL & HTML removal
* Stopword removal
* Lemmatization
* Train/Validation/Test split

---

## 3. Text Representation

Traditional methods:

* Bag-of-Words (BoW)
* TF-IDF

Transformer embeddings:

* RoBERTa Embedding
* Sentence-BERT (SBERT)

---

## 4. Machine Learning Models

Implemented models:

* LinearSVC
* Random Forest
* Gradient Boosting
* LightGBM
* CatBoost

---

## 5. Deep Learning Model

Custom architecture:

* Embedding Layer
* BiLSTM
* Masked Attention
* Dense Layers
* Dropout

---

# Best Results

| Model               | Accuracy | Macro F1 |
| ------------------- | -------- | -------- |
| TF-IDF + LinearSVC  | 76.13%   | 69.88%   |
| RoBERTa + LinearSVC | 76.86%   | 71.38%   |

RoBERTa embeddings achieved the best balance across categories.

---


---

# Installation

Clone the repository:

```bash
git clone https://github.com/your-username/news-category-classification.git
cd news-category-classification
```

---

# How To Run

Open Jupyter Notebook:

```bash
jupyter notebook
```

Then run notebooks inside:

```bash
notebooks/
```
---

# Requirements

Main libraries used in this project:

* Python
* Pandas
* NumPy
* Scikit-learn
* NLTK
* Transformers
* SentenceTransformers
* TensorFlow / Keras
* CatBoost
* LightGBM

---

# Report PDF

Project report:

```bash
reports/final_report.pdf
```

---

# Google Kaggle Notebooks

* Feature Extraction:
  https://www.kaggle.com/code/kimanaru/tr-ch-xu-t-c-tr-ng-m-h-nh

* Bow RandomForest, LightGBM, LinearSVC:
  https://www.kaggle.com/code/hoanghaha/bow-models-randomforest-lightgbm-linearsvc 

* Deep Learning Pipeline:
  https://www.kaggle.com/code/kimanaru/pipeline-h-c-s-u

* BERT + LinearSVC:
  https://www.kaggle.com/code/kimanaru/bert-linearsvc 

* TF-IDF + Catboost:
  https://www.kaggle.com/code/kimanaru/bert-linearsvc 
https://www.kaggle.com/code/huyhonghunh/th-c-c-tr-ch-xu-t-model?scriptVersionId=317112987
---

# References

* HuggingFace Transformers
* Scikit-learn Documentation
* Kaggle News Category Dataset
* BERT: Pre-training of Deep Bidirectional Transformers for Language Understanding
