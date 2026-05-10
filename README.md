# News Category Classification

Machine Learning project for multi-class news category classification using traditional Machine Learning, Transformer Embeddings, and Deep Learning approaches.

---

## Overview

This project focuses on classifying news articles into different categories using the **News Category Dataset** from Kaggle.

The input text is created by combining:

* `headline`
* `short_description`

The target output is:

* `category`

The project explores multiple NLP pipelines ranging from traditional TF-IDF methods to modern Transformer-based embeddings and deep learning architectures.

---

## Dataset

Dataset: **News Category Dataset**

* Source: HuffPost News
* Time range: 2012 - 2022
* Total samples: ~209,000
* Original categories: 42

After preprocessing, the project keeps the **Top 15 most frequent categories** to reduce class imbalance and improve training stability.

---

## Project Pipeline

### 1. Exploratory Data Analysis (EDA)

* Category distribution
* Text length analysis
* Vocabulary analysis
* TF-IDF keyword extraction
* N-gram analysis

---

### 2. Data Preprocessing

* Missing value handling
* Duplicate removal
* Text cleaning
* Lowercasing
* URL & HTML removal
* Stopword removal
* Lemmatization
* Train/Validation/Test split

---

### 3. Text Representation

Traditional methods:

* Bag-of-Words (BoW)
* TF-IDF

Transformer embeddings:

* RoBERTa Embedding
* Sentence-BERT (SBERT)

---

### 4. Machine Learning Models

Implemented models:

* LinearSVC
* Random Forest
* Gradient Boosting
* LightGBM
* CatBoost

---

### 5. Deep Learning Model

Custom architecture:

* Embedding Layer
* BiLSTM
* Masked Attention
* Dense Layers
* Dropout

---

## Best Results

| Model               | Accuracy | Macro F1 |
| ------------------- | -------- | -------- |
| TF-IDF + LinearSVC  | 76.13%   | 69.88%   |
| RoBERTa + LinearSVC | 76.86%   | 71.38%   |

RoBERTa embeddings achieved the best balance across categories.

---

## Project Structure

```bash
news-category-classification/
│
├── data/
├── notebooks/
├── src/
├── models/
├── reports/
├── results/
└── README.md
```

---

## Installation

Clone the repository:

```bash
git clone https://github.com/your-username/news-category-classification.git
cd news-category-classification
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## Run Experiments

Example:

```bash
python src/models/linearsvc.py
```

or open notebooks:

```bash
jupyter notebook
```

---

## Technologies Used

* Python
* Scikit-learn
* Pandas
* NumPy
* NLTK
* Transformers
* SentenceTransformers
* TensorFlow / Keras
* CatBoost
* LightGBM

---

## Authors

* Huỳnh Huy Hoàng
* Trần Nguyễn Đức Hưng
* Phan Gia Phúc
* Nguyễn Gia Khiêm
* Nguyễn Mạnh Trung

Faculty of Computer Science and Engineering
Ho Chi Minh City University of Technology (HCMUT)

---

## References

* HuggingFace Transformers
* Scikit-learn Documentation
* Kaggle News Category Dataset
* BERT: Pre-training of Deep Bidirectional Transformers for Language Understanding
