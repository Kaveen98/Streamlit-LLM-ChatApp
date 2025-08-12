# Streamlit LLM Chat App

This is a simple yet powerful Streamlit-based chatbot interface that allows you to interact with both local and remote Large Language Models (LLMs). 
It uses OpenRouter for cloud-based models and supports local model inference via `llama.cpp`.

---

<br>

## 🚀 Features

- ✅ Streamlit chat interface
- 🔄 Chat memory for continuous dialogue
- 🔌 Toggle between local and cloud-based LLMs
- 🔐 Environment-based API key handling
- 📦 Docker + docker-compose support for easy deployment

---

<br>

## 🛠️ Tech Stack

- Python 3.12
- Streamlit
- LangChain with `langchain_openai`
- dotenv for secure environment variable loading
- Docker & Docker Compose

---

<br>

## ⚙️ Setup Instructions

### 1. Clone the Repository

```
git clone https://github.com/Kaveen98/Streamlit-LLM-ChatApp.git
cd Streamlit-LLM-ChatApp
```

<br>

### 2. Set Up Environment Variables

Create a **.env** file (already included) and add the following:
```
LOCAL_BASE_URL=http://model-runner.docker.internal/engines/llama.cpp/v1
REMOTE_BASE_URL=https://openrouter.ai/api/v1
LOCAL_MODEL_NAME=ai/qwen2.5:0.5B-F16
REMOTE_MODEL_NAME=qwen/qwen3-30b-a3b
OPENROUTER_API_KEY=your_openrouter_api_key
```
*Note:* replace '**your_openrouter_api_key**' with your actual API key.  

<br>

### 3. Install Dependencies

```
pip install -r requirements.txt
```

<br>

### 4. Run the App

```
streamlit run app.py
```

---

<br>

### 🐳 Docker Instructions

Build and Run Locally
```
docker-compose up --build
```

---

<br>

## ✅ Usage

1. Type your message in the chat.
2. Toggle the "Switch to the cloud model" checkbox to switch between local and cloud models.
3. The app remembers previous messages for contextual replies.

---

<br>

## 📌 Notes

- Cloud model runs via OpenRouter API
- Local model runs through llama.cpp server
- You must run or expose a model-runner backend compatible with your local setup.

---

<br>

## Author
#### Kaveen Weerasena
📧 kaveenweerasena@gmail.com  
🔗 www.linkedin.com/in/kaveen-weerasena-60703776

<br>

---
