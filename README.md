# Fake News Detection Using Machine Learning

## 🔍 Project Overview

This project builds a fake news classifier trained on news headlines. We compare multiple approaches:

- **Classical ML:** Logistic Regression, Naive Bayes, Random Forest, XGBoost, SVM, Word2Vec
- **Feature Extraction:** TF-IDF and Bag of Words (BOW) with bigrams
- **Deep Learning:** Neural Network with BERT embeddings (Sentence Transformers), FastText
- **Preprocessing:** Stopword removal, lemmatization, stemming, special character, punctuation and number removal

---

## Project Goals

- Detect fake vs real news automatically
- Compare multiple machine learning approaches
- Improve text classification through preprocessing
- Reduce overfitting and improve generalization
- Deploy a practical fake news classifier

---

## 📁 Dataset

- **Training data:** `training_data_fixed.csv` — 34,152 labeled news headlines
  - `0` = Fake news
  - `1` = Real news
- **Test data:** `testing_data_lowercase_nolabels.csv` — 9,984 unlabeled headlines for Kaggle submission
- **Split:** 80% train / 20% test
---

## 📂 Project Structure
```text
├── Models/
│   ├── BoW-Models & Word2Vec-Model.ipynb
│   ├── DD_V3.ipynb           
│   ├── Group2.csv
│   ├── Preprocessing+final_model.ipynb
│   └── embeddings_fasttext.ipynb
│
├── Presentation Slides/
│   └── Fake News Detection Presentation.pptx
│
└── README.md
```

---

## ⚙️ Tech Stack
Python
NumPy
Pandas
Matplotlib
Jupyter Notebook 

---

## Final Results (Top 5 Models)

| Rank | Model | Test Accuracy |
|------|------|--------------|
| 🥇 | Triple Hybrid Ensemble | 95.58% |
| 🥈 | Naive Bayes + TF-IDF + Stemming + N-gram | 94.28% |
| 🥉 | SVM + TF-IDF + Stemming + N-gram | 93.53% |
|  4 | Naive Bayes + TF-IDF + Stemming + N-gram | 93.40% |
|  5 | FastText Embeddings | 92.00% |

---

## Winner Model

### Triple Hybrid Ensemble & Metrics

- Multinomial Naive Bayes
- Logistic Regression
- FastText Embeddings

| Metric | Score |
|------|------|
| Train Accuracy | 97.06% |
| Test Accuracy | 95.58% |
| F1-Score | 0.9327 |
| Generalization Gap | 1.48% |

---

## Validation Strategy

- Accuracy Score
- F1 Score
- Cross Validation
- Generalization Checks

---

## 👥 Team : Group 2, Ironhack AI-bootcamp 2026 

- Rima
- Domien
- Dimi

---

## Run Project

```
# pip install notebook
# jupyter notebook
# Notebook : Models/Preprocessing+final_model.ipynb
# Open the notebook and run all cells.
# The notebook installs the required libraries inside the notebook cells.

```
---

## Final Conclusion

With **95.58% accuracy**, the Triple Hybrid Ensemble provides a strong and scalable solution for fake news classification.
