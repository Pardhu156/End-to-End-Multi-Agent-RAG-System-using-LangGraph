# End-to-End Multi-Agent RAG System using LangGraph, Llama & Astra DB

An end-to-end **stateful Multi-Agent Retrieval-Augmented Generation (RAG)** system built using **LangGraph** for orchestration and **Llama** as the reasoning engine.

The system implements **hybrid retrieval** through:

-  **Wikipedia Search Agent** → External real-time knowledge retrieval  
-  **Astra DB Vector Retrieval Agent** → Internal semantic search over embedded documents  

This project demonstrates production-style GenAI architecture using multi-agent workflows, vector databases, and conditional graph execution.

---

##  Key Features

- Stateful multi-agent orchestration using **LangGraph**
- Hybrid retrieval (External + Vector Database)
- Vector similarity search using **Astra DB (Cassandra)**
- Embedding pipeline using **MiniLM**
- LLM-powered query routing and response synthesis
- Modular, extensible architecture

---

## Internal Knowledge Base (Astra DB)

Internal knowledge such as:
- RAG concepts
- LangGraph workflows
- Agent architecture documentation

is processed through:

1. Document ingestion  
2. Recursive text chunking  
3. Embedding generation using **MiniLM**  
4. Vector storage in **Astra DB (Cassandra-based Vector Database)**  
5. Top-k similarity retrieval during query execution  

This enables scalable, low-latency semantic search.

---

## 🛠️ Tech Stack

- Python  
- LangChain  
- LangGraph  
- Llama (LLM)  
- Astra DB (Cassandra Vector Database)  
- HuggingFace MiniLM (sentence-transformers)  
- Wikipedia API  
- python-dotenv  
