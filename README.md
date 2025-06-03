# 🏷️ Automatic Question Tagging using NLP

Automatically predict relevant tags for user-submitted questions using Natural Language Processing (NLP) and machine learning, achieving **90% accuracy**.

---

## 📘 Project Overview

In Q&A platforms like Stack Overflow, accurate tagging is essential for content discoverability and efficient information retrieval. This project presents an **Automatic Question Tagging System** that leverages NLP techniques to classify and assign appropriate tags to a question based on its textual content.

---

## 🚀 Features

- Preprocessing of question text (tokenization, lemmatization, stop word removal)
- TF-IDF and Word Embedding-based feature extraction
- Multi-label classification using machine learning models
- Achieves up to **90% accuracy** on test data
- Scalable and efficient pipeline ready for real-time applications

---

## 🛠️ Tech Stack

- **Languages**: Python  
- **Libraries**: `scikit-learn`, `NLTK`, `spaCy`, `Pandas`, `NumPy`  
- **Model**: Logistic Regression / SVM / Random Forest / Multi-label Classifier  
- **Vectorization**: TF-IDF / Word2Vec  
- **Evaluation Metrics**: Accuracy, Hamming Loss, F1 Score

---

## 📂 Dataset

The dataset consists of user-submitted questions and their corresponding tags. Tags are typically multi-label, meaning each question may belong to multiple categories.

- **Format**: `.csv`
- **Columns**: `question_title`, `question_body`, `tags`

> *Dataset source: Kaggle / Custom-collected from Stack Overflow*

---

## ⚙️ Installation & Usage

```bash
# Clone the repository
git clone https://github.com/your-username/automatic-question-tagging.git
cd automatic-question-tagging

# Install dependencies
pip install -r requirements.txt

# Run the model
python train_model.py

# Predict tags for a new question
python predict.py --question "How to implement logistic regression from scratch in Python?"
