# RAG-Based Document Question Answering System

A **Retrieval-Augmented Generation (RAG)** based Document Question Answering system that enables users to ask natural language questions over documents and receive accurate, context-aware answers using **semantic search** and **Large Language Models (LLMs)**.

This project demonstrates a **real-world RAG pipeline** combining document ingestion, vector similarity search, and LLM-powered answer generation, suitable for AI-powered search engines and enterprise knowledge assistants.

---

## 📌 Overview

Traditional LLMs may hallucinate or provide outdated information.  
This system solves that by **retrieving relevant document context first** and then generating answers grounded in actual data.

**Key idea:**  
> *Retrieve first → Generate second*

---

## 🚀 Key Features

- 📄 Document ingestion and preprocessing
- 🔍 Semantic search using vector embeddings
- 🧠 Retrieval-Augmented Generation (RAG) architecture
- 🤖 LLM-powered answer generation
- 📊 JSON-based input/output handling
- 📝 Logging for debugging and traceability
- 🧩 Modular and extensible Python codebase
- ⚙️ Shell-based deployment support

---

## 🏗️ Architecture

```

User Question
↓
Vector Embedding
↓
Semantic Retriever
↓
Relevant Document Context
↓
LLM (GPT-based)
↓
Final Answer

```

---

## 🧰 Tech Stack

- **Language:** Python
- **LLM Integration:** GPT-based client
- **Vectorization:** Embedding-based semantic search
- **Data Formats:** JSON
- **Deployment:** Shell scripting
- **Version Control:** Git & GitHub

---

## 📂 Project Structure

```

rag-based-document-qa/
│
├── app.py                 # Application entry point
├── main.py                # Core execution flow
├── document_loader.py     # Document ingestion & preprocessing
├── vectorizer.py          # Embedding generation logic
├── retriever.py           # Semantic similarity search
├── gpt_client.py          # LLM interaction
├── submitter.py           # Output handling
├── deploy.sh              # Deployment helper script
├── requirements.txt       # Python dependencies
├── questions.json         # Sample input questions
├── answers_output.json    # Generated answers
├── log.txt                # Execution logs
└── README.md

````

---

## ▶️ How to Run the Project

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/Debasish-87/rag-based-document-qa.git
cd rag-based-document-qa
````

### 2️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

### 3️⃣ Configure LLM Access

* Add your API key inside `gpt_client.py`
* Or configure environment variables as required

### 4️⃣ Run the Application

```bash
python app.py
```

### 5️⃣ View Results

* Generated answers → `answers_output.json`
* Logs → `log.txt`

---

## 📌 Sample Workflow

1. Load documents
2. Chunk and vectorize content
3. Accept user questions from JSON
4. Retrieve relevant context using semantic similarity
5. Generate grounded answers via LLM
6. Store output for analysis

---

## 🧪 Use Cases

* 📚 Enterprise document Q&A
* 🔍 AI-powered knowledge search
* 📄 Research paper analysis
* 🏢 Internal documentation assistants
* 🤖 Chatbots with document grounding

---

## 🔐 Security & Limitations

* API keys must be kept secure (never commit secrets)
* Designed for learning and demonstration purposes
* Can be extended with production-grade vector databases

---

## 🚧 Future Enhancements

* FAISS / Pinecone / ChromaDB integration
* Web-based UI (FastAPI / Streamlit)
* Support for PDF, DOCX, and HTML documents
* Authentication & access control
* Performance optimization for large datasets

---

## 👨‍💻 Contributors

* **Debasish Mohanty** – Core development & architecture
* **Rudra Prasad Jena** – Collaboration & contributions
* **Srujan Rana** – Feature enhancements

---

## 📜 License

This project is licensed under the **MIT License**.

---

