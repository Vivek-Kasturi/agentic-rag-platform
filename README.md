# 🏥 Agentic RAG System
Agentic Retrieval-Augmented Generation system with multi-source retrieval, relevance grading, and fallback reasoning pipelines.


An Agentic Retrieval-Augmented Generation (RAG) system designed for medical domain question answering using:

- Medical device manuals  
- Medical Q&A dataset  
- Web search fallback  
- Relevance grading  
- Conditional routing  
- Self-correcting answer loop  

This project demonstrates a production-style agentic RAG architecture using structured routing and answer evaluation.

---

## 🚀 Problem Statement

Large Language Models (LLMs) struggle with:

- Domain-specific knowledge  
- Hallucination in medical contexts  
- Outdated information  
- Long document retrieval  

This system addresses these challenges by:

- Retrieving relevant medical documents  
- Grading document relevance  
- Falling back to web search when necessary  
- Evaluating answer quality before final response  

---

## 🏗️ Architecture Overview

The system follows an Agentic RAG workflow:

User Query 
This architecture ensures:

- Reduced hallucination  
- Higher factual accuracy  
- Domain-specific grounding  

---

## 📊 Datasets Used

### 1️⃣ Global Medical Device Manuals Dataset (2025)

**Source:**  
https://www.kaggle.com/datasets/pratyushpuri/global-medical-device-manuals-dataset-2025?resource=download

Used for:

- Technical device documentation retrieval  
- Domain grounding  

---

### 2️⃣ Comprehensive Medical Q&A Dataset

**Source:**  
https://www.kaggle.com/datasets/thedevastator/comprehensive-medical-q-a-dataset

Used for:

- Medical question answering  
- Training retrieval logic  
- Evaluation testing  

---

## 🛠️ Tech Stack

- Python  
- LangGraph  
- LangChain  
- Vector Database (FAISS / Chroma)  
- OpenAI / HuggingFace Embeddings  
- LLM (GPT / open-source LLM)  
- Mermaid Architecture Visualization  

---

## 🧠 Key Features

✔ Multi-source retrieval (Manuals + Q&A)  
✔ Intelligent routing  
✔ Relevance grading  
✔ Web search fallback  
✔ Agentic decision loop  
✔ Architecture visualization  
✔ Reduced hallucination via grounded generation  

---

## ⚙️ How to Run

```bash
git clone https://github.com/Vivek-Kasturi/agentic-rag-platform
cd agentic-rag-platform
pip install -r requirements.txt

  ↓ 
Router (Device vs QnA) 
  ↓ 
Document Retrieval 
  ↓ 
Relevance Check 
  ↓ 
(If relevant) → Augment → Generate 
(If not relevant) → Web Search 
  ↓ 
Answer Evaluation 
  ↓ 
Final Output
```
Create a .env file:
GROQ_API_KEY=your_key_here
TAVILY_API_KEY=your_key_here

Run the notebook
agentic_rag_medical_qa_system.ipynb

📈 Future Improvements
Add hybrid search (BM25 + dense retrieval)

Add reranker model

Add evaluation metrics (Precision@k, Recall@k)

Deploy using FastAPI

Add Streamlit UI

Add medical safety filtering layer

🎯 Why This Project Matters
Medical AI systems require:

Accuracy

Transparency

Grounded responses

Error mitigation

This project demonstrates how Agentic RAG can improve reliability in high-risk domains.

Architecture Diagram
<img width="510" height="732" alt="output" src="https://github.com/user-attachments/assets/77412497-3a21-4afd-9d02-8d473e83581b" />




