# MrHelpMateAI


# Project Name
> Mr HelpMate AI project - Smart Policy Assistant: Implementing a Retrieval Augmented LLM for Life Insurance 


## General Information

In the insurance industry, life insurance policy documents are o en lengthy and complex involving legal 
terminology. This makes it difficult for policyholders to quickly find answers to specific ques ons such as 
eligibility, exclusions, claim procedures, or grace periods. Tradi onal search systems struggle to interpret 
natural language queries. 
Mr.HelpMate AI project aims to implement such a system for life insurance documents. By leveraging 
embedding models, vector databases like ChromaDB, cross-encoder reranking, and OpenAI’s GPT models, the 
system delivers accurate, context-aware answers to user queries. Addi onally, it implements a caching 
mechanism to opmize repeated query performance, improving both response speed and cost efficiency. 

## Objectives

1. Design a Retrieval-Augmented Genera on (RAG) System 
Build a modular, mul-layer architecture (Embedding → Search → Genera on) capable of answering 
user ques ons from a life insurance policy PDF. 
2. Implement Effec ve Embedding 
Experiment with different embedding models (OpenAI & SentenceTransformers) to generate high
quality vector representa ons of the policy document. 
3. Build and Query a Vector Search Index Using ChromaDB 
Store chunk embeddings in ChromaDB and retrieve relevant chunks using seman c similarity for user 
queries. 
4. Implement a Cache-First Query Resolu on Strategy 
Introduce a dual-layer search approach with a fast cache collec on and a fallback full-data search, 
opmizing repeated query performance. 
5. Integrate a Cross-Encoder Re-ranker 
Improve search result accuracy by re-ranking top-k chunks using a sentence-level cross-encoder model  
6. Generate Context-Aware Responses via LLMs 
Construct dynamic prompts incorpora ng retrieved context chunks and use OpenAI GPT-3.5 to 
generate  answers. 
7. Evaluate System Performance Across Sample Queries 
Test the pipeline against at least 3 user-designed queries and measure relevance, accuracy, and 
completeness of generated answers. 
8. Reusability in Code Design 
Keep future extension and code reusability while wri ng code

## Design
- Embedding Layer
    Effectively extract, clean and chunk the document text using various strategies
    Evaluate multiple embedding models

- Search Layer
    Define at least three realistic queries whose answers reside in the policy.
    Build a vector search pipeline (ChromaDB) with a caching mechanism for speed.
    Integrate a cross-encoder reranker to improve the relevance of the top-K results.

- Generation Layer
    Craft an exhaustive prompt that injects the reranked context chunks (and optional few-shot examples) into an LLM (e.g., GPT-3.5/4). 
## Tools and Technologies
Python 3.10.4
Jupyter notebook
LLM(OpenAI GPT, sentence_transformers)
ChromaDB(Vector DB)

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## conclusions
Developed a solution to query PDF documents using RAG implementation.


## Contact
Created by Saurabh Pandey - feel free to contact me!
