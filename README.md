# RAG Project

A small Retrieval-Augmented Generation (RAG) project that:
- loads PDF files
- chunks PDF text
- generates embeddings with `sentence-transformers`
- stores vectors in `chromadb`
- retrieves the most relevant chunks for a query
- uses retrieved context for a simple RAG prompt

## Project structure

- `pyproject.toml` — project dependencies and Python settings
- `requirements.txt` — pinned dependency list
- `notebook/document.ipynb` — main pipeline notebook
- `data/pdf/` — source PDF files
- `data/vector_store/` — persistent Chroma vector store

## Prerequisites

- macOS Intel (`x86_64`)
- Python `3.11.x` (recommended)
- `uv` package manager installed
- A valid Groq API key if you want LLM answers via Groq

## Install

```bash
cd /Users/archbutmac/Desktop/RAG
uv add -r requirements.txt
