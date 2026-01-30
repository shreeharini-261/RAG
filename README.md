# 🌍 Global Cooperation Barometer – RAG Chatbot

## 📌 Project Overview
This project implements a **Retrieval-Augmented Generation (RAG) chatbot** system that answers questions about the World Economic Forum’s **"Global Cooperation Barometer 2024"** report. The system extracts insights from the PDF document using natural language queries.

---

## ✨ Features
- **PDF Processing:** Extracts and processes text from the Global Cooperation Barometer 2024 PDF  
- **Vector Database:** Stores document embeddings using ChromaDB with Nomic embeddings  
- **Intelligent Retrieval:** Uses multi-query retrieval to find relevant document chunks  
- **LLM Integration:** Powered by Ollama’s Mistral model for natural language responses  
- **Interactive Q&A:** Chat interface for querying the report content  

---

## 🧰 Technology Stack
- **Document Processing:** LangChain, UnstructuredPDFLoader  
- **Embeddings:** Ollama (nomic-embed-text)  
- **Vector Database:** ChromaDB  
- **LLM:** Ollama (Mistral model)  
- **Framework:** LangChain  

---

## 🔄 How It Works

### 1. Document Processing
- Loads the `WEF_The_Global_Cooperation_Barometer_2024.pdf` file  
- Splits the document into chunks of 7500 characters with 100-character overlap  
- Creates embeddings for each chunk using Nomic embeddings  

### 2. Vector Database Setup
- Stores document chunks and embeddings in ChromaDB  
- Enables semantic search across the document content  

### 3. Query Processing
- Uses multi-query retrieval to generate multiple perspectives on user questions  
- Retrieves relevant document chunks based on semantic similarity  
- Combines retrieved context with the original query  

### 4. Response Generation
- Mistral LLM generates answers based on retrieved context  
- Ensures responses are grounded in the original document  
- Provides detailed explanations of concepts from the report  

---

## 💬 Example Queries
- "What are the 5 pillars of global cooperation?"  
- "Explain each pillar in detail"  
- "What is the current state of global cooperation?"  
- "How does the barometer measure cooperation?"  

---

## 🚀 Key Capabilities
- **Semantic Search:** Finds relevant information even with different phrasing  
- **Multi-Perspective Retrieval:** Generates multiple query variations for better coverage  
- **Context-Aware Responses:** Answers are grounded in the specific report content  
- **Detailed Explanations:** Provides comprehensive answers with supporting details  

---

## 📊 Performance
- Uses Nomic embeddings for efficient similarity search  
- Mistral model provides high-quality, coherent responses  
- Multi-query retrieval improves recall and relevance  

---

## 🎯 Potential Applications
- Research assistance for global cooperation topics  
- Quick reference for report findings  
- Educational tool for understanding global cooperation metrics  
- Policy analysis support  

