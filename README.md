# AI-Powered RAG Knowledge Assistant

An AI-powered document question-answering system built using n8n, Ollama, and Supabase Vector Store. It allows users to upload PDF documents and ask questions based on their content.

## Project Overview

This project implements Retrieval-Augmented Generation (RAG) to retrieve relevant information from uploaded PDF documents and provide context-based answers.

The system is designed to answer questions using the uploaded document rather than relying on general knowledge.

## Technologies Used

- **n8n** – Workflow automation
- **Ollama** – Local text embeddings
- **all-minilm:l6-v2** – Text embedding model
- **Supabase** – Database and vector storage
- **PDF Extraction** – Document text extraction
- **Webhooks** – Frontend and backend integration
- **HTML, CSS, JavaScript** – User interface

## Key Features

- PDF document upload through a web interface.
- Automatic PDF text extraction.
- Text embeddings generated locally using Ollama.
- Vector storage and similarity search using Supabase.
- Question answering based on retrieved document content.
- Responses indicate when the requested information is unavailable in the uploaded documents.
- Integration between the frontend and n8n workflows.

## Workflow Architecture

**PDF Upload → Text Extraction → Text Chunking → Embeddings → Supabase Vector Store → Similarity Search → Context-Based Answer**

## Project Structure

```text
ai-powered-rag-knowledge-assistant/
├── workflows/
│   └── rag-workflow.json
├── screenshots/
└── README.md
```


## Project Screenshots

### PDF Upload Workflow
![PDF Upload Workflow](screenshots/pdf-upload-workflow.png)

### RAG Chat Workflow
![RAG Chat Workflow](screenshots/rag-chat-workflow.png)

### Working Application
![RAG Knowledge Assistant UI](screenshots/rag-assistant-ui.png)

## Setup Instructions

1. Install and run n8n.
2. Install Ollama and download the required embedding model.
3. Configure Supabase and create the required vector table and search function.
4. Configure the required credentials in n8n.
5. Import the workflow JSON files.
6. Configure the frontend webhook URLs.
7. Upload a PDF and test document-based questions.

## Important Note

This project uses a local embedding model. The language model used to generate answers depends on the configured workflow.

## Security

Do not publish API keys, access tokens, database passwords, or private documents in this repository.

## Author

Anuj Singh
