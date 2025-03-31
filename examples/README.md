# Agentic AI Examples

This directory contains practical examples demonstrating how to use various frameworks, tools, and techniques discussed in the main [Awesome Agentic AI guide](../README.md).

Our goal is to provide runnable code snippets and small projects categorized for easy navigation.

## Proposed Structure

Examples are organized primarily by the **core framework** or **concept** they demonstrate. Within each category, further sub-categorization might occur based on complexity or specific task.

*   **/langchain/**: Examples using the LangChain framework.
    *   `/basic_agents/`: Simple agent implementations (ReAct, etc.).
    *   `/tool_use/`: Demonstrating custom and built-in tools.
    *   `/rag_agents/`: Agents integrated with retrieval systems.
    *   `/memory/`: Examples showcasing different memory types.
    *   `/langgraph/`: More complex stateful agents using LangGraph.
*   **/llamaindex/**: Examples focusing on LlamaIndex, particularly RAG.
    *   `/data_ingestion/`: Using various data loaders.
    *   `/indexing/`: Demonstrating different index types.
    *   `/query_engines/`: Basic and advanced querying examples.
    *   `/rag_pipelines/`: End-to-end RAG examples.
    *   `/agent_integration/`: Using LlamaIndex components as tools for agents.
*   **/crewai/**: Examples of multi-agent collaboration using CrewAI.
    *   `/simple_crew/`: Basic 2-3 agent crews.
    *   `/hierarchical_crew/`: Crews with manager-worker structures.
    *   `/custom_tools/`: Agents using custom-developed tools.
*   **/autogen/**: Examples of multi-agent conversations using AutoGen.
    *   `/two_agent_chat/`: Simple request-response patterns.
    *   `/group_chat/`: Multiple agents collaborating (e.g., coding, research).
    *   `/function_calling/`: Agents executing functions.
*   **/openai_assistants/**: Examples using the OpenAI Assistants API.
    *   `/code_interpreter/`: Using the built-in code interpreter.
    *   `/retrieval/`: Q&A over uploaded files.
    *   `/function_calling/`: Assistants using custom external tools.
*   **/vector_stores/**: Examples of using specific vector databases.
    *   `/chromadb/`: Snippets for ChromaDB operations.
    *   `/qdrant/`: Snippets for Qdrant operations.
    *   *(Add others as needed)*
*   **/evaluation/**: Examples demonstrating evaluation frameworks.
    *   `/langfuse_integration/`: Code showing how to trace applications with Langfuse.
    *   `/ragas_usage/`: Evaluating RAG pipelines with Ragas.
*   **/concepts/**: Snippets illustrating core Agentic AI concepts.
    *   `/react_pattern/`: A minimal implementation of the ReAct loop.
    *   `/function_calling_simple/`: Basic function calling without a full framework.

## Contribution

We welcome contributions! Please see the main [CONTRIBUTING.md](../CONTRIBUTING.md). When adding an example:
*   Place it in the most relevant category.
*   Include a `README.md` within the example's specific folder explaining:
    *   What the example does.
    *   How to set it up (dependencies, API keys).
    *   How to run it.
*   Keep examples focused and as minimal as possible to demonstrate the core concept.
*   Ensure code is well-commented.

*(This structure is a starting point and can evolve as more examples are added.)*
