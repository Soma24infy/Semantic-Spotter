## Project Description
Semantic spotter is a solution which should solve the following requirements using LlamaIndex:
- Users would get responses from insurance policy knowledge base.
- If user want to perform a query, system must be able to response to query accurately.


## Objectives
The goal of the project will be to build a robust generative search system capable of effectively and accurately answering
questions from various policy documents.

## RAG Pipeline

- Embedding Layer: Turn text and tables from PDFs into dataframes and create vector representations with OpenAI's text-embedding-ada-002 model. Save these vectors in ChromaDB.
- Search and Rank Layer: Conduct a semantic search for user queries within the knowledge database, bringing up the most relevant results.
- Generation Layer: Combine the search results with the original query and a structured prompt to form coherent responses using a language model.

## Technologies Used
- Programming Languages: Python
- Frameworks: LlamaIndex, OpenAI
- Cache: diskcache


## Contact
Created by Soma Mukherjee


Developed as part of the GEN AI required for Post Graduate Diploma in Machine Learning and AI - IIIT,Bangalore.