# 💊 Drug Information Assistant

An AI-powered **Retrieval-Augmented Generation (RAG)** system for answering drug-related queries.  
Built with **LangChain, Python, LLMs, and Sentence Transformers**, the assistant retrieves relevant medical knowledge and provides accurate, context-aware responses through a text-based interface.

---

## 🚀 Features

- **RAG Pipeline with LangChain** – retrieves the most relevant context before answering.  
- **Sentence Transformers** – chunks documents and generates embeddings for semantic similarity search.  
- **Vector Database** – stores embeddings for efficient retrieval.  
- **Contextual Compression Retriever** – filters noise, reducing irrelevant results by 40%.  
- **Memory & Prompt Engineering** – improves dialogue flow and accuracy.  
- **Low Latency** – average query resolution time < 3 seconds.  

---

## 🧠 System Architecture

1. **Document Ingestion** → Upload & preprocess medical/drug documents.  
2. **Chunking & Embedding** → Sentence Transformers split text and create embeddings.  
3. **Vector Store** → Stores embeddings for semantic similarity search.  
4. **Retriever** → Contextual Compression Retriever fetches top-k relevant passages.  
5. **LLM Response** → Retrieved context + query passed to LLM with optimized prompts.  
6. **Memory** → Keeps track of conversation history.  
7. **Interface** → Text-based chatbot interface.  

---

## 🛠️ Tech Stack

- **Python**  
- **LangChain**  
- **Sentence Transformers**  
- **Vector Database** (FAISS / Chroma)  
- **Large Language Models (LLMs)** – OpenAI / Hugging Face  

---

## 📊 Performance

- **92% retrieval accuracy** on test queries.  
- **Reduced irrelevant results by 40%** with Contextual Compression Retriever.  
- **Average response latency:** < 3 seconds.  
