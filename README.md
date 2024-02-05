# Chatbot with Q&A using LangChain and OpenAI

This repository contains a Streamlit web application that integrates LangChain for text processing and OpenAI for question-answering. The chatbot is designed to provide answers based on a given set of documents, which can be loaded from a PDF file.

## Installation

Make sure you have the required packages installed. You can install them using the following:

```bash
pip install langchain openai PyPDF2 faiss-cpu tiktoken streamlit pyngrok==4.1.1
```

## Usage

1. Clone the repository:

```bash
git clone https://github.com/your_username/your_repo.git
cd your_repo
```

2. Download the PDF file:

```bash
wget https://pgcag.files.wordpress.com/2010/01/48lawsofpower.pdf
```

3. Run the Streamlit app:

```bash
streamlit run app.py
```

The application will open in your default web browser.

## Configuration

Before running the app, make sure to set your OpenAI API key. Create a `.env` file in the project root directory and add your API key:

```plaintext
OPENAI_API_KEY=your_api_key_here
```

## Q&A Examples

Here are a few examples of questions you can ask the chatbot:

1. "Can you give me an example from history where the enemy was crushed totally from the book?"
2. "What's the point of making myself less accessible?"
3. "Can you tell me the story of Queen Elizabeth I from this 48 Laws of Power book?"

Feel free to explore more questions and observe the chatbot's responses.

## Deployment

The app can be deployed using ngrok. Follow the instructions provided in the code to set up ngrok and expose your local server to the internet.

```bash
ngrok authtoken your_ngrok_authtoken_here
ngrok connect port='8501'
streamlit run /content/app.py
```

Visit the provided ngrok URL to access your deployed chatbot.

## Known Issues

If you encounter issues with port availability or need to restart the app, the included script helps to terminate the process on port 8501:

```bash
python kill_process.py
```

Make sure to run this script when needed to free up the port.

## Link for the App: [http://f75e-35-186-163-228.ngrok-free.app](https://45b9-104-198-218-80.ngrok-free.app/)

## Contributors

- Sakina Zaveri (@szaveri99)
- [OpenAI](https://github.com/openai)
- [LangChain Community](https://github.com/langchain-community)

Feel free to contribute and improve the functionality of this chatbot. Open issues or pull requests are welcome!
