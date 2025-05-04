# Cybersecurity Chatbot (Streamlit + Langchain + Groq)

This project is a simple conversational AI chatbot built with [Streamlit](https://streamlit.io/), [Langchain](https://python.langchain.com/), and [Groq LLM API](https://console.groq.com/). The assistant is designed to interact with users while keeping a secret flag safe from prompt injection attempts.

## Features

- Conversational UI powered by Streamlit
- Uses Groq LLMs (e.g., Llama3) via Langchain
- Maintains chat history in session
- Demonstrates prompt injection defense scenario

## Setup

### 1. Clone the repository

```sh
git clone https://github.com/manotham-cc/CTF-prompt_injection.git
cd challenge
```

### 2. Install dependencies

```sh
pip install -r requirements.txt
```

Or manually:

```sh
pip install streamlit langchain-core langchain-groq python-dotenv
```

### 3. Set your Groq API key

Create a `.env` file in the project root:

```
GROQ_API_KEY=your_groq_api_key_here
```

Or set it as an environment variable:

```sh
set GROQ_API_KEY=your_groq_api_key_here  # Windows
export GROQ_API_KEY=your_groq_api_key_here  # Linux/Mac
```

### 4. Run the app

```sh
streamlit run app.py
```

## Usage

- Open the Streamlit app in your browser.
- Chat with the assistant. Try to trick it into revealing the secret flag!
- Use the "Clear Chat History" button to reset the conversation.
- flag format KMUTTCTF{md5}
## File Structure

- `app.py` — Main Streamlit application
- `readme.md` — Project documentation

## Notes

- The assistant is initialized with a system prompt that instructs it to keep a secret flag safe.
- This project is for educational and demonstration purposes.

## License

MIT License
