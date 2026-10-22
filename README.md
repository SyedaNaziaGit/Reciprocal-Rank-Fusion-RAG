# Reciprocal-Rank-Fusion-RAG

## RAG Fusion Pipeline
This notebook demonstrates a complete RAG (Retrieval-Augmented Generation) pipeline built on top of our custom RAGFusion class. The pipeline uses LLM-generated sub-queries to improve retrieval quality, then fuses the results using Reciprocal Rank Fusion (RRF).

Steps covered:

Load the source PDF
Split documents into chunks
Generate embeddings and store in ChromaDB
Create a similarity-search retriever
Apply RAG Fusion (sub-query generation + RRF)
Augmentation - build context from retrieved documents
Generation - produce a grounded answer using an LLM
