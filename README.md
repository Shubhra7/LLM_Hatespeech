# 🚫 Hate Speech Detection using LLMs (XLM-RoBERTa, BERT, BiLSTM)

Detecting hate speech in multilingual social media content using cutting-edge Large Language Models (LLMs) and deep learning techniques.

![Python](https://img.shields.io/badge/Language-Python-blue.svg)
![Model](https://img.shields.io/badge/Model-XLM--RoBERTa-green)

---

## 📌 Project Overview

This project aims to build a **robust and multilingual hate speech detection system** using advanced NLP techniques. It combines **transfer learning (BERT, XLM-RoBERTa)** and **deep sequence models (LSTM, BiLSTM)** to classify social media content as either *Neutral* or *Non-Neutral (Hateful)*.

---

## ✨ Highlights

- ✅ Pre-trained LLMs: **XLM-RoBERTa, BERT**
- 🔄 Models Compared: **LSTM, BiLSTM, BERT, XLM-RoBERTa**
- 🏆 Achieved **F1-Score: 91%**
- 🌐 Multilingual Support: **English, Bengali, Many More**
- 📊 Deployed using: **Streamlit & Gradio** 
- 📁 Datasets from **Twitter, Stormfront, Hugging Face**, etc.

---

## 🧠 Architecture

The proposed pipeline includes:

- **Text Preprocessing**
  - Cleaning, tokenization, label encoding

- **Transfer Learning**
  - Fine-tuned XLM-RoBERTa

- **Model Ensemble**
  - Compared LSTM, BiLSTM, BERT, and final XLM-RoBERTa model

- **Training & Validation**
  - K-Fold Cross-Validation
  - Evaluation using Accuracy, F1 Score, ROC AUC

- **Deployment**
  - Real-time prediction with Gradio & Streamlit interfaces

---

## 📂 Dataset Sources

| Dataset        | Source       | Language | Labels        | Size  |
|----------------|--------------|----------|---------------|-------|
| Waseem et al.  | Twitter       | English  | Hate/Neutral  | 6.3k  |
| Gilbert et al. | Stormfront    | English  | Hate/Neutral  | 10.9k |
| Reza et al.    | HuggingFace   | Bengali  | Hate/Neutral  | 10.9k |

---

## 📊 Results & Comparative Analysis

| Model              | Accuracy | F1 Score | Notes                                     |
|--------------------|----------|----------|-------------------------------------------|
| LSTM               | 75%      | 0.746    | Baseline sequential model                 |
| BiLSTM             | 77%      | 0.767    | Bi-directional context                    |
| BERT               | 83%      | 0.826    | Improved semantic understanding           |
| **XLM-RoBERTa**    | **91%**  | **0.908**| Best performance; multilingual edge       |

---

## 🚀 Getting Started

### 🔧 Installation

```bash
git clone https://github.com/Shubhra7/LLM_Hatespeech.git
cd LLM_Hatespeech
pip install -r requirements.txt
streamlit run app.py
