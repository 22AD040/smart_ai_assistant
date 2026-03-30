![GitHub stars](https://img.shields.io/github/stars/22AD040/smart_ai_assistant?style=social)
![GitHub forks](https://img.shields.io/github/forks/22AD040/smart_ai_assistant?style=social)
![GitHub repo size](https://img.shields.io/github/repo-size/22AD040/smart_ai_assistant)

---

![Python](https://img.shields.io/badge/Python-3.10-blue)
![Streamlit](https://img.shields.io/badge/Streamlit-App-red)
![LangChain](https://img.shields.io/badge/LangChain-AI-green)
![LangGraph](https://img.shields.io/badge/LangGraph-Workflow-purple)
![Gemini](https://img.shields.io/badge/Gemini-AI-brightgreen)
![LangSmith](https://img.shields.io/badge/LangSmith-Monitoring-blue)
![License](https://img.shields.io/badge/License-MIT-brightgreen)

---

# 🤖 Smart AI Assistant

> 🧠 AI-powered assistant using **LangGraph + RAG + Gemini AI**

---

## 🚀 Live Demo

🌐 **Streamlit App:**  
👉 https://smartaiassistant-rdwqygtwenqcekyznjbfzu.streamlit.app/

---

## 🧠 Overview

**Smart AI Assistant** is an intelligent chatbot system that:

- 💬 Answers user questions using AI
- 📄 Reads PDFs and performs RAG (Retrieval-Augmented Generation)
- 🧠 Uses LangGraph for decision-based workflows
- 📜 Stores chat history per user
- 🔐 Includes authentication system

---

## ✨ Features

### 🔐 Authentication
- Login / Register system
- Secure password hashing (bcrypt)
- SQLite-based user storage

---

### 🤖 AI Chat System
- Powered by **Google Gemini (gemini-2.5-flash)**
- Generates:
  - Structured answers
  - Headings & bullet points
  - Clear explanations

---

### 📄 RAG (PDF Support)
- Upload PDF documents
- Extract content
- Store embeddings using FAISS
- Answer based on document context

---

### 🔄 LangGraph Workflow
- Intelligent routing:
- 📚 RAG Agent
- 🧠 General AI Agent
- 🤖 Evaluation node for response quality
- 📊 Router Node → decides flow

---

### 📊 LangSmith Monitoring (IMPORTANT 🚀)

This project integrates **LangSmith** for:

- 🔍 Tracing each LangGraph execution
- 📈 Monitoring latency & token usage
- 🐞 Debugging errors
- 📊 Observing system performance

👉 Helps understand **how AI decisions are made internally**

---

### 💬 Chat History
- Stored in SQLite
- User-specific history
- Sidebar navigation

---

## 🧠 Tech Stack

| Technology        | Purpose                     |
|------------------|---------------------------|
| Streamlit        | Frontend UI               |
| LangChain        | LLM orchestration         |
| LangGraph        | Workflow logic            |
| Google Gemini    | AI Model                  |
| FAISS            | Vector database           |
| SQLite           | Database (users + chats)  |
| Python           | Core logic                |

---

## 📸 Screenshots

### 🔐 Login Page
![Login](assets/login.png)

### 💬 Chat Interface
![Chat](assets/chat.png)

### 📄 PDF Upload & RAG
![PDF](assets/pdf.png)

---

## 📁 Project Structure

```bash
smart-ai-assistant/
│
├── app/
│   ├── main.py
│   ├── auth.py
│   ├── chat.py
│
├── agents/
│   ├── graph.py
│   ├── rag_agent.py
│   ├── general_agent.py
│   ├── evaluator.py
│   ├── router.py
│
├── core/
│   ├── llm.py
│   ├── embeddings.py
│   ├── vector_store.py
│   ├── rag.py
│
├── services/
│   ├── memory.py
│   ├── prompts.py
│
├── utils/
│   ├── helpers.py
│
├── assets/
├── database/
├── requirements.txt
├── README.md
└── LICENSE

---

## ⚙️ Installation

### 1️⃣ Clone Repository

```bash
git clone https://github.com/22AD040/smart_ai_assistant.git
cd smart_ai_assistant
````

### 2️⃣ Create Virtual Environment

```bash
python -m venv venv
venv\Scripts\activate
```

### 3️⃣ Install Requirements

```bash
pip install -r requirements.txt
```

### 4️⃣ Setup Environment Variables

Create a `.env` file:

```env
GEMINI_API_KEY=your_key_here
```

### 5️⃣ Streamlit Secrets (for deployment)

```toml
GEMINI_API_KEY="your_key"
LANGCHAIN_API_KEY="your_key"
LANGCHAIN_TRACING_V2="true"
LANGCHAIN_PROJECT="smart-ai-assistant"
```

---

## ▶️ Run Locally

```bash
streamlit run app/main.py
```

---

## 🌐 Deployment

### 🔹 Streamlit Cloud

* Connect your GitHub repo
* Add secrets
* Deploy

---

## 🔒 Security

* 🔐 API keys stored securely
* 🚫 `.gitignore` prevents DB leakage
* 🔑 Password hashing using bcrypt
* 👤 User-specific data isolation

---

## ⚠️ Known Limitations

* SQLite not suitable for large-scale apps
* No multi-session chat threads
* No real-time streaming responses

---

## 🚀 Future Improvements

* 💬 ChatGPT-style UI
* 🗑 Delete chat option
* 📊 Analytics dashboard
* 🌍 Multi-language support
* ⚡ Faster response streaming

---

## 👩‍💻 Author

**Ratchita B**
🎓 AI & Data Science Student

---

## ⭐ Support

If you like this project:

👉 Star ⭐ the repo
👉 Share with others

---

## 📜 License

This project is licensed under the MIT License

---

```