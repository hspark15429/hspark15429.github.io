---
title: "Graph RAG Legal Chatbot"
date: 2025-11-27
excerpt: "Citation-aware legal assistant utilizing Neo4j and Gemini <br/><br/><img src='/images/neo4j.jpg'>"
collection: portfolio
---

![neo4j](/images/neo4j.jpg)
![lawrag](/images/lawrag.png)

**Objective:** Designed a citation-aware RAG (Retrieval-Augmented Generation) pipeline specifically for the legal domain, enabling users to receive verifiable immigration advice grounded in US Code while minimizing hallucinations.

**Features:**
* **Citation-Aware Pipeline:** Engineered a system that retrieves and cites specific legal statutes, ensuring high transparency and trust.
* **Hybrid Retrieval Strategy:** Combined semantic search (vector embeddings) with graph traversal to increase retrieval recall by 20% compared to standard vector-only methods.
* **Knowledge Graph Integration:** Utilized Neo4j to model complex relationships between legal entities and statutes.
* **Domain-Specific Embeddings:** Integrated LegalBERT to capture nuanced legal terminology and context.
* **Generative Engine:** Deployed Google's Gemini models to synthesize retrieved legal context into clear, actionable advice.

**Technologies:** Python, Neo4j, LangChain, LegalBERT, Google Gemini API, Docker.