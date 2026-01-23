---
title: "HuggingFace KG Retriever"
date: 2025-12-02
excerpt: "Heterogeneous Knowledge Graph pipeline with GNNs and LLM fine-tuning <br/><br/><img src='/images/graph_retrieval.png'>"
collection: portfolio
---

![diagram](/images/graph_retrieval.png)
![results](/images/full_model_comparison.png)

**Objective:** Built a sophisticated retrieval pipeline that leverages heterogeneous Knowledge Graphs (KGs) to enhance multi-label classification and retrieval accuracy, effectively bridging the gap between structured graph data and Large Language Models (LLMs).

**Features:**
* **Heterogeneous Graph Pipeline:** Constructed a robust pipeline integrating BGE (semantic) and BM25 (lexical) embeddings to represent complex data relationships.
* **Advanced GNN Architectures:** Trained Graph Attention Networks (GAT) and Graph Transformers to capture structural dependencies.
* **Imbalance Handling:** Implemented Focal Loss during training to significantly improve performance on underrepresented classes, boosting micro-f1 scores by 30% over baselines.
* **Graph-RAG Implementation:** Developed Retrieval-Augmented Generation using Ego-Graphs to ground LLM responses in structured facts.
* **Cross-Modal Alignment:** Implemented a trained Projection Layer to map GAT-encoded graph features into the LLM's embedding space, enabling the model to "see" graph structures natively.
* **Efficient LLM Adaptation (LoRA):** Applied Low-Rank Adaptation (LoRA) adapters to open-source LLMs (Qwen and Mistral), facilitating efficient fine-tuning on graph tasks while preserving pre-trained knowledge.
* **Structured Instruction Tuning:** Designed a specialized prompt schema ([INST] Task List + Node Name + Instructions [/INST]) processed via an LLM Text Embedder to guide the generative output for specific node-level tasks.

**Technologies:** Python, PyTorch Geometric, Neo4j, BGE, BM25, Qwen, Mistral, GAT, Graph Transformer.

Github Repo:  [https://github.com/KeXin95/HuggingfaceKG-retriever](https://github.com/KeXin95/HuggingfaceKG-retriever)

