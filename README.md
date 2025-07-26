# RAG with LangChain, OpenAI, and FAISS

A Retrieval-Augmented Generation (RAG) system built with LangChain, OpenAI GPT models, and FAISS vector database for intelligent document querying and question answering.

## 🚀 Overview

This project implements a RAG pipeline that processes PDF documents, creates embeddings using HuggingFace models, stores them in a FAISS vector database, and uses OpenAI's GPT models to provide intelligent answers based on the retrieved context.

## 🛠️ Tech Stack

- **Python 3.13.5**
- **LangChain** - Framework for building applications with LLMs
- **OpenAI GPT-3.5-turbo** - Large Language Model for text generation
- **FAISS** - Facebook AI Similarity Search for vector storage and retrieval
- **HuggingFace Transformers** - Embeddings model (BAAI/bge-small-en-v1.5)
- **PyPDF** - PDF document processing
- **Sentence Transformers** - Text embedding utilities
- **Python-dotenv** - Environment variable management

## 📋 Features

- **PDF Document Processing**: Automatically loads and processes PDF documents
- **Intelligent Text Chunking**: Splits documents into optimal chunks for retrieval
- **Vector Embeddings**: Uses state-of-the-art HuggingFace embeddings
- **Semantic Search**: FAISS-powered similarity search for relevant context retrieval
- **GPT-Powered Responses**: Leverages OpenAI's GPT-3.5-turbo for intelligent answers
- **Configurable Prompts**: Customizable prompt templates for different use cases

## 📊 Performance Considerations

- **Chunk Size**: Smaller chunks (512 tokens) provide more precise retrieval but may lack context
- **Embedding Model**: BAAI/bge-small-en-v1.5 offers good performance with reasonable speed
- **Vector Store**: FAISS provides fast similarity search for moderate-sized document collections

### Example Queries

```python
# Query the document
response = rag_chain.invoke("What is the business strategy of Nike?")
print(response)
```

## 👨‍💻 Author

**Chirag Singhvi**
- Email: csinghvi15@gmail.com
- GitHub: [@chiragsinghvi01](https://github.com/chiragsinghvi01)
