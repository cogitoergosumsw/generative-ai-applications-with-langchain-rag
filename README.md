# Generative AI Applications with LangChain and RAG

A comprehensive tutorial project demonstrating how to build Retrieval-Augmented Generation (RAG) applications using LangChain and IBM Watsonx.ai. This project includes both educational Jupyter notebooks and functional Python applications.

## 📚 Project Overview

This repository contains a complete learning path for building RAG applications, from basic document processing to full-stack chatbot implementations. The project is designed to teach the fundamentals of RAG systems through hands-on examples and practical applications.

## 🗂️ Project Structure

### 📖 Educational Notebooks

The project includes several Jupyter notebooks that cover different aspects of RAG development:

- **`LangChain document loader.ipynb`** - Learn how to load documents from various sources (PDF, TXT, JSON, CSV, Word, HTML, etc.)
- **`LangChain text-splitter.ipynb`** - Master text splitting techniques for optimal document chunking
- **`LangChain vector store.ipynb`** - Create and manage vector databases (Chroma, FAISS) for document embeddings
- **`LangChain retriever.ipynb`** - Develop retrievers to fetch relevant document segments based on queries
- **`Embed documents with watsonx s embedding.ipynb`** - Use IBM Watsonx.ai embeddings for document processing
- **`Full document retrieve limitation.ipynb`** - Understand the limitations and challenges of document retrieval

### 🚀 Functional Applications

Two ready-to-use Python applications demonstrate practical RAG implementations:

#### 1. **`qabot.py`** - RAG-based Question Answering System
A complete RAG application that:
- Loads PDF documents using PyPDFLoader
- Splits documents into chunks using RecursiveCharacterTextSplitter
- Creates embeddings using IBM Watsonx.ai (slate-30m-english-rtrvr model)
- Stores embeddings in a Chroma vector database
- Provides a Gradio web interface for document Q&A
- Uses IBM Granite-3-3-8b-instruct model for text generation

#### 2. **`llm_chat.py`** - Simple Chatbot Interface
A basic chatbot that:
- Uses IBM Watsonx.ai models (Mistral Medium or Granite)
- Provides a Gradio web interface for text-based conversations
- Demonstrates direct LLM interaction without RAG

## 🛠️ Technologies Used

- **LangChain** - Framework for building LLM applications
- **IBM Watsonx.ai** - AI platform for foundation models and embeddings
- **Gradio** - Web interface framework for ML applications
- **Chroma** - Vector database for storing embeddings
- **PyPDF2** - PDF document processing
- **Jupyter Notebooks** - Interactive learning environment

## 🎯 Key Learning Objectives

After completing this project, you will be able to:

1. **Document Processing**
   - Load documents from multiple formats (PDF, TXT, JSON, CSV, Word, HTML)
   - Split documents into optimal chunks for processing
   - Handle various document structures and formats

2. **Vector Operations**
   - Create document embeddings using Watsonx.ai
   - Store and manage embeddings in vector databases
   - Perform similarity searches and retrieval

3. **RAG Implementation**
   - Build complete RAG pipelines
   - Implement different retrieval strategies
   - Create question-answering systems

4. **Application Development**
   - Build web interfaces using Gradio
   - Deploy functional RAG applications
   - Integrate multiple AI services

## 🚀 Getting Started

### Prerequisites

- Python 3.8+
- IBM Watsonx.ai account and API credentials
- Jupyter Notebook (for educational content)

### Installation

1. Clone this repository:
```bash
git clone <repository-url>
cd generative-ai-applications-with-langchain-rag
```

2. Install required dependencies:
```bash
pip install langchain langchain-ibm gradio chromadb pypdf2
```

3. Set up your IBM Watsonx.ai credentials:
   - Create an account at [IBM Watsonx.ai](https://watsonx.ai)
   - Configure your project ID and API credentials

### Running the Applications

#### RAG Q&A System
```bash
python qabot.py
```
Access the web interface at `http://localhost:7860`

#### Simple Chatbot
```bash
python llm_chat.py
```
Access the web interface at `http://127.0.0.1:7860`

## 📖 Learning Path

1. Start with the document loader notebook to understand data ingestion
2. Move to text splitting to learn chunking strategies
3. Explore vector stores for embedding management
4. Study retrievers for query processing
5. Practice with the embedding notebooks
6. Build and deploy the functional applications

## 🤝 Contributing

This is an educational project. Feel free to:
- Report issues or bugs
- Suggest improvements
- Add new examples or tutorials
- Enhance documentation

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- IBM Watsonx.ai for providing the AI models and platform
- LangChain team for the excellent framework
- Skills Network for educational content structure

---

**Note**: This project is designed for educational purposes and demonstrates best practices for building RAG applications. Make sure to follow IBM Watsonx.ai usage guidelines and API limits when deploying in production environments.
