# Q&A Chatbot with OpenAI

A simple Streamlit app for asking questions with an OpenAI chat model. The app uses LangChain to build a prompt and display the model's response.

## Features

- Choose between `gpt-4o` and `gpt-4-turbo`
- Adjust response temperature and maximum output tokens
- Enter an OpenAI API key in the app's sidebar

## Requirements

- Python 3.9 or later
- An OpenAI API key with access to the selected model

## Setup

1. Clone this repository and change into its directory.
2. Create and activate a virtual environment:

   ```bash
   python -m venv .venv
   ```

   Windows PowerShell:

   ```powershell
   .venv\Scripts\Activate.ps1
   ```

   macOS or Linux:

   ```bash
   source .venv/bin/activate
   ```

3. Install the dependencies:

   ```bash
   pip install -r requirements.txt
   ```

## Run

Start the Streamlit app from the project directory:

```bash
streamlit run project.py
```

Enter your API key in the sidebar, select a model, adjust the settings, type a question, and click **Answer**.

## Security

The app requests the API key through a password field and passes it to the model client. Do not commit API keys or other secrets to GitHub. If you choose to store a key in a `.env` file, add `.env` to `.gitignore` first.

## Dependencies

Dependencies are listed in [`requirements.txt`](requirements.txt).
