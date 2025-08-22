# AI-Powered PDF Question Answering (RAG Pipeline)

A general-purpose Retrieval-Augmented Generation (RAG) pipeline that lets you ask natural-language questions about any PDF document.

Built with:

Mistral-7B-Instruct (LLM)

BAAI/bge-large-en-v1.5 (Embeddings)

LangChain + ChromaDB (Vector Search)

Gradio (Interactive UI)

Designed to run seamlessly on Google Colab 🚀.

## ⚠️ Disclaimer

Add your Hugging Face API key first in Colab Secrets or as an environment variable (HF_API_KEY).

This notebook is for educational/demo purposes only.

Answers are AI-generated — always verify with official documents.

❌ Do not upload confidential or sensitive PDFs.

## ✨ Features

📂 Upload any PDF at runtime via Colab file picker.

✂️ Automatic text chunking for efficient embeddings.

🔍 Semantic search powered by BGE embeddings.

🤖 LLM Q&A with Mistral-7B-Instruct (via Hugging Face Inference API).

📑 Answers include source references for transparency.

🖥️ Interactive Gradio web app for easy question-asking.

## 🚀 How to Use (Google Colab)

Open the notebook in Google Colab.

Add your Hugging Face API key in Colab Secrets:

Go to Tools → Settings → Secrets.

Add key: HF_API_KEY

Value: <your Hugging Face API key>

Upload your PDF when prompted.

Run cells step by step:

✅ Connect to Hugging Face API

📑 Load PDF

✂️ Split text into chunks

🧩 Create embeddings & vector store

🔗 Build the RAG QA chain

🎛️ Launch the Gradio interface

Ask questions about your document 🎉

## 💡 Example Questions

What is the company’s policy on remote work?

How do I request vacation time?

What benefits are available to employees?

Summarize the main points of section 3.

## 📝 Notes

Works for any text-based PDF (not images).

For scanned PDFs, you’ll need OCR (e.g., Tesseract + PyMuPDF).

Can be easily adapted for finance, legal, technical manuals, research papers, and more.

## 📦 Dependencies

`langchain`

`langchain_community`

`chromadb`

`gradio`

sentence-transformers

pypdf or pymupdf (for PDF parsing)
