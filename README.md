---
title: 1_foundations
app_file: app.py
sdk: gradio
sdk_version: 5.49.1
---

# AI Career Clone

An AI-powered chatbot that answers questions about my background, skills, and experience using my LinkedIn profile and personal summary.

The assistant runs locally using **Ollama** with the **Llama 3.2** model and provides an interactive chat interface built with **Gradio**.

## Features

- Powered by a local LLM
- Uses LinkedIn profile and personal summary as context
- Tool-calling system for performing actions
- Records user contact information
- Logs unanswered questions for future improvements
- Interactive web interface

## Tech Stack

- Python
- Gradio
- Ollama (Llama 3.2)
- OpenAI Python SDK
- Pushover API
- PyPDF

## How It Works

The chatbot loads my LinkedIn profile and summary, then answers questions as if it were me.  
If a user wants to get in touch, the assistant can record their email using a tool call.

If the model encounters a question it cannot answer, it logs the question so the system can be improved later.

## Running Locally

Install dependencies:

`pip install -r requirements.txt`

Install Ollama and download the model:

 `Ollama pull llama3.2`

Run the application:

`uv run app.py`

## Author

Dharshini Thirumal

Computer Science Graduate | Software Engineer