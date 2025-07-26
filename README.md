# 🚀 SmartTutor: Your Personalized AI Tutor

[![Run on Streamlit Community Cloud](https://img.shields.io/badge/Run_on_Streamlit_Community_Cloud-green)](https://smarttutor.streamlit.app)
[![Google GenerativeAI](https://img.shields.io/badge/google--generativeai-0.8.4-blue?logo=google)](https://github.com/google-gemini/generative-ai-python)
[![Streamlit Version](https://img.shields.io/badge/streamlit-1.43.2-blue?logo=streamlit)](https://streamlit.io/)
[![Python Version](https://img.shields.io/badge/python-3.12-blue?logo=python)](https://www.python.org/downloads/)
[![MIT License](https://img.shields.io/badge/License-MIT-green)](https://opensource.org/licenses/MIT)

**SmartTutor** is an AI-powered educational assistant built with Streamlit. It leverages Google's **Gemini 1.5** and **Gemini 2.0 Flash** models to provide interactive tutoring sessions. Instead of giving direct answers, SmartTutor encourages students to think, offering hints, guided prompts, and explanations to support active learning.

---

## 🎯 Features

- 🤖 **Powered by Gemini 2.0 & Gemini 1.5 Flash**
- 📘 **Interactive Learning**: Ask questions and get step-by-step hints and explanations.
- 🧠 **Smart Feedback**:
  - ⭐ Emoji for correct answers
  - ⚠️ Warnings for restricted or direct-answer attempts
- 🧮 **LaTeX Math Support**
- 📎 **Upload PDFs** (e.g., problem sets)
- 💻 **Built-in Python Code Execution**
- 🔐 **No user tracking or data storage**
- 🌐 **100% Open Source and deployable on Streamlit Cloud**

---

## 🧑‍💻 How to Use

1. Launch the app and select your preferred model.
2. Enter a subject you'd like to study (e.g., "Algebra", "Python").
3. Ask your question in the chatbox.
4. The tutor will guide you using hints or prompts, without directly solving homework for you.
5. Upload PDF problems for help solving math and other content interactively.

---

## 📦 Installation & Deployment

### 🚀 Deploy on Streamlit Cloud

1. Fork this repo to your GitHub account.
2. Go to [Streamlit Cloud](https://share.streamlit.io/) and click **New app**.
3. Set the main file to `educhat.py` (or your renamed file).
4. In **Advanced Settings → Secrets**, add your API key like this:

```env
GEMINI_API_KEY="your_google_api_key"
💻 Local Installation

git clone https://github.com/harshalsoni-ai/SmartTutor.git
cd SmartTutor
pip install -r requirements.txt
streamlit run educhat.py

🔑 Requirements

    Python 3.12

    Streamlit 1.43.2

    Google Generative AI SDK (google-generativeai==0.8.4)

📁 File Structure

SmartTutor/
├── educhat.py           # Main Streamlit app file
├── requirements.txt     # Python dependencies
└── README.md            # Project documentation

📚 Learning Behavior

    Uses zero temperature for consistent and factual responses.

    Dynamically limits token use to avoid model cutoff errors.

    Encourages self-learning through guided prompts.

    Maintains full chat history using st.session_state.

🙋 About the Developer

This project was developed and personalized by Harshal Soni, based on the original open-source EduChat project. It is tailored for educational use, demonstration, and free deployment.