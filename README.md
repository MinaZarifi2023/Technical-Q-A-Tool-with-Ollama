
# Technical Q&A Tool with Ollama (llama3.2)

A command-line tool that uses the `llama3.2` model via the [Ollama](https://ollama.com) CLI to explain technical code snippets or answer programming questions in simple terms.

This Python script lets you ask technical questions in the terminal and get simple explanations using the `llama3.2` model via the Ollama CLI.

* It formats your question into a prompt.
* Sends the prompt to the Ollama command-line tool using `subprocess`.
* Captures and shows the model’s response.
* If there's an error calling Ollama, it shows the error message instead of crashing.
* The program runs in a loop, letting you ask multiple questions until you type "exit".

The sample question asks for an explanation of a Python code snippet that extracts authors from a list of books.


## Features

- Accepts technical questions interactively from the terminal  
- Uses `ollama run llama3.2` to generate responses  
- Formats questions into prompts for better answers  
- Handles errors from the Ollama CLI without crashing  

## Requirements

- Python 3.7 or higher  
- Ollama CLI installed and configured  
- `llama3.2` model pulled via:


## Usage

Clone the repository and run the script:

```bash
git clone https://github.com/MinaZarifi2023/Technical-Q-A-Tool-with-Ollama.git
cd Technical-Q-A-Tool-with-Ollama
python ask_llama.py
```

## Example

```bash
$ python ask_llama.py
Technical Question Explainer using llama3.2
Type 'exit' to quit.

Your technical question:
Please explain what this code does and why:
yield from {book.get("author") for book in books if book.get("author")}

Explanation:
[ model response here... ]
Type your technical question at the prompt. Enter exit to quit
```


## How it works

- Reads your input question
- Creates a prompt for the llama3.2 model
- Runs Ollama CLI using subprocess with the prompt
- Returns and displays the model's explanation
- Shows error messages if the CLI call fails







