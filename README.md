# RAG Chatbot Project 🚀

[![Python Version](https://img.shields.io/badge/python-3.11-blue)](https://www.python.org/)
[![React Version](https://img.shields.io/badge/react-vite-green)](https://vitejs.dev/)
[![License](https://img.shields.io/badge/license-MIT-green)](LICENSE)

A **Retrieval-Augmented Generation (RAG)** chatbot using **Python 3.11**, **Flan-T5**, **ChromaDB**, and a **React Vite** frontend.  
Users can upload multiple document types (PDF, DOCX, CSV, TXT), extract knowledge, and ask questions based on uploaded content. Answers are strictly grounded in the documents.

---

## Features

- Upload multiple files (PDF, DOCX, CSV, TXT)
- Automatic text extraction and chunking
- Vector database (ChromaDB) for efficient similarity search
- Flan-T5 based question answering
- Session-based chat history saving
- React Vite frontend for interactive UI
- Supports multiple concurrent users

---

## Tech Stack

- **Backend:** Python 3.11, FastAPI
- **Frontend:** React + Vite
- **Vector Database:** ChromaDB
- **Embedding Model:** `sentence-transformers/all-MiniLM-L6-v2`
- **LLM:** `google/flan-t5-base`
- **Database:** Optional (SQLite) for chat history

---

## Installation & Run Commands

### Backend


# 1. Create virtual environment
python -m venv myvenv
source myvenv/bin/activate  # Linux/Mac
myvenv\Scripts\activate     # Windows

# 2. Install dependencies
pip install --upgrade pip
pip install -r backend/requirements.txt

# 3. Run backend server
cd backend
uvicorn app.main:app --reload


---

## Installation & Run Commands

### Frontend


# 1. Navigate to frontend folder
cd frontend

# 2. Install dependencies
npm install

# 3. Run frontend dev server
npm run dev
