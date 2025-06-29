# 🤖 RAG-based Customer Complaint Chatbot with API Integration

This project is an intelligent chatbot application that allows users to file and track customer complaints via natural language, powered by **LangChain**, **FastAPI**, **Streamlit**, and **Hugging Face embeddings**. It also uses **Retrieval-Augmented Generation (RAG)** to answer FAQs from a customer service knowledge base.

---

## 📌 Features

- 🧠 **RAG-based QA**: Answers from a PDF knowledge base using ChromaDB + Hugging Face embeddings
- 🗣️ **Conversational Complaint Filing**: Interactive chatbot collects user details and files a complaint
- 🆔 **Complaint Tracking**: Retrieve complaint status by ID
- 🔐 **REST API Integration**: FastAPI backend for creating and retrieving complaints
- 📋 **Validation**: Ensures email and phone number formats are correct

---

## 🛠️ Tech Stack

| Layer         | Technology                                                                   |
|---------------|------------------------------------------------------------------------------|
| Frontend      | Streamlit                                                                    |
| Backend API   | FastAPI                                                                      |
| Vector Store  | ChromaDB                                                                     |
| Embeddings    | all-MiniLM-L6-v2 via Hugging Face                                            |
| LLM           | ChatGroq (`llama3-70b-8192`) integrated via LangChain                        |
| Database      | SQLite                                                                       |
| PDF Parsing   | PyPDFLoader from `langchain_community.document_loaders`                     |

---

📦 rag-chatbot-complaint-creation
├── backend.py                       # FastAPI backend with complaint API
├── run.py                           # Streamlit chatbot app
├── complaints.db                    # SQLite database (auto-generated)
├── Customer_Service_Knowledge_Base.pdf
├── requirements.txt
└── README.md

