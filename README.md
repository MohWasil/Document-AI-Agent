# DocumentChat: Multi-Agent RAG System

**DocChat** is an advanced Retrieval-Augmented Generation (RAG) tool designed to extract precise, fact-checked information from long and complex documents. Unlike standard chatbots that struggle with dense text and tables, DocChat utilizes a multi-agent architecture to eliminate hallucinations and ensure document-grounded accuracy.

---

### Estimated Setup Time: 60 Minutes

## Overview
Standard LLMs like ChatGPT or DeepSeek often struggle with long-form documents, frequently misinterpreting tables or fabricating citations (hallucinations). **DocChat** solves this by moving away from a single-model approach. It employs a team of specialized AI agents to retrieve, analyze, and verify data before presenting it to the user.

## Key Features
*   **Hybrid Retrieval:** Combines **BM25 keyword search** and **vector embeddings** to find the needle in the haystack.
*   **Multi-Agent Workflow:**
    *   **Research Agent:** Analyzes content and generates initial responses.
    *   **Verification Agent:** Cross-checks claims against the source to flag hallucinations.
    *   **Self-Correction:** Automatically re-runs the research step if contradictions are detected.
*   **Multi-Document Support:** Seamlessly query across multiple large files (e.g., 80+ page reports).
*   **Hallucination-Free:** Every response is verified against the original document to ensure factual correctness.
*   **Gradio Interface:** A clean, intuitive UI for easy document uploading and chatting.

## Why DocChat?
In benchmarks involving complex documents (like the *Google 2024 Environmental Report* and *DeepSeek-R1 Technical Report*), DocChat outperformed leading models:
- **vs. DeepSeek:** DocChat reads entire documents where others hit context limits.
- **vs. ChatGPT-4o:** DocChat provides verified data points where others might hallucinate numbers in tables or footnotes.

## What You Will Learn
1.  Building a **Multi-Agent RAG pipeline** using LangGraph.
2.  Implementing **Hybrid Retrieval** (Lexical + Semantic search).
3.  Designing a **Verification Pipeline** to detect and fix AI hallucinations.
4.  Deploying a functional AI app with **Gradio**.

## Tech Stack
- **Orchestration:** [LangGraph](www.langchain.com) / [LangChain](www.langchain.com)
- **Retrieval:** BM25 & Vector Databases
- **UI:** [Gradio](www.gradio.app)
- **LLM:** Integration with high-reasoning models for agentic tasks

## Prerequisites
- Python 3.9+ < 3.11
- API Keys for your chosen LLM provider (e.g., OpenAI, Anthropic, or DeepSeek)

## Installation & Setup

1. **Clone the repository:**
   ```bash
   git clone github.com
   cd DocChat
