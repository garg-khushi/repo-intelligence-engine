# Repo Intelligence Engine

An LLM-powered system for understanding, exploring, and querying software repositories using retrieval-augmented generation (RAG).

This project enables users to ask natural language questions about a codebase and receive context-grounded answers by combining document ingestion, embeddings, vector search, and conversational reasoning.

---

## 🚀 What This Project Does

- Clones a public GitHub repository
- Parses source files and documentation
- Splits code into semantic chunks
- Generates vector embeddings
- Stores embeddings in a vector database
- Enables conversational Q&A grounded in repository context

This allows questions such as:
- *"What does this project do?"*
- *"How is authentication handled?"*
- *"Where is the main training loop defined?"*
- *"Explain the data flow in this codebase."*

---

## 🧠 System Architecture

```
GitHub Repo
↑
↑
File Loader & Parser
↑
Text Chunking
↑
Embedding Model
↑
Vector Store (Chroma)
↑
Retriever
↑
LLM (Conversational QA)
↑
Streamlit UI
```

---

## 🛠️ Tech Stack

| Layer | Technology |
|-----|----------|
| Language | Python |
| UI | Streamlit |
| LLM | OpenAI GPT models |
| Framework | LangChain |
| Embeddings | OpenAI Embeddings |
| Vector Store | Chroma |
| Version Control | Git |

---

## 📂 Repository Structure

```
.
├── app_updated.py              # Main Streamlit application
├── requirements.txt           # Python dependencies
├── Projreport_OpenAI.docx    # Project report and documentation
└── data/                       # Vector store persistence (generated)
```

---

## 🔬️ What's Implemented

- ✅ GitHub repository cloning
- ✅ File loading and preprocessing
- ✅ Chunk-based embedding generation
- ✅ Vector search using Chroma
- ✅ Conversational retrieval QA
- ✅ Interactive Streamlit interface

---

## ⚠️ Scope & Limitations

- Designed for **demonstration and experimentation**
- Not optimized for very large repositories
- Embedding persistence is local
- Security hardening and sandboxing are out of scope

This project intentionally prioritizes **clarity and correctness** over production scaling.

---

## 😧 Planned Enhancements

- Per-repository isolated vector stores
- Language-aware file parsing
- Support for multiple embedding models
- Repository summarization and dependency graphs
- Deployment-ready API layer (FastAPI)

---

## 👨‍💻 How to Run Locally

```bash
git clone https://github.com/garg-khushi/repo-intelligence-engine.git
cd repo-intelligence-engine
pip install -r requirements.txt
streamlit run app_updated.py
```

Create a `.env` file with:
```
OPENAI_API_KEY=your_api_key_here
```

---

## 🎯 Why This Project Matters

This project demonstrates:
- Practical use of LLMs beyond chat
- Retrieval-augmented generation pipelines
- Vector databases and semantic search
- Developer tooling and code intelligence systems

It reflects real-world patterns used in modern AI-powered developer platforms.

---

## 📃 License

MIT
