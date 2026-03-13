# RAG Chatbot using n8n

This project is a Retrieval-Augmented Generation (RAG) chatbot built using n8n workflow automation.

The chatbot answers user questions based on company policy and FAQ documents stored in a PDF.

## Features

- AI powered chatbot
- PDF knowledge base
- Vector similarity search
- Automated workflow using n8n

## Tech Stack

- n8n (Workflow automation)
- OpenRouter (Chat model gateway)
- Pinecone (Vector database)
- OpenAI Embeddings
- Google Drive (Document storage)

## Architecture

User Question → n8n Workflow → Embedding Search → Pinecone Vector DB → Retrieve Context → LLM Response

## Workflow Steps

1. User sends question to chatbot
2. n8n receives query
3. Query converted to embedding
4. Pinecone searches relevant document chunks
5. Retrieved context sent to LLM via OpenRouter
6. LLM generates response

## Setup Instructions

1 Install n8n

2 Import the workflow JSON

3 Configure API keys
- OpenAI API
- Pinecone API
- OpenRouter API

4 Upload PDF to Google Drive

5 Run the workflow

## Example Questions

- What is the company's refund policy?
- What are the leave policies?
- What documents are required for onboarding?

## Future Improvements

- Add website chat widget
- Add multi-document support
- Add conversation memory
