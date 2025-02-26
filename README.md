# Multimodal-RAG-for-Text-Image-Table-Extraction

## Overview
This project implements a **Multimodal Retrieval-Augmented Generation (RAG) pipeline** using **Amazon Bedrock, LangChain, and FAISS** to extract and retrieve text, images, and tables from PDFs. The approach enables intelligent question-answering over structured and unstructured document content.

## Features
- Extracts text, images, and tables from PDFs using **PyMuPDF** & **Tabula**.
- Embeds multimodal data with **Amazon Titan Embeddings**.
- Stores and retrieves relevant chunks via **FAISS Vector Database**.
- Generates responses using **Amazon Nova & LangChain**.
- Demonstrated on the *"Attention Is All You Need"* research paper.

## Installation
Clone the repository and install dependencies:
```bash
git clone https://github.com/yourusername/multimodal-rag.git
cd multimodal-rag
pip install -r requirements.txt
```

Dependencies can also be installed in the notebook


## Architecture & Workflow
1. **Extract**: Text, images, and tables are parsed from PDFs.
2. **Embed**: Multimodal embeddings are generated using Amazon Titan.
3. **Store**: FAISS stores vector embeddings for efficient retrieval.
4. **Retrieve**: Relevant chunks are retrieved based on user queries.
5. **Generate**: Amazon Nova generates responses based on retrieved data.

## Example Output
**Query:** *"What is self-attention?"*

**Response:** "Self-attention is a mechanism in the Transformer model that allows each word to focus on other words in a sentence, enabling context-aware representations."



## License & Attribution
- Inspired by the [YouTube Video](https://www.youtube.com/watch?v=jDFpEnJeSVg) on Multimodal RAG.

