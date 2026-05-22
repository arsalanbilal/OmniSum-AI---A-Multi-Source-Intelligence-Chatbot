# OmniSum AI – Multi-Source Intelligence Chatbot

OmniSum AI is a multi-source intelligence chatbot built to help users ask questions across different types of data from a single interface. It combines Python, LangChain, Ollama-style LLM workflows, Hybrid RAG, reranking, and Streamlit to deliver grounded answers from uploaded files and web content.

## Overview

The goal of OmniSum AI is to reduce the time users spend manually searching through documents, spreadsheets, text files, and web pages. Instead of reading each source separately, users can upload or connect content and ask natural-language questions to receive context-aware answers with source-backed responses.

## Key Features

- Multi-source ingestion for PDF, CSV, Excel, text files, and web pages
- Hybrid retrieval using semantic search plus BM25 retrieval
- Query rewriting to improve retrieval quality
- Reranking to prioritize the most relevant context
- Source-grounded responses with supporting excerpts
- Streamlit-based interface for simple and interactive usage

## Tech Stack

- **Language:** Python
- **Frameworks/Libraries:** LangChain, Streamlit
- **LLM Workflow:** Ollama / LLM API integration
- **Retrieval:** Hybrid RAG, BM25, Vector Search
- **Embeddings & Vector Store:** Hugging Face Embeddings, FAISS
- **Document Processing:** PyPDFLoader, CSVLoader, UnstructuredExcelLoader, TextLoader, WebBaseLoader

## How It Works

1. The user uploads a file or provides a web URL.
2. The application extracts content from the selected source.
3. The extracted text is split into chunks for retrieval.
4. Embeddings are created and stored in a FAISS vector index.
5. A hybrid retriever combines vector search and BM25 retrieval.
6. The user query is rewritten to improve retrieval effectiveness.
7. Retrieved chunks are reranked to select the most relevant context.
8. The LLM generates a grounded answer using the selected context.
9. The interface displays both the answer and source snippets.

## Use Cases

- Enterprise knowledge assistant for internal documents
- Research summarization across multiple sources
- Document Q&A for reports, notes, and web content
- Fast information retrieval from mixed structured and unstructured data

## Project Impact

- Reduced manual information search by enabling question answering across multiple data sources in one interface
- Improved retrieval quality through the combination of vector search, BM25, query rewriting, and reranking
- Increased trust in generated answers by surfacing supporting source snippets
- Demonstrated end-to-end GenAI application development for real-world document intelligence use cases

## Folder Structure

```bash
OmniSum-AI/
│── app.py
│── requirements.txt
│── README.md
```

## Installation

```bash
git clone <your-repository-url>
cd OmniSum-AI
pip install -r requirements.txt
streamlit run app.py
```

## Example Resume Description

**OmniSum AI – Multi-Source Intelligence Chatbot**

Built a multi-source intelligence chatbot using Python, LangChain, Ollama LLM, Hybrid RAG, BM25, reranking, and Streamlit. Enabled question answering across PDFs, CSVs, Excel files, text files, and web pages through retrieval orchestration and source-grounded responses.

## Current Status

This project is a strong portfolio-level GenAI application and demonstrates practical understanding of multi-source RAG pipelines. It is suitable for showcasing on a resume, GitHub, and LinkedIn as a fresher-level flagship project.

## Future Improvements

- Add production-grade reranking with cross-encoder or hosted rerank APIs
- Add stronger metadata-based citations such as file name, page number, and URL tracking
- Improve caching and indexing strategy for larger datasets
- Add evaluation metrics for retrieval quality and answer relevance
- Add deployment hardening, logging, and monitoring for production environments

## Author

**Arsalan Bilal**  
LinkedIn: https://linkedin.com/in/contactarsalanbilal  
GitHub: https://github.com/arsalanbilal
