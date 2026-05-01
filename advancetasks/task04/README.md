# Context-Aware Chatbot using Sentence Transformers and FAISS

## Overview

This project implements a simple **RAG-style (Retrieval-Augmented Generation) Context-Aware Chatbot** using semantic embeddings and vector similarity search.

The chatbot retrieves the most relevant response from a predefined knowledge base based on user queries.

---

## Technologies Used

* Python
* Sentence Transformers
* FAISS
* NumPy
* Gradio

---

## Project Architecture

### Embedding Model

* **Model Used:** all-MiniLM-L6-v2
* Converts documents and user queries into dense vector embeddings

### Vector Database

* **FAISS (Facebook AI Similarity Search)**
* Stores document embeddings for fast similarity retrieval

---

## Knowledge Base

The chatbot uses the following predefined AI/ML knowledge documents:

* Artificial Intelligence definition
* Machine Learning explanation
* Deep Learning overview
* Python for AI/Data Science
* Data Science explanation

---

## How It Works

1. Convert documents into embeddings
2. Store embeddings in FAISS index
3. Convert user query into embedding
4. Perform similarity search
5. Retrieve most relevant document
6. Return matched answer

---

## Gradio Interface

Interactive web UI allows users to:

* Ask AI/Data Science related questions
* Receive context-aware retrieved responses instantly

---

## How to Run

### Install Dependencies

```bash id="xk5m9w"
pip install sentence-transformers faiss-cpu gradio
```

### Run Project

```bash id="r5mh4k"
python rag_chatbot.py
```

---

## Sample Query

Input:

```text id="l7u5sv"
What is machine learning?
```

Output:

```text id="u2lsik"
Answer: Machine Learning is a subset of AI that learns patterns from data.
```

---

## Project Workflow

1. Define Knowledge Base
2. Generate Document Embeddings
3. Store in FAISS Vector Index
4. Accept User Query
5. Retrieve Most Similar Context
6. Return Relevant Response

---

## Future Improvements

* Expand knowledge base dynamically
* Use top-k retrieval instead of single result
* Integrate with LLM for generative answers
* Connect to external documents/PDFs
* Deploy on Hugging Face Spaces

---

## Author

Arfa Imran
