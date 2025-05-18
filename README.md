# 💔 Relationship Breakup Prediction using Machine Learning

This project aims to analyze relationship-related text and predict whether a breakup is likely to happen. It's built using classic machine learning techniques and demonstrates end-to-end NLP processing.

---

## 📂 Dataset

The dataset used is `relationship_breakup_dataset.csv`. It contains rows of textual inputs (such as phrases or sentences people might say) labeled as either indicating a potential breakup or not.

- **Columns**: 
  - `text`: User-provided statement.
  - `label`: 0 (not a breakup signal) or 1 (likely a breakup signal)

The dataset is split into training and testing subsets using an 80/20 ratio.

---

## 🔍 Workflow

1. **Data Preprocessing**:
   - Convert all text to lowercase.
   - Remove punctuation and stopwords.
   - Apply stemming using NLTK's PorterStemmer.

2. **Feature Extraction**:
   - Use **TF-IDF Vectorization** to convert processed text into numerical vectors suitable for training.

3. **Model Training & Evaluation**:
   - Models used:
     - Logistic Regression
     - Support Vector Classifier (SVC)
     - Decision Tree Classifier
     - Random Forest Classifier
   - Accuracy is computed on the test set using `accuracy_score`.

4. **Prediction**:
   - The notebook allows testing new user input by processing the text and passing it through the trained model.

---
