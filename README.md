<div align="center">

# 🧠 RAG PDF Chatbot  
### *A Context-Aware Document Q&A System powered by LangChain, ChromaDB, and Llama 3.*

![Python](https://img.shields.io/badge/Python-3.10+-blue.svg)
![LangChain](https://img.shields.io/badge/LangChain-Framework-green)
![LLM](https://img.shields.io/badge/Model-Llama--3.3--70B--Versatile-purple)
![License](https://img.shields.io/badge/License-MIT-yellow)
![Chroma](https://img.shields.io/badge/VectorDB-ChromaDB-orange)
![SentenceTransformers](https://img.shields.io/badge/SentenceTransformers-all--MiniLM--L6--v2-blueviolet)
![Embeddings](https://img.shields.io/badge/Embeddings-Semantic_Search-green)

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

<img width="1582" height="987" alt="RAG 1 " src="https://github.com/user-attachments/assets/e5c7e04f-cc70-4c27-861c-ac5751a747d4" />
<img width="1577" height="995" alt="RAG 2" src="https://github.com/user-attachments/assets/ea1ca742-9969-4502-aaec-989d13144421" />
<img width="1578" height="988" alt="RAG 3" src="https://github.com/user-attachments/assets/b2f74f31-3e2f-4d04-976a-4a989d22f1a5" />
<img width="1583" height="991" alt="RAG 4" src="https://github.com/user-attachments/assets/bfa35796-1985-4fb2-a342-313d335a3aeb" />
<img width="1578" height="987" alt="RAG 5" src="https://github.com/user-attachments/assets/9d42bdd4-3009-467a-9ee0-9accde36690e" />

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








