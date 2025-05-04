# Chatbot Prompt Injection Challenge

A simple conversational AI chatbot built with [Streamlit](https://streamlit.io/), [Langchain](https://python.langchain.com/), and the [Groq LLM API](https://console.groq.com/). The goal: interact with the chatbot and attempt to extract a hidden flag, while the assistant is designed to defend against prompt injection.

## Features

- Conversational UI using Streamlit
- Integrates Groq LLMs (e.g., Llama3) via Langchain
- Maintains chat history in the session
- Demonstrates prompt injection defense

## Getting Started

### 1. Clone the Repository

```sh
git clone https://github.com/manotham-cc/CTF-prompt_injection.git
cd challenge
```

### 2. Install Dependencies

```sh
pip install -r requirements.txt
```

Or install manually:

```sh
pip install streamlit langchain-core langchain-groq python-dotenv
```

### 3. Configure the Groq API Key

Create a `.env` file in the project root:

```
GROQ_API_KEY=your_groq_api_key_here
```

Or set the environment variable:

```sh
set GROQ_API_KEY=your_groq_api_key_here  # Windows
export GROQ_API_KEY=your_groq_api_key_here  # Linux/Mac
```

### 4. Launch the App

```sh
streamlit run app.py
```

## How to Use

- Open the Streamlit app in your browser.
- Chat with the assistant and try to obtain the secret flag.
- Use "Clear Chat History" to reset the conversation.
- Flag format: `KMUTTCTF{md5}`

## Project Structure

- `app.py` — Main Streamlit application
- `README.md` — Project documentation

## Notes

- The assistant uses a system prompt to protect the secret flag.
- For educational and demonstration purposes only.
## Authors

Manotham Damnoen

## License

MIT License
