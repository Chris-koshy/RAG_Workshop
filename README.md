# My RAG_Workshop

## Topic: NVIDIA Strategy Q&A Bot

## What I changed:

- Documents: Added 5 PDF case studies related to Nvidia Case Study Reports.

- Chunking: Used chunk_size=400 and chunk_overlap=50 for better context retention and summarization.

- Retrieval: Updated retriever settings to search_type="mmr", k=5, fetch_k=15, lambda_mult=0.8 for more relevant and detailed results.

Model Configuration Evaluation: 	
	
	-Two parameter configurations were tested for the RAG model. The first setup — with chunk_size=400, chunk_overlap=50, k=5, fetch_k=15, and lambda_mult=0.8 — consistently produced more accurate and contextually relevant responses compared to the second configuration (chunk_size=1200, chunk_overlap=200, k=7, fetch_k=6, lambda_mult=0.5). Hence, the first set of parameters was adopted as the final configuration for this project.

## How to run:

1. Install requirements: pip install -r requirements.txt

2. Run: python RAG_Workshop_modified.py

## Test questions:

1. What is Nike as a brand known for ?

2. How did Nike use athlete endorsements to strengthen its brand image?

SYSTEM REQUIREMENTS:

Minimum 8GB RAM (16GB recommended for better performance)
At least 20GB free disk space for models and vector databases
Python 3.8+ installed
Stable internet connection for initial model downloads
Ollama installed (https://ollama.ai/)
phi3:mini model downloaded via: ollama pull phi3:mini
INSTALLATION STEPS:

Install Python 3.8+
Install Ollama from https://ollama.ai/
Run: ollama pull phi3:mini
Install required Python packages (see Part 0 below)
Create 'data' folder and add PDF documents

