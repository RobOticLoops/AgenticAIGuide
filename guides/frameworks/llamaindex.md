# Learning Guide: LlamaIndex

LlamaIndex is a data framework designed specifically for building context-aware LLM applications, excelling particularly in Retrieval Augmented Generation (RAG). It provides tools for data ingestion, indexing, querying, and integration into LLM workflows and agents.

**Key Concepts for Agentic AI:**
*   Data Connectors: Ingesting data from various sources (APIs, files, databases).
*   Indexing: Structuring data for efficient retrieval (Vector Stores, Summaries, Knowledge Graphs).
*   Retrievers: Fetching relevant context based on a query.
*   Query Engines: Answering questions over your data using retrieval and LLMs.
*   Agents: Building agents that leverage LlamaIndex's data capabilities for reasoning and tool use (often complementary to LangChain agents).
*   Observability & Evaluation: Tools for tracking and evaluating RAG pipeline performance.

**Core Links:**
*   [GitHub](https://github.com/run-llama/llama_index)
*   [Documentation](https://docs.llamaindex.ai/en/stable/)
*   [Examples](https://docs.llamaindex.ai/en/stable/examples/examples.html)
*   [YouTube Channel](https://www.youtube.com/@LlamaIndex)
*   [Discord Community](https://discord.gg/llama-index)

---

## LearnLM 1.5 Prompt: LlamaIndex Learning Plan

*Copy and paste the following prompt into a powerful LLM like Google's LearnLM 1.5 (or similar advanced model) to generate a personalized learning plan.*

**Prompt:**

"Act as an expert AI curriculum designer specializing in data frameworks for LLM applications. I am a Python developer aiming to build sophisticated Agentic AI systems that require robust interaction with custom data sources (Retrieval Augmented Generation - RAG). I have a foundational understanding of LLMs and may have some familiarity with frameworks like LangChain.

My goal is to become proficient in using the **LlamaIndex** framework to ingest, index, and query external data effectively within my LLM applications and agents.

Please generate a structured, step-by-step learning plan covering:

1.  **LlamaIndex Fundamentals:** Core concepts (Data Connectors, Nodes, Indexing strategies, Retrievers, Query Engines, Response Synthesizers) and the overall RAG pipeline.
2.  **Data Ingestion:** Connecting to various data sources (files, web pages, APIs) using Data Loaders/Connectors.
3.  **Indexing Strategies:** Understanding and implementing different index types (VectorStoreIndex, SummaryIndex, KnowledgeGraphIndex) and their use cases.
4.  **Retrieval Techniques:** Configuring retrievers for optimal context fetching (similarity search, filtering, fusion).
5.  **Querying Data:** Building basic and advanced query engines (sub-question querying, routing).
6.  **Integration with Agents:** Using LlamaIndex query engines and retrievers as tools within agent frameworks (like LangChain or LlamaIndex's own agent abstractions).
7.  **Evaluation & Observability:** Utilizing LlamaIndex's tools or integrating with external tools (like Langfuse, TruLens) to evaluate and debug RAG pipelines.
8.  **Practical Examples:** Progressing from simple RAG over a document to more complex multi-document queries and agentic data interaction.
9.  **Project Ideas:** Suggest 1-2 projects focused on building a knowledge-enhanced agent using LlamaIndex (e.g., chatbot over technical documentation, a research assistant agent).
10. **Resource Mapping:** Link learning objectives to specific LlamaIndex documentation sections, tutorials, or key example notebooks.

Structure the plan logically, emphasizing hands-on coding for building effective RAG pipelines."

---
