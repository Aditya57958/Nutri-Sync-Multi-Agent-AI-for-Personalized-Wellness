# Nutri-Sync-Multi-Agent-AI-for-Personalized-Wellness


Welcome to **Wellness AI**, an intelligent health and fitness assistant powered by advanced LLMs and [CrewAI](https://github.com/joaomdmoura/crewai)! This application uses multiple expert AI agents to provide **customized nutrition plans, yoga routines, exercise suggestions, mindset tips**, and **supplement recommendations** based on your personal inputs.

---

## 🚀 Project Overview

This project is a Gradio-based web application that allows users to input personal health data and receive a detailed wellness report. It utilizes a crew of autonomous agents, each specializing in a specific aspect of wellness like nutrition planning, fitness advice, mental wellness, and regional meal adaptation.

Each agent works collaboratively using the [CrewAI framework](https://github.com/joaomdmoura/crewai) and a powerful **LLM backend (LLaMA3-70B via Groq)** for fast and context-aware responses.

---

## 🧩 Features

✅ Personalized 28-day meal plans
✅ Yoga & exercise routines based on user fitness & goals
✅ Regional food recommendations
✅ Mindset & motivation tips
✅ Disease-specific nutrition planning
✅ Daily activity suggestions
✅ Supplement recommendations
✅ Simple and beautiful UI using **Gradio Tabs**

---

## 📦 Tech Stack

* **Python**
* **Gradio** – for UI
* **CrewAI** – to manage multi-agent task execution
* **Langchain Groq (LLaMA3 70B)** – fast LLM backend
* **Agents** – AI-powered specialists for each domain

---

## 📥 Installation

Clone the repo and install dependencies:

```bash
git clone https://github.com/yourusername/wellness-ai
cd wellness-ai
pip install -r requirements.txt
```

Or manually install:

```bash
pip install gradio crewai langchain_groq
```

> 🔐 Make sure to set your `GROQ_API_KEY` in the environment or directly pass it to the `ChatGroq` initializer.

---

## ⚙️ How It Works

1. **User inputs details** (age, country, dietary preferences, fitness goals, etc.).
2. A series of specialized agents are created with these inputs.
3. Tasks are assigned to each agent:

   * Meal plan creation
   * Yoga/exercise suggestions
   * Motivation and mindset coaching
   * Supplement guidance
   * Regional meal adjustments
   * Fitness enhancement tips
4. Outputs from each agent are collected and displayed as a comprehensive wellness report using Gradio.

---

## 🖥️ How to Run

```bash
python app.py
```

Or if the Gradio app is defined inside a script, you can run:

```bash
python your_script_name.py
```

Then open the local URL provided by Gradio (usually `http://127.0.0.1:7860/`) in your browser.

---

## 🧠 Sample Use Case

A 30-year-old user from Maharashtra, India, wants to lose weight. They’re diabetic, follow a vegetarian diet, and have a light fitness routine.

By filling out the form:

* A **meal plan** is generated that avoids sugar, respects vegetarian choices, and aims at weight loss.
* A **yoga & fitness routine** aligned with diabetes and stamina building is included.
* They also get **local Maharashtrian meal suggestions**, **supplement tips**, and **daily motivation** to stay consistent.

---

## 🔐 API Key Notice

This application uses **Groq’s LLaMA3-70B** model, which requires an API key:

```python
llm = ChatGroq(
    temperature=0,
    model_name="llama3-70b-8192",
    api_key='your_groq_api_key'
)
```

> ⚠️ **Never expose your real API key in public repositories!** Use `.env` files or secret management tools.

---

## 📄 Folder Structure

```
wellness-ai/
│
├── app.py                  # Main Python file with Gradio interface
├── README.md               # You're here!
├── requirements.txt        # Python dependencies
└── assets/                 # (Optional) For images or additional content
```

---

## 🧑‍💻 Contributing

Feel free to fork, enhance, and make this project even more powerful.

---

## 🙌 Acknowledgements

* [CrewAI](https://github.com/joaomdmoura/crewai)
* [LangChain + Groq Integration](https://python.langchain.com/docs/integrations/llms/groq/)
* [Gradio](https://www.gradio.app/)
* [Meta’s LLaMA 3 Model](https://ai.meta.com/llama/)

---

## 📢 Disclaimer

This tool is for educational and wellness purposes only and should not replace professional medical advice.

---

## 📬 Contact

Made with ❤️ by \[Aditya_]

