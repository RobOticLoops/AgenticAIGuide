 # Learning Guide: Microsoft AutoGen

AutoGen is a framework developed by Microsoft for building applications using multiple, conversational agents that collaborate to solve complex tasks. It simplifies the orchestration, automation, and optimization of LLM workflows involving diverse agent roles and interactions.

**Key Concepts for Agentic AI:**
*   Conversable Agents: The core building block, agents that can send and receive messages.
*   User Proxy Agent: Represents the human user in the conversation.
*   Assistant Agent: A generic LLM-powered agent.
*   Group Chat Manager: Orchestrates conversations between multiple agents.
*   Agent Roles & Specialization: Defining agents with specific skills or instructions (e.g., Coder, Critic, Planner).
*   Tool Use / Function Calling: Enabling agents to execute code or call external APIs.
*   Conversation Patterns: Designing workflows for how agents interact (e.g., sequential chats, group discussions).

**Core Links:**
*   [GitHub](https://github.com/microsoft/autogen)
*   [Documentation](https://microsoft.github.io/autogen/)
*   [Examples (Notebooks)](https://github.com/microsoft/autogen/tree/main/notebook)
*   [Blog Posts/Papers](https://microsoft.github.io/autogen/blog/)
*   [Discord Community](https://discord.gg/pAbnFJrkgZ)

---

## LearnLM 1.5 Prompt: AutoGen Learning Plan

*Copy and paste the following prompt into a powerful LLM like Google's LearnLM 1.5 (or similar advanced model) to generate a personalized learning plan.*

**Prompt:**

"Act as an expert AI curriculum designer specializing in Multi-Agent Systems (MAS). I am a Python developer familiar with LLMs and basic agent concepts, looking to build more complex, collaborative AI systems.

My goal is to learn the **Microsoft AutoGen** framework to create applications where multiple specialized AI agents converse and work together to achieve sophisticated tasks.

Please generate a structured, step-by-step learning plan covering:

1.  **AutoGen Core Concepts:** Understanding the framework's philosophy, Conversable Agents (`UserProxyAgent`, `AssistantAgent`), and the role of conversation in driving workflows.
2.  **Basic Agent Setup:** Creating and configuring individual agents with different LLMs and system messages.
3.  **Two-Agent Conversations:** Setting up simple interactions between two agents (e.g., user proxy and assistant).
4.  **Group Chat Orchestration:** Using `GroupChat` and `GroupChatManager` to manage multi-agent collaborations.
5.  **Defining Agent Roles:** Designing effective prompts and configurations for specialized agents (e.g., Planner, Coder, Critic, Executor).
6.  **Tool Use & Function Calling:** Registering Python functions or tools for agents to execute within the conversation flow.
7.  **Conversation Flow Control:** Customizing agent replies, termination conditions, and speaker selection.
8.  **AutoGen Studio (Optional):** Briefly introduce the UI tool for building and experimenting with AutoGen agents.
9.  **Practical Examples:** Building example multi-agent systems like automated code generation/debugging, research task decomposition, or conversational analysis.
10. **Project Ideas:** Suggest 1-2 projects involving 3+ collaborating agents using AutoGen.
11. **Resource Mapping:** Link learning objectives to specific AutoGen documentation pages, example notebooks, or research papers.

Structure the plan logically, emphasizing practical implementation of conversational agent patterns."

---
