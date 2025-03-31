# Learning Guide: Qdrant

Qdrant (pronounced "Quadrant") is an open-source vector database and vector similarity search engine written in Rust. It's designed for performance, scalability, and flexibility, offering features like rich filtering, payload storage, and efficient querying, making it suitable for demanding Agentic AI memory and RAG tasks.

**Key Concepts for Agentic AI:**
*   Vector Embeddings & Similarity Search: Core concepts.
*   Collections: Storing points (vectors with optional payloads and IDs).
*   Points: Representing data with a vector, an ID, and an optional JSON payload.
*   Payloads: Storing arbitrary JSON data alongside vectors, enabling filtering.
*   Filtering: Performing searches that combine vector similarity with filtering on payload fields (pre-filtering or post-filtering).
*   Quantization: Techniques (Scalar, Product Quantization) for reducing memory footprint and potentially speeding up search, with a trade-off in accuracy.
*   Deployment: Running locally (Docker), Qdrant Cloud (managed service), or self-hosting clusters.
*   Clients: Official clients available (Python, Go, Rust, TypeScript).

**Core Links:**
*   [GitHub](https://github.com/qdrant/qdrant)
*   [Website](https://qdrant.tech/)
*   [Documentation](https://qdrant.tech/documentation/)
*   [Qdrant Cloud](https://cloud.qdrant.io/)
*   [Blog](https://qdrant.tech/blog/)
*   [Discord Community](https://discord.gg/qdrant)

---

## LearnLM 1.5 Prompt: Qdrant Learning Plan

*Copy and paste the following prompt into a powerful LLM like Google's LearnLM 1.5 (or similar advanced model) to generate a personalized learning plan.*

**Prompt:**

"Act as an expert AI curriculum designer focused on vector database technology. I am a Python developer building Agentic AI systems requiring efficient and scalable vector storage for RAG and long-term memory, potentially with complex filtering needs.

My goal is to become proficient in using the **Qdrant** vector database.

Please generate a structured, step-by-step learning plan covering:

1.  **Qdrant Fundamentals:** Core concepts (Collections, Points, Vectors, Payloads, Similarity Metrics, Filtering). How Qdrant differs from other vector DBs.
2.  **Setup & Basic Operations:** Setting up Qdrant (e.g., using Docker for local development) and using the `qdrant-client` (Python) to connect, create collections, add points (vectors + payloads), and perform basic similarity searches.
3.  **Indexing and Storage:** Understanding configuration options for collections (vector parameters, indexing options).
4.  **Advanced Search & Filtering:**
    *   Implementing searches with metadata filtering (using `must`, `should`, `must_not` conditions on payloads).
    *   Understanding filter performance implications.
5.  **Data Management:** Updating payloads, deleting points, managing collections.
6.  **Performance Considerations:** Introduction to concepts like quantization (Scalar, PQ), sharding, and replication (more focus on concepts than deep implementation initially).
7.  **Integration with LLM Frameworks:** Showing basic examples or pointing to resources on integrating Qdrant as a VectorStore in LangChain or LlamaIndex.
8.  **Deployment Options:** Overview of running locally, using Qdrant Cloud, and self-hosting.
9.  **Project Ideas:** Suggest a simple project integrating Qdrant where filtering is beneficial (e.g., RAG over product reviews with filtering by rating or date).
10. **Resource Mapping:** Link learning objectives to specific Qdrant documentation pages (quickstart, concepts, tutorials, client library docs), blog posts, or example code snippets.

Structure the plan logically, focusing on practical Python client usage and understanding Qdrant's filtering capabilities."

---
