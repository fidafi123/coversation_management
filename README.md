# Conversation Management & JSON Extraction (Groq API, OpenAI-compatible)

This repository contains a **Google Colab notebook** (`chat_management.ipynb`) that demonstrates:

1. **Task 1: Conversation Manager**
   - Tracks user–assistant messages.
   - Summarizes every *k* turns using Groq API.
   - Shows history + summaries.

2. **Task 2: JSON Schema Extraction**
   - Extracts structured details (name, age, email, phone, location).
   - Uses Groq API’s function-calling style.
   - Falls back to regex if LLM call fails.

3. **Task 3: Integrated Demo**
   - Combines conversation summarization + schema extraction.
   - Summarizes every k-th turn and stores extracted info in a DataFrame.

---

## 🚀 Features
- **Summarization** → periodic (k-th turn).
- **Extraction** → JSON schema style.
- **Integration** → summary + extracted info in one flow.
- **Environment** → Google Colab / Jupyter Notebook.

---

## 🛠️ Tech & Tools
- Python 3
- Libraries: `openai`, `requests`, `pandas`, `re`
- LLM Backend: Groq API (`llama-3.1-8b-instant`)

---

## ▶️ How to Run
1. Open the notebook in **Google Colab**.
2. Install dependencies:
   ```bash
   !pip install openai requests pandas
```

3. Set Groq API key:

import os
os.environ["GROQ_API_KEY"] = "your_api_key_here"
```
4. Run cells for:
- Task 1: Conversation Manager
- Task 2: Schema Extraction
- Task 3: Integrated Demo
