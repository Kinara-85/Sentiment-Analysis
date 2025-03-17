# Sentiment Analysis on IMDB Movie Reviews

This project uses **Deep Learning** to analyze the sentiment of IMDB movie reviews. The goal is to classify each review as **positive** or **negative** using **Neural Networks** (Simple Neural Network, CNN, and LSTM).

---

## 📌 Overview

- **Dataset**: [IMDB movie reviews dataset](https://drive.google.com/file/d/1He6pot7hsWfSURS0Kh-MlmDyQqfRUUdd/view?usp=drive_link) (CSV format)
- **Goal**: Predict whether a review is **positive** or **negative**
- **Methods Used**:
  - **Data Preprocessing**: Cleaning and tokenizing text
  - **Word Embeddings**: Using pre-trained **GloVe embeddings**
  - **Deep Learning Models**:
    - Simple **Neural Network (SNN)**
    - **Convolutional Neural Network (CNN)**
    - **Long Short-Term Memory (LSTM)**

---

## 📂 Project Structure

```
├── dataset
│   ├── IMDB_Dataset.csv  # Movie reviews dataset
│   ├── glove.6B.100d.txt  # Pre-trained word embeddings
│
├── models
│   ├── snn_model.h5   # Trained Simple Neural Network
│   ├── cnn_model.h5   # Trained CNN model
│   ├── lstm_model.h5  # Trained LSTM model
│
├── sentiment_analysis.py  # Main script
├── requirements.txt  # Required Python packages
├── README.md  # Project Documentation
```

---

## 🚀 Process Flow

### **1️⃣ Data Collection**
- Load **IMDB movie reviews** dataset using Pandas.

### **2️⃣ Data Preprocessing**
- Remove **HTML tags**, punctuation, and special characters.
- Convert text to **lowercase**.
- Remove **stopwords** (common words like *is, the, and*).
- Tokenize words and convert them into **numerical sequences**.

### **3️⃣ Word Embeddings**
- Load **pre-trained GloVe embeddings** to understand word relationships.
- Create an **embedding matrix** for our dataset.

### **4️⃣ Model Training**
We experiment with three models:
1. **Simple Neural Network (SNN)**: Basic model with embedding and dense layers.
2. **Convolutional Neural Network (CNN)**: Uses convolution layers to detect key phrases.
3. **Long Short-Term Memory (LSTM)**: Remembers word order and captures context.

### **5️⃣ Model Evaluation**
- Evaluate performance on test data.
- Plot accuracy and loss curves for training vs. validation.

### **6️⃣ Predictions**
- Test the model on new reviews.
- Save the trained model for future use.

---

## 📚 Credits
- Dataset Source: **[Skillcate AI](https://drive.google.com/file/d/1He6pot7hsWfSURS0Kh-MlmDyQqfRUUdd/view?usp=drive_link)**

