<div align="center">

# 📚 Document RAG AI Knowledge Assistant

### 🚀 Advanced Retrieval-Augmented Generation (RAG) System Built with n8n + OpenAI

<img src="https://img.shields.io/badge/n8n-AI%20Automation-orange?style=for-the-badge&logo=n8n" />
<img src="https://img.shields.io/badge/OpenAI-GPT--4o-green?style=for-the-badge&logo=openai" />
<img src="https://img.shields.io/badge/RAG-Vector%20Search-blue?style=for-the-badge" />
<img src="https://img.shields.io/badge/AI-Knowledge%20Assistant-purple?style=for-the-badge" />
<img src="https://img.shields.io/badge/Status-Active-success?style=for-the-badge" />

---

### 🧠 Chat with Your Own Documents Using AI

Instead of generating generic AI responses, this assistant retrieves answers directly from uploaded documents — creating a **private AI knowledge base** powered by semantic search and vector embeddings.

</div>

---

# 🌟 Overview

This project is an advanced **RAG (Retrieval-Augmented Generation)** implementation built entirely in **n8n** using:

- 🤖 OpenAI GPT Models
- 🧠 Embedding-based Semantic Search
- 📚 Vector Database Retrieval
- 🔍 Knowledge Grounding
- 💬 Conversational Memory
- 📄 PDF & Document Processing

The system allows users to upload their own documents and interact with them like a personalized ChatGPT.

---

# 🔥 Features

## ✅ AI-Powered Knowledge Assistant

- Upload PDFs, notes, resumes, policies, and documents
- Convert documents into searchable embeddings
- Retrieve relevant knowledge using semantic search
- Generate accurate AI responses from uploaded content

---

## ✅ Hallucination Reduction

Unlike normal AI chatbots:

✔ Answers are generated ONLY from uploaded knowledge  
✔ Prevents random hallucinated responses  
✔ Uses retrieval-based context injection  

---

## ✅ Conversational Memory

Supports:

- Follow-up questions
- Context retention
- Multi-turn conversations
- AI memory handling

---

## ✅ Fully Automated RAG Pipeline

The entire workflow is automated using n8n.

From ingestion → embeddings → retrieval → AI response.

---

# 🧠 What is RAG?

## Retrieval-Augmented Generation (RAG)

RAG combines:

```text
Information Retrieval
        +
Vector Search
        +
Large Language Models
```

This allows AI systems to retrieve real knowledge before generating responses.

Instead of relying only on pretrained data, the AI can answer questions using YOUR uploaded documents.

---

# 📂 Repository Structure

```text
document-rag-n8n/
│
├── DATA INGESTION.json
├── searchable knowledge base.json
└── README.md
```

---

# ⚙️ Workflows Included

# 1️⃣ DATA INGESTION Workflow

## Purpose

Processes uploaded documents and prepares them for semantic search.

---

## Responsibilities

✅ Extract text from PDFs/documents  
✅ Split text into chunks  
✅ Generate OpenAI embeddings  
✅ Store vectors in vector database  
✅ Build searchable knowledge base  

---

## Technologies Used

| Technology | Purpose |
|---|---|
| OpenAI Embeddings | Semantic Search |
| PDF Extraction | Document Parsing |
| Text Chunking | RAG Preparation |
| Vector Database | Knowledge Storage |
| n8n | Workflow Automation |

---

# 2️⃣ Searchable Knowledge Base Workflow

## Purpose

Handles user questions and retrieves relevant knowledge using AI.

---

## Responsibilities

✅ Accept user queries  
✅ Generate query embeddings  
✅ Perform semantic search  
✅ Retrieve relevant chunks  
✅ Inject context into GPT  
✅ Generate grounded AI responses  
✅ Maintain conversation memory  

---

## Technologies Used

| Technology | Purpose |
|---|---|
| GPT-4o Mini | Response Generation |
| Semantic Search | Knowledge Retrieval |
| AI Agent | Intelligent Responses |
| Memory | Follow-up Conversations |
| Prompt Engineering | Hallucination Reduction |

---

# 🧩 Complete System Architecture

```text
                ┌────────────────────┐
                │   User Uploads     │
                │     Documents      │
                └─────────┬──────────┘
                          │
                          ▼
                ┌────────────────────┐
                │  PDF/Text Extract  │
                └─────────┬──────────┘
                          │
                          ▼
                ┌────────────────────┐
                │   Text Chunking    │
                └─────────┬──────────┘
                          │
                          ▼
                ┌────────────────────┐
                │ OpenAI Embeddings  │
                └─────────┬──────────┘
                          │
                          ▼
                ┌────────────────────┐
                │   Vector Database  │
                └─────────┬──────────┘
                          │
                          ▼
                ┌────────────────────┐
                │    User Question   │
                └─────────┬──────────┘
                          │
                          ▼
                ┌────────────────────┐
                │  Semantic Search   │
                └─────────┬──────────┘
                          │
                          ▼
                ┌────────────────────┐
                │ Relevant Context   │
                └─────────┬──────────┘
                          │
                          ▼
                ┌────────────────────┐
                │   GPT-4o Response  │
                └────────────────────┘
```

---

# 💡 Use Cases

## 📄 Resume Assistant

Ask questions about uploaded resumes.

Example:
```text
"Summarize this candidate's experience"
```

---

## 🏢 Company Policy Assistant

Search and retrieve answers from internal company policies.

Example:
```text
"What is the leave policy?"
```

---

## 🎓 Student Notes Assistant

Chat with educational notes and study materials.

Example:
```text
"Explain chapter 4 in simple terms"
```

---

## 📚 Research Assistant

Interact with research papers and technical documentation.

Example:
```text
"What are the main findings?"
```

---

## 🧠 Personal Knowledge Base

Create your own private AI assistant trained on your data.

---

# 🛠 Tech Stack

<div align="center">

| Technology | Usage |
|---|---|
| n8n | Workflow Automation |
| OpenAI API | AI Processing |
| GPT-4o Mini | AI Responses |
| OpenAI Embeddings | Semantic Search |
| Vector Database | Knowledge Storage |
| RAG Architecture | Retrieval Pipeline |
| AI Agent | Intelligent Querying |
| Memory | Context Retention |
| PDF Extraction | Document Parsing |

</div>

---

# 📥 Setup Instructions

# Step 1 — Clone Repository

```bash
git clone https://github.com/yourusername/document-rag-n8n.git
```

---

# Step 2 — Import Workflows into n8n

Import:

```text
DATA INGESTION.json
searchable knowledge base.json
```

---

# Step 3 — Configure Credentials

Add your:

- OpenAI API Key
- Vector Database Credentials
- Storage Credentials

---

# Step 4 — Run Data Ingestion

Upload your documents and execute:

```text
DATA INGESTION.json
```

This workflow will:

✅ Extract text  
✅ Generate embeddings  
✅ Store vectors  

---

# Step 5 — Start Chatting

Execute:

```text
searchable knowledge base.json
```

Ask questions about your uploaded documents.

---

# 🔐 Security

## This repository does NOT contain:

❌ API Keys  
❌ Secrets  
❌ Tokens  
❌ Credentials  

Please configure your own credentials inside n8n.

---

# 🎯 Key Learnings

This project helped me understand:

✅ Retrieval-Augmented Generation (RAG)  
✅ Embedding-based search systems  
✅ Vector databases  
✅ Prompt engineering  
✅ AI workflow orchestration  
✅ Context-aware AI agents  
✅ Hallucination reduction techniques  
✅ Semantic retrieval pipelines  
✅ Conversational memory systems  

---

# 🚀 Future Improvements

- Multi-document collections
- Hybrid search
- OCR support
- Metadata filtering
- Multi-user authentication
- Web UI integration
- Streaming responses
- Local embedding models
- Advanced vector databases
- Multi-agent workflows

---

# 📸 Project Vision

> Building AI is not only about chatbots.
>
> It’s about giving AI:
>
> - the right knowledge,
> - the right memory,
> - and the right context.

This project represents another step in my journey as a **BTech CSE student building real-world AI systems** using automation and generative AI.

---

# ⭐ Support

If you found this project useful:

⭐ Star the repository  
🍴 Fork the project  
🚀 Contribute improvements  
💬 Share feedback  

---

<div align="center">

# 🚀 Let's Build Smarter AI Systems Together

</div>

---

# 📜 License

MIT License
