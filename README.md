📌 Project Overview
This project aims to build a robust and multilingual hate speech detection system using advanced NLP techniques. It combines transfer learning (BERT, XLM-RoBERTa) and deep sequence models (LSTM, BiLSTM) to classify social media content as either Neutral or Non-Neutral (Hateful).

✨ Highlights
✅ Pre-trained LLMs: XLM-RoBERTa, BERT

🔄 Models Compared: LSTM, BiLSTM, BERT, XLM-RoBERTa

🏆 Achieved F1-Score: 91%

🌐 Multilingual Support: English, Bengali

📊 Deployed using: Streamlit & Gradio (demo screenshots available)

📁 Datasets from Twitter, Stormfront, Hugging Face, etc.

🧠 Architecture
The proposed pipeline includes:

Text Preprocessing

Cleaning, tokenization, label encoding

Transfer Learning

Fine-tuned XLM-RoBERTa

Model Ensemble

Compared LSTM, BiLSTM, BERT, and final XLM-RoBERTa model

Training & Validation

K-Fold Cross-Validation

Evaluation using Accuracy, F1 Score, ROC AUC

Deployment

Real-time prediction with Gradio & Streamlit interfaces



📂 Dataset Sources
Dataset	Source	Language	Labels	Size
Waseem et al.	Twitter	English	Hate/Neutral	6.3k
Gilbert et al.	Stormfront	English	Hate/Neutral	10.9k
Reza et al.	HuggingFace	Bengali	Hate/Neutral	10.9k

📊 Results & Comparative Analysis
Model	Accuracy	F1 Score	Notes
LSTM	75%	0.746	Baseline sequential model
BiLSTM	77%	0.767	Bi-directional context
BERT	83%	0.826	Improved semantic understanding
XLM-RoBERTa	91%	0.908	Best performance; multilingual edge

🚀 Getting Started
🔧 Installation
bash
Copy
Edit
git clone https://github.com/Shubhra7/LLM_Hatespeech.git
cd LLM_Hatespeech
pip install -r requirements.txt
▶️ Run the App (Streamlit)
bash
Copy
Edit
streamlit run app.py
💡 Sample Prediction (via CLI)
python
Copy
Edit
from model import predict_hate
text = "I hate you for who you are"
predict_hate(text)
💬 Real-Time Interface (Screenshots)
Bengali Example	English Example

📚 Tech Stack
Python 3.8

PyTorch, Hugging Face Transformers

XLM-RoBERTa, BERT, LSTM

Streamlit, Gradio

Google Colab (GPU: Tesla T4)

🔮 Future Scope
🧩 Multimodal Hate Detection (text + image/video)

🧠 Bias mitigation and model interpretability

🌍 Support for more Indian and low-resource languages

⚡ Real-time content moderation systems integration
