# 🏥 Clinical Decision Support System using RAG

## 📌 Overview

This project implements a **Retrieval-Augmented Generation (RAG)** based Clinical Decision Support System using **LLaMA-2** and medical information from the **Merck Manuals**.

The system retrieves relevant medical information from a vector database and uses it as context to generate more grounded responses.

## 🎯 Objectives

* Build a medical Q&A system using LLaMA-2.
* Implement RAG for medical knowledge retrieval.
* Compare **Baseline LLaMA-2** vs **RAG-based LLaMA-2**.
* Evaluate responses based on **Groundedness** and **Relevance**.

## 🔄 Workflow

```text
Medical Query
     ↓
ChromaDB Retriever
     ↓
Relevant Medical Documents
     ↓
LLaMA-2 13B
     ↓
Final Response
```

## 🛠️ Technologies

* Python
* LLaMA-2 13B
* LangChain
* ChromaDB
* Hugging Face
* Sentence Transformers
* MiniLM-L6-v2
* PyMuPDF
* Pandas

## 📚 Knowledge Base

**Merck Manuals** medical documentation is used as the knowledge source. The documents are chunked, converted into embeddings, and stored in ChromaDB for semantic retrieval.

## 📊 Evaluation

The project compares baseline and RAG responses using an **LLM-as-a-Judge** approach for:

* Groundedness
* Relevance

This project is an **educational/research prototype** and should not be used as a replacement for professional medical advice or clinical decision-making.

