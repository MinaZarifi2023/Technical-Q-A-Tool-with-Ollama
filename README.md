# 🧠 Technical Q&A Tool with Ollama (llama3.2)

This is a simple command-line Python tool that uses the [Ollama](https://ollama.com) CLI with the `llama3.2` model to explain technical code snippets or questions in a clear and beginner-friendly way.

---

## 🚀 Features

- Ask **technical programming questions** directly in the terminal  
- Uses the `llama3.2` model via `ollama run`  
- Automatically formats your prompt to get clean and understandable explanations  
- Gracefully handles errors from the CLI

---

## 🧩 Example Use Case

```bash
$ python ask_llama.py
🔍 Technical Question Explainer using llama3.2
Type 'exit' to quit.

❓ Your technical question:
Please explain what this code does and why:
yield from {book.get("author") for book in books if book.get("author")}
``` 
💡 Explanation:
[ model response here... ]
---

## ⚙️ Requirements

- Python 3.7+
- Ollama CLI installed
- `llama3.2` model already pulled via:

```bash
ollama pull llama3.2
```

## 📦 How to Run
Make sure Ollama CLI is installed and set up correctly.

Clone this repository:
git clone https://github.com/MinaZarifi2023/Technical-Q-A-Tool-with-Ollama.git
cd Technical-Q-A-Tool-with-Ollama




