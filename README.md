## Project Description
Semantic spotter is a solution which should solve the following requirements using LlamaIndex:
- Users would get responses from insurance policy knowledge base.
- If user want to perform a query, system must be able to response to query accurately.


## Objectives
The goal of the project will be to build a robust generative search system capable of effectively and accurately answering
questions from various policy documents.

## Architecture Description

1. Documents: We will be using list of HDFC insurance documents provides inside a single
folder.
2. Open API embedding: We ars using OpenAPI embedding as Vector DB for indexing
insureance documetns in the form of embedding.
3. Query Engine: We are using Query Engine Module of Llammaindex for perfomring
synantic Search. Query Engine will use internally Retriver and Cohere Rerank to retrrive
top-k relvent nodes from embedding.
4. LLM : top k-documets along with usewr query will be passed to LLM to generate the
accurate response.We are using chatGPT LLM.
5. Caching:" Caching is being used to improve the read operation. Recent similar search
will be store in Caching and user query frist will be served from Cahcing. If user query
not found in cahce then query will be forwared to query engine and then LLM to generate
the resposne. user query and generated resposne will be cached in in cache and will be
served from there based ttl.
6. Meta data:Along with Resposne we are also returning docs referece and similary score to
improve the user confidence towards the implemented RAG system.
7. Cohere-Rerank: Is being used to rerank the query based on semantic score.

## Technologies Used
- Programming Languages: Python
- Frameworks: LlamaIndex, OpenAI
- Cache: diskcache


## Contact
Created by Soma Mukherjee


Developed as part of the GEN AI required for Post Graduate Diploma in Machine Learning and AI - IIIT,Bangalore.
