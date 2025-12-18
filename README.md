# Personal AI Portfolio Assistant 🤖📄

An interactive AI assistant built with **Gradio** and **OpenAI-powered models** that represents me (*Yug Agarwal*).
It answers questions about my background, skills, projects, and experience, and can also collect contact details or unanswered queries for follow-ups.

🚀 **Live Demo:** [https://personal-ai-portfolio-assistant.onrender.com](https://personal-ai-portfolio-assistant.onrender.com)

---

## 📌 What it does

* 💬 Conversational assistant that responds as *Yug Agarwal*, grounded in my resume and LinkedIn data.
* 🧠 Uses **OpenAI GPT models** via **OpenRouter** for reliable, high-quality responses.
* 📄 Ingests structured and unstructured data from `summary.txt` and `linkedin.pdf`.
* 🔔 Captures unknown questions and user contact details using **Pushover notifications**.
* 🌐 Clean, minimal **Gradio UI** designed for quick interaction.

---

## ⚙️ Tech Stack

* **Python 3.10+**
* **Gradio** – frontend and interaction layer
* **OpenAI API (via OpenRouter)** – LLM access
* **PyPDF** – parsing LinkedIn PDF data
* **python-dotenv** – environment variable management
* **Pushover API** – alerts for unanswered queries and user details

---

## 🧠 How it works

1. Loads personal context from `summary.txt` and `linkedin.pdf`.
2. Builds a system prompt that constrains the assistant to answer strictly from this data.
3. Routes user queries through OpenRouter-backed LLMs.
4. Logs unanswered or out-of-scope questions and optional user contact info via Pushover.
5. Serves everything through a lightweight Gradio interface.

---

## 🚀 Deployment

The app is deployed on **Render** and auto-deploys on every push to the main branch.

### Run locally

```bash
# Clone the repository
# Clone the repository
git clone https://github.com/YugAgarwal005/Personal-AI-Portfolio-Assistant.git
cd Personal-AI-Portfolio-Assistant


# Create and activate a virtual environment
python -m venv venv
source venv/bin/activate   # Linux / macOS
venv\Scripts\activate      # Windows


# Install dependencies
pip install -r requirements.txt


# Start the app
python app.py
```

---

## 🔐 Environment Variables

Create a `.env` file in the project root:

```env
OPENROUTER_API_KEY=your_openrouter_api_key
PUSHOVER_USER_KEY=your_pushover_user_key
PUSHOVER_APP_TOKEN=your_pushover_app_token
```

---

## 📈 Use cases

* Personal portfolio assistant for recruiters and collaborators
* Interactive alternative to a static resume or website
* Experimentation with prompt design, RAG-style context injection, and notifications

---

## 🧩 Future improvements

* Vector-based retrieval for larger documents
* Conversation memory per user session
* Resume upload and dynamic context switching
* Analytics on user queries and interests

---

## 📬 Contact

If this project interests you or you want to collaborate, feel free to reach out through the assistant itself or connect with me on GitHub and LinkedIn.
