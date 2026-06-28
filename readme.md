#  AI Chatbot

A conversational AI chatbot built with **Streamlit** and powered by **Groq's LLaMA 3 model**. Users can ask anything and get instant, intelligent responses in a clean and modern chat interface.

---

##  Live Demo
> Coming soon after deployment on Streamlit Cloud

---

##  What Does This Project Do?

This chatbot allows users to:
- Ask any question and get AI-powered responses
- Have a back-and-forth conversation (chat history is maintained)
- Experience a clean, modern dark-themed UI

---

##  How It Works — The Logic

```
User types a message
        ↓
Message is sent to Groq API
        ↓
Groq runs the LLaMA 3 model on the message
        ↓
AI generates a response
        ↓
Response is displayed in the chat UI
        ↓
Both user message + AI reply are saved in chat history
```

The app uses **Streamlit's session state** to remember the full conversation, so the AI understands context from previous messages — just like a real chat!

---

##  Tech Stack

| Technology | Purpose |
|------------|---------|
| Python | Core programming language |
| Streamlit | Frontend UI framework |
| Groq API | AI inference engine (super fast!) |
| LLaMA 3 (8B) | Large Language Model for responses |
| python-dotenv | Securely load API keys from .env file |

---

##  Project Structure

```
chatbot/
│
├── chatbot.py        # Main application file
├── .env              # API key stored here (NOT uploaded to GitHub)
├── .gitignore        # Tells Git to ignore the .env file
└── README.md         # This file
```

---

##  How to Run This Project Locally

### Step 1 — Clone the Repository
```bash
git clone https://github.com/sagardubeyokk/Ai_chatbot.git
cd Ai_chatbot
```

### Step 2 — Install Required Libraries
```bash
pip install streamlit groq python-dotenv
```

### Step 3 — Get Your Free Groq API Key
1. Go to [console.groq.com](https://console.groq.com)
2. Sign up for a free account
3. Click **"API Keys"** → **"Create API Key"**
4. Copy your key

### Step 4 — Create a `.env` File
Create a file named `.env` in the project folder and add:
```
GROQ_API_KEY=your_groq_api_key_here
```

### Step 5 — Run the App
```bash
streamlit run chatbot.py
```

The app will open automatically in your browser at `localhost:8501` 

---

##  API Key Security

- The API key is stored in a `.env` file
- The `.env` file is listed in `.gitignore`
- This means the key is **never uploaded to GitHub** — it stays safe on your local machine

---

##  Features

-  Real-time AI responses
-  Context-aware conversation (remembers chat history)
-  Beautiful dark-themed UI with glassmorphism design
-  Super fast responses powered by Groq
-  Clean and minimal interface

---

##  About

Built by **Daya Sagar** as part of a Generative AI learning project.

- GitHub: [@sagardubeyokk](https://github.com/sagardubeyokk)
- Built with: Python, Streamlit, Groq API