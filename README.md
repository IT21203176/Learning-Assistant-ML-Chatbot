# CTSE Lecture Notes Chatbot 🤖  
**LLM Development Toolkit – Building a RAG-based Academic Chatbot**

---

## 📌 Overview  
This project demonstrates the development of a **Retrieval-Augmented Generation (RAG)** based chatbot capable of answering questions from **CTSE (Current Trends in Software Engineering)** lecture notes.

The chatbot is implemented inside a **Jupyter Notebook** using **LangChain**, **Gemini 1.5 Flash** (Google Generative AI), and **FAISS** for semantic search. The objective is to build a lightweight, efficient, and context-aware assistant that retrieves relevant content from lecture notes and provides accurate answers.

---

## ✨ Features  

- **PDF Ingestion** – Load CTSE lecture notes using **PyPDFLoader**  
- **Text Chunking** – Split documents into manageable chunks for semantic search  
- **Embeddings** – Generate high-dimensional vector representations using **Gemini Embedding-001**  
- **Semantic Search** – Use **FAISS** to retrieve the most relevant content efficiently  
- **LLM-powered Q&A** – Integrate **Gemini 1.5 Flash** via **LangChain**’s `RetrievalQA` chain  
- **Modular Design** – Easy to extend with more documents or swap in a different LLM  
- **Interactive Querying** – Real-time question answering inside Jupyter Notebook  

---

## System Architecture  

The chatbot follows a modular **RAG pipeline**:

1. **Import Libraries**   
2. **Load Lecture Notes** (via `PyPDF`)  
3. **Split Text into Chunks** (`CharacterTextSplitter`)  
4. **Generate Embeddings** (`Gemini Embedding-001`)  
5. **Store Vectors** in **FAISS Vector DB**  
6. **Retrieve Relevant Chunks** based on user queries  
7. **LLM Integration** with **Gemini 1.5 Flash**  
8. **Generate Context-aware Answers**  

---

## 🚀 Tech Stack  

| Component      | Technology / Library     | Purpose                     |
|---------------|---------------------------|-----------------------------|
| **LLM**       | Gemini 1.5 Flash         | Answer generation          |
| **Framework** | LangChain                | Orchestrating RAG pipeline |
| **Vector DB** | FAISS                    | Semantic search & retrieval |
| **Embeddings**| Gemini Embedding-001     | Convert text to vectors    |
| **PDF Loader**| PyPDFLoader              | Read and parse lecture notes |
| **Environment** | Jupyter Notebook      | Development & testing      |



