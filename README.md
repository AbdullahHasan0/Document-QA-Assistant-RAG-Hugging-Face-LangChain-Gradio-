# AI-Powered PDF Question Answering (RAG Pipeline)

A general-purpose, AI-powered Retrieval-Augmented Generation (RAG) pipeline for asking questions about documents (any PDF).
Built with Mistral-7B-Instruct (LLM), BGE Large (v1.5) embeddings, LangChain, and ChromaDB — fully Colab-friendly.

## ⚠️ Disclaimer

Add your Hugging Face API key first in Colab Secrets or as an environment variable (HF_API_KEY).

This notebook is for educational/demo purposes only.

AI-generated answers may not be fully accurate — always verify with official documents.

Do not upload sensitive or confidential PDFs.

## ✨ Features

📂 Upload any PDF at runtime using Colab file picker.

✂️ Split documents into smaller chunks for better embeddings.

🔍 Generate BAAI/bge-large-en-v1.5 embeddings and store them in a Chroma vector store.

🤖 Use Mistral-7B-Instruct (via Hugging Face Inference API) for LLM-powered Q&A.

⚡ Perform semantic search to retrieve relevant chunks.

🖥️ Ask questions via an interactive Gradio web interface.

📑 Returns answers with source references.

## 🚀 How to Use (Colab)

Open the notebook in Google Colab.

Add your Hugging Face API key in Colab Secrets:

Go to Tools → Settings → Secrets

Add key: HF_API_KEY

Value: <Your Hugging Face API key>

Upload your PDF when prompted by the file picker.

Run the notebook cells step by step:

Connect to Hugging Face API

Load PDF

Split text into chunks

Create embeddings & vector store

Build the RAG QA chain

Launch the Gradio interface

Ask questions about your uploaded PDF using the interface 🎉

## 💡 Example Questions

What is the company’s policy on remote work?

How do I request vacation time?

What benefits are available to employees?

## 📝 Notes

Works for any text-based PDF, not tied to a specific file.

Scanned PDFs (images) are not supported without OCR.

The pipeline can be adapted for finance, legal, technical manuals, academic papers, etc.

## 📦 Dependencies

`langchain`

`langchain_community`

`chromadb`

`gradio`

`sentence-transformers`

`pypdf or pymupdf (for PDF parsing)`
