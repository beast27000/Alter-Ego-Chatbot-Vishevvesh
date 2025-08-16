# Alter Ego Chatbot – Vishevvesh

## Overview
This project demonstrates an **Alter Ego Chatbot** powered by **Large Language Models (LLMs)** and **Agentic AI**.  
The chatbot can parse a LinkedIn résumé (PDF), generate a structured self-summary, and interact through a Gradio-based conversational UI.  
It integrates **Azure OpenAI** for intelligent reasoning and supports agentic workflows to extend capabilities.

---

## Features
- **LinkedIn Resume Parsing**: Extracts text from your résumé PDF (`me/linkedin.pdf`).  
- **Automated Summary Generation**: Creates a `summary.txt` file describing your profile.  
- **Gradio UI**: Provides an interactive web interface for chatbot conversations.  
- **Azure OpenAI Integration**: Uses GPT-based models for reasoning and dialogue.  
- **Agentic AI Workflow**: Demonstrates multi-agent coordination for structured tasks.  

---

## Setup Instructions

### 2. Create Virtual Environment
```bash
python -m venv venv
source venv/bin/activate   # On macOS/Linux
venv\Scripts\activate      # On Windows
```

### 3. Install Dependencies
```bash
pip install -r requirements.txt
```

### 4. Configure Environment
Create a `.env` file in the root folder:
```plaintext
AZURE_OPENAI_KEY=your_api_key_here
AZURE_OPENAI_ENDPOINT=https://your-endpoint.openai.azure.com/
AZURE_OPENAI_DEPLOYMENT=gpt-4o-mini
AZURE_OPENAI_VERSION=2024-06-01
```

## Usage

### Step 1: Run the Notebook
Open the notebook:
```bash
jupyter notebook 3_lab3.ipynb
```

### Step 2: Upload LinkedIn PDF
Replace the placeholder file with your own résumé:
```
me/linkedin.pdf
```

### Step 3: Generate Summary
Running the notebook will produce:
```
summary.txt
```

### Step 4: Launch Chatbot
A Gradio web interface will open in your browser for interactive chat.

## Project Structure
```
├── me/
│   └── linkedin.pdf       # Your résumé file
├── summary.txt            # Auto-generated résumé summary
├── 3_lab3.ipynb           # Main notebook (chatbot + agents)
├── requirements.txt       # Project dependencies
└── README.md              # Documentation
```

## Notes
- Replace the sample `linkedin.pdf` with your own résumé before running.
- Extendable with agentic AI tools (e.g., web search, custom knowledge base).
- Built as a learning project for experimenting with LLM-powered agent workflows.

## Future Work
- Integrate speech-to-text for voice interaction.
- Add document-grounded question answering.
- Expand to multi-agent reasoning with external APIs.

## Author
Vishevvesh  
Project developed as part of exploring Agentic AI and LLM applications.

## Tech Stack
- Python 3.10+
- Jupyter Notebook
- Gradio – Chatbot UI
- pypdf – PDF parsing
- Azure OpenAI – LLM integration
- Autogen / Agentic AI Frameworks – Agent workflows
