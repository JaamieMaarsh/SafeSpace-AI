---
title: SafeSpace AI
emoji: 🧠
colorFrom: gray
colorTo: purple
sdk: gradio
sdk_version: 4.22.0
app_file: app.py
pinned: false
---

# 🧠 SafeSpace AI

**_We care for you._**  
SafeSpace AI is an intelligent mental health assistant built with Gradio and Google’s Gemma model, powered by Retrieval-Augmented Generation (RAG) and Whisper for seamless voice/text-based diagnosis and support.

---

## 🚀 Demo

> 🧪 Try it now: [SafeSpace AI on Hugging Face](https://huggingface.co/spaces/Jaamie/SafeSpace-AI)

![App Screenshot](https://huggingface.co/spaces/Jaamie/SafeSpace-AI/resolve/main/assets/screenshot.png)

---

## 🧩 Features

- 🎙️ **Voice Input** using Whisper
- 💬 **Text-based Queries** for emotional concerns
- 🔍 **RAG-powered Contextual Retrieval** via FAISS
- 🤖 **Mental Health Diagnosis** using fine-tuned Gemma
- 📄 **PDF Report Generation** with AI's response
- 📊 **Diagnosis Dashboard** (Plotly)
- 📝 **Anonymous Feedback Logging**
- 📂 **Downloadable Logs & Feedback CSVs**

---

## 🧠 Powered By

| Component         | Tech Used                                      |
|------------------|-------------------------------------------------|
| LLM              | `gemma-2-9b-it` (Google)                        |
| Embedding Model  | `BAAI/bge-base-en-v1.5`                         |
| Audio Model      | `openai/whisper-base`                          |
| UI Framework     | `Gradio`                                       |
| Retrieval Engine | `FAISS`                                        |
| Emotion Classifier| `nateraw/bert-base-uncased-emotion`           |


#### You can also use the pretrained gemma model on the this specific case, for more info : https://huggingface.co/Jaamie/gemma-mental-health-qlora
---

## ⚙️ Setup Locally

```bash
git clone https://github.com/JaamieMaarsh/SafeSpace-AI.git
cd SafeSpace-AI
pip install -r requirements.txt

# Create a .env file with your secrets
echo "HF_TOKEN=your_huggingface_token_here" > .env

# Run the app
python app.py
