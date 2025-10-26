<div align="center">

# 🧠 RAG PDF Chatbot  
### *A Context-Aware Document Q&A System powered by LangChain, ChromaDB, and Llama 3.*

![Python](https://img.shields.io/badge/Python-3.10+-blue.svg)
![LangChain](https://img.shields.io/badge/LangChain-Framework-green)
![LLM](https://img.shields.io/badge/Model-Llama--3.3--70B--Versatile-purple)
![License](https://img.shields.io/badge/License-MIT-yellow)
![Chroma](https://img.shields.io/badge/VectorDB-ChromaDB-orange)

</div>

---

## 🌟 Overview  

I’ve worked with **Google Gemini** before, but this marks my **first real hands-on experience with Retrieval-Augmented Generation (RAG)** — and it’s been a fascinating build.  

After a full day of watching videos, experimenting, and debugging, I successfully built a complete **RAG pipeline** that can:  
- Read PDFs 📄  
- Understand their context 🧠  
- Retrieve meaningful chunks 🔍  
- Generate natural, grounded answers 💬  
- And even **remember previous questions** in the same session 🔁  

This project combines **information retrieval + language generation** into a seamless local knowledge assistant that truly understands your data.  

---

## ⚙️ Workflow  

📄 **Read PDF** → ✂️ **Chunk it** → 🔍 **Embed using all-MiniLM-L6-v2 (Sentence Transformer)** → 🧱 **Store in Chroma Vector DB** → 🔁 **Retrieve relevant chunks** → 🤝 **Integrate with LangChain + Llama-3.3-70B-Versatile** → 💬 **User Q&A with session-level memory**

---

## 🧩 What the System Does  

✅ Reads and processes entire PDFs (tested on *Trading for Dummies* and *The Inner Workings of Large Language Models*)  
✅ Splits them into meaningful, overlapping chunks for better context retention  
✅ Generates **semantic embeddings** using Sentence Transformers  
✅ Stores vectors in **ChromaDB** for fast, persistent similarity search  
✅ Integrates with **LangChain** and **Llama 3.3-70B-Versatile** to generate fact-based answers  
✅ Keeps a **chat session memory** — so follow-up questions stay contextual  

🧠 *Essentially, it’s like building your own mini ChatGPT — but powered by your own documents.*

---
## 🧠 Tech Stack  

| Layer | Technology |
|:------|:------------|
| **Document Loader** | LangChain `PyPDFLoader` |
| **Text Splitting** | `RecursiveCharacterTextSplitter` |
| **Embeddings** | `sentence-transformers/all-MiniLM-L6-v2` |
| **Vector Store** | `ChromaDB` |
| **LLM** | `Llama-3.3-70B-Versatile` |
| **Framework** | `LangChain` |
| **Language** | Python 3.10+ |

---

## 🚀 Run Locally  

```bash
# Clone the repo
git clone https://github.com/<your-username>/rag-pdf-chatbot.git
cd rag-pdf-chatbot

# Create a virtual environment
python -m venv .venv
.venv\Scripts\activate   # (Windows)
source .venv/bin/activate   # (Mac/Linux)

# Install dependencies
pip install -r requirements.txt




