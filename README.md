# 🌐 OmniChat AI – Universal Multi-Platform AI Chatbot

OmniChat AI is an **LLM-powered universal chatbot** that works across multiple messaging platforms such as WhatsApp, Telegram, Instagram, and Messenger.

It combines **Large Language Models (LLMs), Retrieval Augmented Generation (RAG), and conversation memory** to provide intelligent responses based on uploaded documents and conversation context.

The system allows businesses or developers to deploy **one AI backend** that can serve multiple communication platforms.

---

# 🚀 Features

### 🤖 AI-Powered Responses

Uses an LLM to generate intelligent and contextual replies.

### 📚 RAG (Retrieval Augmented Generation)

The chatbot retrieves relevant information from uploaded documents before generating answers.

### 📄 Document Upload

Upload PDFs or text files to create a custom knowledge base.

### 🧠 Conversation Memory

Remembers previous messages to maintain context in conversations.

### 🌍 Multi-Platform Messaging

Designed to support multiple messaging services:

* Telegram
* WhatsApp
* Instagram
* Facebook Messenger

### ⚡ FastAPI Backend

High-performance asynchronous API built using FastAPI.

---

# 🧠 System Architecture

```
Messaging Platforms
(WhatsApp / Telegram / Instagram)
            │
            ▼
        FastAPI Server
            │
            ▼
       Document Upload
            │
            ▼
        Vector Database
          (Chroma)
            │
            ▼
     Retrieval Augmented Generation
            │
            ▼
        Large Language Model
            │
            ▼
     Conversation Memory Layer
            │
            ▼
           Response
```

---

# 📁 Project Structure

```
universal_ai_bot/
│
├── main.py
├── ai_engine.py
├── rag_engine.py
├── memory.py
├── upload_docs.py
│
├── data/
│   └── docs/
│
├── vectordb/
│
└── requirements.txt
```

---

# ⚙️ Installation

Clone the repository

```
git clone https://github.com/yourusername/universal-ai-bot.git
cd universal-ai-bot
```

Install dependencies

```
pip install -r requirements.txt
```

---

# ▶️ Run the Server

```
uvicorn main:app --reload
```

Server will run on:

```
http://localhost:8000
```

---

# 📄 Upload Knowledge Documents

Upload a document (PDF/TXT) to create a knowledge base.

Endpoint:

```
POST /upload
```

Example:

```
curl -F "file=@catalog.pdf" http://localhost:8000/upload
```

---

# 💬 Chat with the AI

Endpoint:

```
POST /chat
```

Example request:

```
{
 "user_id": "123",
 "message": "What products do you sell?"
}
```

Example response:

```
{
 "reply": "We offer laptops, headphones, and other accessories."
}
```

---

# 🧠 Technologies Used

* Python
* FastAPI
* LangChain
* Chroma Vector Database
* Sentence Transformers
* OpenAI LLM

---

# 📌 Use Cases

* Customer Support Automation
* Business Knowledge Assistant
* Multi-platform Chatbot
* AI Helpdesk System
* Document Question Answering

---

# 🔮 Future Improvements

* Voice message support
* Admin dashboard
* Real-time analytics
* Agentic tool calling
* Multi-language support

---

# 👨‍💻 Author

Harsh Chaturvedi

BTech AI Student | AI Developer | Hackathon Builder

---

# ⭐ If you like this project

Give the repository a star ⭐
