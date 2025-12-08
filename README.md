# 🚀 AI Chatbot (Streamlit + Python Backend)

Demo: https://chat-bot-g69fdrfdppx5nlo5d8pgfn.streamlit.app/

This is a lightweight AI chatbot application built using:

- **Python Backend**
- **Streamlit Frontend**
- **Google Gemini (via LangChain Google GenAI)**
- **Environment-based API key protection**

The project demonstrates how to safely load API keys using `.env`, structure a backend chatbot function, and create a clean Streamlit interface for interaction.

---

## 📁 Project Structure

```
project/
 ├── backend.py        # Chatbot backend (Gemini model)
 ├── frontend.py       # Streamlit UI
 ├── .env              # Environment variables (ignored in Git)
 ├── .gitignore        # Prevents API keys from leaking
 └── README.md
```

---

## 🔐 Environment Setup

### 1️⃣ Install dependencies

```bash
pip install streamlit python-dotenv langchain-google-genai
```

---

## 2️⃣ Create a `.env` file in the project root

```
GOOGLE_API_KEY=your_actual_api_key_here
```

⚠️ **IMPORTANT:**  
Never push your API key to GitHub.  
This project uses `.gitignore` to prevent `.env` from being committed.

---

## 🧠 Backend (backend.py) Overview

- Loads API key safely using `dotenv`
- Initializes Gemini model (`ChatGoogleGenerativeAI`)
- Provides a simple `chatbot()` function for frontend use



## ▶️ Running the Application

### 1️⃣ Run the backend (if needed separately)
```bash
python backend.py
```

### 2️⃣ Run Streamlit frontend
```bash
streamlit run frontend.py
```

## 📝 .gitignore Example

```
.env
__pycache__/
*.pyc
```

---

## ⭐ Features

- ✔ Secure API key handling  
- ✔ Streamlit UI  
- ✔ Modular backend  
- ✔ Gemini integration  
- ✔ Beginner-friendly structure  

---

## 📌 Future Improvements (Optional)

- Add memory / chat history  
- Add multiple model support  
- Add microphone input  
- Deploy to cloud (Render / HuggingFace / Railway / Streamlit Cloud)  

---

## 🧑‍💻 Author

Developed by **Ahad Maruf**  
Feel free to fork, improve, and contribute!
