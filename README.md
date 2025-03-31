# Awesome Agentic AI - The Master Guide
Mater Guide for Development of Agentic AI

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

**A curated list of awesome frameworks, platforms, models, tools, APIs, and resources for building Agentic AI systems.**

This repository aims to be the definitive guide for developers looking to explore and build with Agentic AI. We focus primarily on **free and open-source** solutions, providing links to documentation, tutorials, examples, and communities to help you get started and stay up-to-date.

**Contributions are welcome!** Please see the [Contributing Guidelines](./CONTRIBUTING.md).

**You will notice prompts tailered to LearnLM 1.5 within the guide files. This is for a future implementation of a Dynamic UI that creates a learning path and time blocks based off specfic Agentic goals the user creates.** 

---

## Table of Contents

*   [Core Concepts](#core-concepts)
*   [Major Ecosystems & Platforms](#major-ecosystems--platforms)
    *   [Google](#google)
    *   [Microsoft](#microsoft)
    *   [OpenAI](#openai)
    *   [Anthropic](#anthropic)
    *   [Meta](#meta)
    *   [Mistral AI](#mistral-ai)
    *   [Hugging Face](#hugging-face)
*   [Agent Frameworks](#agent-frameworks)
    *   [General Purpose / Foundational](#general-purpose--foundational)
    *   [Multi-Agent Systems](#multi-agent-systems)
    *   [Specialized / Experimental](#specialized--experimental)
*   [Orchestration & Deployment Platforms](#orchestration--deployment-platforms)
*   [Foundation Models (LLMs/VLMs)](#foundation-models-llmsvlms)
    *   [Open Weights Models](#open-weights-models)
    *   [API Accessible Models](#api-accessible-models)
*   [Supporting Tools & Libraries](#supporting-tools--libraries)
    *   [Vector Databases](#vector-databases)
    *   [Evaluation & Observability](#evaluation--observability)
    *   [Tool Use & Function Calling](#tool-use--function-calling)
*   [Essential APIs](#essential-apis)
    *   [Search APIs](#search-apis)
    *   [Tool/Service APIs](#toolservice-apis)
*   [Learning Resources](#learning-resources)
    *   [Courses & Tutorials](#courses--tutorials)
    *   [Key Research Papers](#key-research-papers)
    *   [Communities](#communities)
    *   [YouTube Channels & Videos](#youtube-channels--videos)
*   [News & Recent Releases](#news--recent-releases)
*   [Example Implementations (Internal Link)](#example-implementations-internal-link)

---

## Core Concepts

Understanding the fundamentals of Agentic AI.

*   **What is an AI Agent?** - An AI system that perceives its environment, makes decisions, and takes actions to achieve specific goals. Often leverages LLMs for reasoning and planning.
*   **Agentic Workflow / Loop:** Typically involves Planning, Tool Use (Action), Observation, and Reflection/Refinement, often powered by an LLM reasoning core.
*   **LLMs as Reasoning Engines:** How Large Language Models form the core decision-making component in many modern agents.
*   **Tool Use / Function Calling:** Enabling agents to interact with external APIs, databases, or code execution environments to gather information or perform actions.
*   **Memory:** Providing agents with short-term (context window) and long-term (vector stores, databases) memory to maintain context and learn over time.
*   **Planning & Decomposition:** Breaking down complex tasks into smaller, manageable steps. Techniques include Chain-of-Thought, ReAct, Tree of Thoughts.
*   **Multi-Agent Systems (MAS):** Systems where multiple agents collaborate or compete to solve problems, often with specialized roles.

---

## Major Ecosystems & Platforms

Key players providing models, tools, and infrastructure relevant to Agentic AI development.

### Google

*   **Models:**
    *   **Gemini:** Google's flagship multimodal model family. Accessible via API.
        *   [Overview](https://deepmind.google/technologies/gemini/) | [Google AI for Developers](https://ai.google.dev/) | [Vertex AI Access](https://cloud.google.com/vertex-ai/docs/generative-ai/learn/models#gemini-models)
    *   **Gemma:** Family of lightweight, open-weight models built from the same research as Gemini.
        *   [Overview](https://ai.google.dev/gemma) | [Hugging Face Models](https://huggingface.co/models?search=google/gemma) | [Kaggle Models](https://www.kaggle.com/models/google/gemma)
*   **Tools & Platforms:**
    *   **Google AI Studio:** Free, web-based tool for prompt engineering and prototyping with Gemini models.
        *   [Website](https://aistudio.google.com/) | [Documentation](https://ai.google.dev/docs/ai_studio_quickstart)
    *   **Vertex AI Agent Builder:** Managed platform for building and deploying enterprise-grade generative AI agents (Search & Conversation). (Managed Service - potential costs)
        *   [Website](https://cloud.google.com/vertex-ai-agent-builder) | [Documentation](https://cloud.google.com/vertex-ai/docs/agent-builder/introduction)
    *   **Project IDX:** Experimental browser-based development environment with AI integrations.
        *   [Website](https://idx.dev/)
    *   **Firebase Genkit (Developer Preview):** Open source framework to build, deploy, and monitor AI-powered features using Go or Node.js. Integrates with various models/tools.
        *   [GitHub](https://github.com/firebase/genkit) | [Documentation](https://firebase.google.com/docs/genkit)

### Microsoft

*   **Models:**
    *   **Phi:** Family of Small Language Models (SLMs) developed by Microsoft Research, often open source.
        *   [Phi-3 Overview](https://azure.microsoft.com/en-us/blog/introducing-phi-3-redefining-whats-possible-with-small-language-models/) | [Hugging Face (Phi-2)](https://huggingface.co/microsoft/phi-2) | [Hugging Face (Phi-3)](https://huggingface.co/microsoft/Phi-3-mini-4k-instruct)
    *   **Azure OpenAI Service:** Provides access to OpenAI models (GPT-4, GPT-3.5, etc.) via Azure infrastructure. (Managed Service - potential costs)
        *   [Website](https://azure.microsoft.com/en-us/products/ai-services/openai-service) | [Documentation](https://learn.microsoft.com/en-us/azure/ai-services/openai/overview)
*   **Tools & Platforms:**
    *   **Azure AI Studio:** Unified platform for building, managing, and deploying AI models and applications, including agentic solutions. (Managed Service - potential costs)
        *   [Website](https://ai.azure.com/) | [Documentation](https://learn.microsoft.com/en-us/azure/ai-studio/what-is-ai-studio)
    *   **Semantic Kernel:** Open-source SDK that lets you easily build agents that can call your existing code. Integrates LLMs with conventional programming languages.
        *   [GitHub](https://github.com/microsoft/semantic-kernel) | [Documentation](https://learn.microsoft.com/en-us/semantic-kernel/overview/) | [YouTube Playlist](https://www.youtube.com/playlist?list=PLlrxD0HtieHjr_S3__N45tRElcE-_23r_)
    *   **AutoGen:** Framework for enabling multi-agent conversation systems. (See [Agent Frameworks](#multi-agent-systems))
        *   [GitHub](https://github.com/microsoft/autogen) | [Documentation](https://microsoft.github.io/autogen/) | [Examples](https://github.com/microsoft/autogen/tree/main/notebook)

### OpenAI

*   **Models:**
    *   **GPT-4 / GPT-4o / GPT-3.5 Turbo:** Powerful language models accessible via API. (API Access - costs involved)
        *   [Platform](https://platform.openai.com/) | [Model Overview](https://platform.openai.com/docs/models) | [API Reference](https://platform.openai.com/docs/api-reference)
*   **Tools & Platforms:**
    *   **Assistants API:** Framework built into the OpenAI API for creating stateful agents with persistent threads, tool use (Code Interpreter, Retrieval, Function Calling).
        *   [Documentation](https://platform.openai.com/docs/assistants/overview) | [Examples](https://github.com/openai/openai-cookbook/tree/main/examples/assistants_api) | [Video Intro](https://www.youtube.com/watch?v=5rcjGjgJNQc)
    *   **Function Calling:** Feature within Chat Completions API enabling models to call external tools/APIs.
        *   [Documentation](https://platform.openai.com/docs/guides/function-calling) | [Cookbook Example](https://github.com/openai/openai-cookbook/blob/main/examples/How_to_call_functions_with_chat_models.ipynb)

### Anthropic

*   **Models:**
    *   **Claude 3 (Opus, Sonnet, Haiku):** Family of capable models with large context windows, accessible via API. (API Access - costs involved)
        *   [Website](https://www.anthropic.com/claude) | [Documentation](https://docs.anthropic.com/claude/reference/getting-started-with-the-api) | [Console](https://console.anthropic.com/)
*   **Tools & Platforms:**
    *   **Tool Use (Beta):** Feature allowing Claude models to interact with external tools and functions.
        *   [Documentation](https://docs.anthropic.com/claude/docs/tool-use)

### Meta

*   **Models:**
    *   **Llama:** Family of powerful open-weight models (Llama 2, Llama 3). Requires requesting access for some versions/uses.
        *   [Llama Website](https://llama.meta.com/) | [Llama 3 Models (HF)](https://huggingface.co/collections/meta-llama/meta-llama-3-66214712577ca434503a4d1c) | [GitHub](https://github.com/meta-llama/llama3)
*   **Tools & Platforms:**
    *   Primarily focused on releasing models, less on specific agent tooling platforms (often integrated via frameworks like LangChain, LlamaIndex).

### Mistral AI

*   **Models:**
    *   **Mistral / Mixtral:** High-performing open-weight and optimized API models.
        *   [Website](https://mistral.ai/) | [Models (HF)](https://huggingface.co/mistralai) | [API Docs](https://docs.mistral.ai/)
*   **Tools & Platforms:**
    *   **La Plateforme:** API access to Mistral models. (API Access - costs involved)
        *   [Platform](https://console.mistral.ai/) | [API Docs](https://docs.mistral.ai/)

### Hugging Face

*   **Platform:** The central hub for open-source AI, hosting models, datasets, and libraries. Essential for accessing many open-weight models.
    *   [Website](https://huggingface.co/)
    *   **Transformers:** Core library for working with transformer models.
        *   [GitHub](https://github.com/huggingface/transformers) | [Documentation](https://huggingface.co/docs/transformers/index)
    *   **Agents:** Experimental library for autonomous agents using Hugging Face models and tools.
        *   [Documentation](https://huggingface.co/docs/transformers/main/en/transformers_agents) | [Blog Post](https://huggingface.co/blog/hf-agents)

---

## Agent Frameworks

Libraries and toolkits specifically designed for building agentic applications.

### General Purpose / Foundational

*   **LangChain:** A popular framework for developing applications powered by language models. Provides modules for models, prompts, memory, indexing, chains, and agents.
    *   **Description:** Comprehensive toolkit with extensive integrations. Can have a steeper learning curve initially.
    *   **Links:** [GitHub](https://github.com/langchain-ai/langchain) | [Python Docs](https://python.langchain.com/) | [JS/TS Docs](https://js.langchain.com/) | [Conceptual Docs](https://docs.langchain.com/docs/) | [YouTube Channel](https://www.youtube.com/@LangChain) 
    *   **Links:** [GitHub](...) | [Python Docs](...) | ... | [**Guide**](./guides/frameworks/langchain.md)
 
*   **LlamaIndex:** A data framework for LLM applications, focused on connecting custom data sources to LLMs. Excels at RAG (Retrieval-Augmented Generation) and data-centric agents.
    *   **Description:** Strong focus on data ingestion, indexing, querying, and integrating data into LLM workflows. Often used alongside LangChain or independently.
    *   **Links:** [GitHub](https://github.com/run-llama/llama_index) | [Documentation](https://docs.llamaindex.ai/en/stable/) | [Examples](https://docs.llamaindex.ai/en/stable/examples/examples.html) | [YouTube Channel](https://www.youtube.com/@LlamaIndex)
*   **LangGraph:** An extension of LangChain for building stateful, multi-actor applications with LLMs, using graphs to define cycles and control flow. Well-suited for complex agentic loops.
    *   **Description:** Enables building robust, cyclical agent behaviors (Plan -> Act -> Observe -> Reflect).
    *   **Links:** [GitHub](https://github.com/langchain-ai/langgraph) | [Documentation](https://langchain-ai.github.io/langgraph/) | [Examples (Python)](https://github.com/langchain-ai/langgraph/tree/main/examples) | [JS Examples](https://github.com/langchain-ai/langgraphjs/tree/main/examples)

### Multi-Agent Systems

*   **AutoGen (Microsoft):** Framework for simplifying the orchestration, optimization, and automation of complex LLM workflows using multiple, conversational agents.
    *   **Description:** Enables building systems where different agents (e.g., planner, coder, critic) collaborate.
    *   **Links:** [GitHub](https://github.com/microsoft/autogen) | [Documentation](https://microsoft.github.io/autogen/) | [Examples (Notebooks)](https://github.com/microsoft/autogen/tree/main/notebook) | [Discord Community](https://discord.gg/pAbnFJrkgZ)
*   **CrewAI:** Framework for orchestrating role-playing, autonomous AI agents. Enables agents to collaborate to accomplish complex tasks.
    *   **Description:** Focuses on defining agents with specific roles, backstories, and tools, and orchestrating their collaboration using a defined process (e.g., sequential, hierarchical).
    *   **Links:** [GitHub](https://github.com/joaomdmoura/crewAI) | [Documentation](https://docs.crewai.com/) | [Examples](https://github.com/joaomdmoura/crewAI-examples) | [Video Intro (by author)](https://www.youtube.com/watch?v=tFZz-kT1L-M)
*   **Agency Swarm:** A framework inspired by swarm intelligence, designed for creating and managing swarms of communicating AI agents that operate collectively on complex tasks.
    *   **Description:** Focuses on defining agent-to-agent communication protocols and facilitating emergent collaboration.
    *   **Links:** [GitHub](https://github.com/VRSEN/agency-swarm) | [Documentation](https://docs.agencyswarm.dev/)

### Specialized / Experimental

*   **MemGPT:** Towards LLMs as Operating Systems - research and framework exploring persistent memory and function calling for agents.
    *   **Description:** Focuses on managing context window limitations through virtual context management and enabling long-term agent interactions.
    *   **Links:** [GitHub](https://github.com/cpacker/MemGPT) | [Website/Paper](https://memgpt.ai/) | [Discord Community](https://discord.gg/memgpt)
*   **BabyAGI:** A simple, early example of an autonomous agent loop (task creation, prioritization, execution). Often used as a learning tool or starting point.
    *   **Description:** Foundational concept demonstrating autonomous task management with LLMs. Many variations exist.
    *   **Links:** [Original GitHub (Yohei Nakajima)](https://github.com/yoheinakajima/babyagi) | [Conceptual Overview](https://twitter.com/yoheinakajima/status/1642836086684221441)
*   **AutoGPT:** One of the first highly visible autonomous agent projects. Aims to achieve goals by breaking them down and using tools automatically.
    *   **Description:** Ambitious project showcasing autonomous capabilities, though practical reliability can vary. Good for understanding agent concepts.
    *   **Links:** [GitHub](https://github.com/Significant-Gravitas/AutoGPT) | [Website](https://agpt.co/) | [Documentation](https://docs.agpt.co/)

---

## Orchestration & Deployment Platforms

Tools and platforms (some open-source, some managed) for building, visualizing, deploying, and monitoring agentic applications.

*   **Flowise:** Open-source UI visual tool to build customized LLM flows & agents using LangChainJS.
    *   **Description:** Drag-and-drop interface for creating agentic workflows without extensive coding.
    *   **Links:** [GitHub](https://github.com/FlowiseAI/Flowise) | [Website](https://flowiseai.com/) | [Documentation](https://docs.flowiseai.com/) | [YouTube Tutorials](https://www.youtube.com/playlist?list=PL4Kv9Hxti93yhjQ-4Tj7NR9mO_MsnbS9-)
*   **Dify.ai:** Open-source LLMOps platform to build and operate generative AI applications, including agent-based systems.
    *   **Description:** Provides tools for prompt engineering, RAG, workflows, and operational monitoring. Offers cloud and self-hosted options.
    *   **Links:** [GitHub](https://github.com/langgenius/dify) | [Website](https://dify.ai/) | [Documentation](https://docs.dify.ai/)
*   **Superagent:** Open-source framework for building, managing & deploying autonomous AI agents with a focus on ease of use and powerful features like scheduling and long-term memory.
    *   **Description:** Provides a higher-level abstraction for agent creation and includes a UI for management.
    *   **Links:** [GitHub](https://github.com/homanp/superagent) | [Website](https://superagent.sh/) | [Documentation](https://docs.superagent.sh/)
*   **Langfuse:** Open-source observability & analytics for LLM applications. Helps trace, debug, and evaluate agent performance.
    *   **Description:** Crucial for understanding and improving complex agent behaviors. Integrates with LangChain, LlamaIndex, etc. Offers cloud and self-hosted options.
    *   **Links:** [GitHub](https://github.com/langfuse/langfuse) | [Website](https://langfuse.com/) | [Documentation](https://langfuse.com/docs)

---

## Foundation Models (LLMs/VLMs)

Core models powering agent intelligence. Focus on accessibility (open weights or reasonable API access).

### Open Weights Models

Models whose weights are publicly available, allowing for local deployment and fine-tuning (check licenses for usage restrictions).

*   **Llama Family (Meta):** (See [Meta](#meta)) Llama 3, Llama 2. Various sizes.
*   **Mistral & Mixtral (Mistral AI):** (See [Mistral AI](#mistral-ai)) High-performance models.
*   **Gemma (Google):** (See [Google](#google)) Lightweight, capable models.
*   **Phi (Microsoft):** (See [Microsoft](#microsoft)) Strong small language models (SLMs).
*   **Qwen (Alibaba Cloud):** Series of powerful multilingual LLMs and VLMs.
    *   [Qwen2 (HF)](https://huggingface.co/collections/Qwen/qwen2-665a574ead71b_9fbtu) | [GitHub](https://github.com/QwenLM/Qwen2)
*   **Command R / R+ (Cohere):** Models focused on RAG and Tool Use, weights available for research/non-commercial use (check license).
    *   [Command R+ (HF)](https://huggingface.co/CohereForAI/c4ai-command-r-plus) | [Blog Post](https://txt.cohere.com/command-r-plus-microsoft-azure/)

### API Accessible Models

Models primarily accessed via APIs (often with free tiers or paid usage).

*   **Gemini Family (Google):** (See [Google](#google))
*   **GPT Family (OpenAI):** (See [OpenAI](#openai))
*   **Claude Family (Anthropic):** (See [Anthropic](#anthropic))
*   **Mistral API Models:** (See [Mistral AI](#mistral-ai))
*   **Cohere API Models:** (Command, Embed, Rerank)
    *   [Website](https://cohere.com/) | [Documentation](https://docs.cohere.com/)

---

## Supporting Tools & Libraries

Essential components often used when building agents.

### Vector Databases

For efficient storage and retrieval of embeddings, crucial for agent memory and RAG.

*   **ChromaDB:** Open-source embedding database.
    *   [GitHub](https://github.com/chroma-core/chroma) | [Website](https://www.trychroma.com/) | [Docs](https://docs.trychroma.com/)
*   **Qdrant:** Open-source vector database & vector similarity search engine.
    *   [GitHub](https://github.com/qdrant/qdrant) | [Website](https://qdrant.tech/) | [Docs](https://qdrant.tech/documentation/)
*   **Weaviate:** Open-source, AI-native vector database.
    *   [GitHub](https://github.com/weaviate/weaviate) | [Website](https://weaviate.io/) | [Docs](https://weaviate.io/developers/weaviate)
*   **LanceDB:** Open-source serverless vector database for AI applications. Runs embedded.
    *   [GitHub](https://github.com/lancedb/lancedb) | [Website](https://lancedb.com/) | [Docs](https://lancedb.github.io/lancedb/)

### Evaluation & Observability

Tools for assessing agent performance, debugging, and monitoring.

*   **Langfuse:** (See [Orchestration & Deployment Platforms](#orchestration--deployment-platforms))
*   **RAGAs:** Evaluation framework for Retrieval Augmented Generation (RAG) pipelines.
    *   [GitHub](https://github.com/explodinggradients/ragas) | [Docs](https://docs.ragas.io/)
*   **TruLens:** Open-source library for evaluating and tracking LLM-based applications, including RAG and agents.
    *   [GitHub](https://github.com/truera/trulens) | [Website](https://www.trulens.org/) | [Docs](https://www.trulens.org/trulens-eval/getting_started/)
*   **LangSmith:** Platform for debugging, testing, evaluating, and monitoring LLM applications (from LangChain creators). Has free tier.
    *   [Website](https://smith.langchain.com/) | [Docs](https://docs.smith.langchain.com/)

### Tool Use & Function Calling

Libraries and standards facilitating agent interaction with external tools. (Often integrated into frameworks)

*   **OpenAI Function Calling:** (See [OpenAI](#openai))
*   **LangChain Tool Use:** Built-in support for defining and using tools within agents.
    *   [Docs](https://python.langchain.com/v0.2/docs/concepts/#tools)
*   **LlamaIndex Tool Use:** Support for function calling and tool abstractions.
    *   [Docs](https://docs.llamaindex.ai/en/stable/module_guides/deploying/agents/tools/root.html)
*   **Gorilla LLM:** Research project and models fine-tuned for accurate API calling.
    *   [GitHub](https://github.com/ShishirPatil/gorilla) | [Project Page](https://gorilla.cs.berkeley.edu/)

---

## Essential APIs

External APIs commonly integrated into agents for real-world interaction.

### Search APIs

Allowing agents to access up-to-date information from the web.

*   **Tavily AI:** Search API optimized for LLMs and RAG, providing concise answers. Offers free tier.
    *   [Website](https://tavily.com/) | [Docs](https://docs.tavily.com/)
*   **SerpApi:** Real-time Google Search API. Paid service with free trial.
    *   [Website](https://serpapi.com/) | [Docs](https://serpapi.com/search-api)
*   **Brave Search API:** Privacy-preserving search API. Offers free tier for developers.
    *   [Website](https://brave.com/search/api/) | [Docs](https://api.search.brave.com/app/documentation/introduction)
*   **You.com API:** Search API focused on providing answers and citations. Free/Paid Tiers.
    *   [API Info](https://about.you.com/youapi/) | [Documentation](https://documentation.you.com/)

### Tool/Service APIs

Examples of APIs agents might use to perform actions.

*   **Weather APIs:** (e.g., OpenWeatherMap, WeatherAPI)
*   **Financial Data APIs:** (e.g., Alpha Vantage, Finnhub)
*   **Code Execution APIs:** (e.g., JUDGE0, various sandbox environments)
*   **Generic Web Interaction:** (e.g., Browserless.io, ScraperAPI for web scraping/automation)
*   **Zapier NLA (Natural Language Actions):** Allows agents to interact with thousands of apps via Zapier.
    *   [Website](https://nla.zapier.com/) | [LangChain Integration](https://python.langchain.com/v0.2/docs/integrations/tools/zapier/)

---

## Learning Resources

Courses, tutorials, papers, and communities to deepen your understanding.

### Courses & Tutorials

*   **DeepLearning.AI Short Courses:** Numerous courses on LangChain, LLM Application Development, Building Agents.
    *   [Website](https://www.deeplearning.ai/short-courses/)
*   **LangChain & LangGraph Tutorials:** Official documentation and example notebooks.
    *   [LangChain Tutorials](https://python.langchain.com/v0.2/docs/tutorials/) | [LangGraph Tutorials](https://langchain-ai.github.io/langgraph/tutorials/)
*   **LlamaIndex Tutorials:** Official documentation and example notebooks.
    *   [Website](https://docs.llamaindex.ai/en/stable/getting_started/starter_tutorials.html)
*   **Microsoft AI Learning:** Courses and paths related to Azure AI and Semantic Kernel.
    *   [Website](https://learn.microsoft.com/en-us/training/ai/)

### Key Research Papers

Foundational papers shaping agentic AI development.

*   **ReAct: Synergizing Reasoning and Acting in Language Models:** (Wei et al., 2022) - [arXiv](https://arxiv.org/abs/2210.03629)
*   **Chain-of-Thought Prompting Elicits Reasoning in Large Language Models:** (Wei et al., 2022) - [arXiv](https://arxiv.org/abs/2201.11903)
*   **Tree of Thoughts: Deliberate Problem Solving with Large Language Models:** (Yao et al., 2023) - [arXiv](https://arxiv.org/abs/2305.10601)
*   **LLMs as Tool Makers (LATM):** (Cai et al., 2023) - [arXiv](https://arxiv.org/abs/2305.17126)
*   **AutoGen: Enabling Next-Gen LLM Applications via Multi-Agent Conversation:** (Wu et al., 2023) - [arXiv](https://arxiv.org/abs/2308.08155)
*   **MemGPT: Towards LLMs as Operating Systems:** (Packer et al., 2023) - [arXiv](https://arxiv.org/abs/2310.08560)

### Communities

*   **LangChain Discord:** Active community for LangChain and LangGraph users.
    *   [Invite Link](https://discord.gg/langchain)
*   **LlamaIndex Discord:** Community for LlamaIndex users.
    *   [Invite Link](https://discord.gg/llama-index)
*   **AutoGen Discord:** Community for AutoGen users.
    *   [Invite Link](https://discord.gg/pAbnFJrkgZ)
*   **Hugging Face Discord:** General AI and Hugging Face ecosystem discussions.
    *   [Invite Link](https://discord.gg/huggingface)
*   **r/LangChain Subreddit:** Reddit community for discussions.
    *   [Link](https://www.reddit.com/r/LangChain/)
*   **r/LocalLLaMA Subreddit:** Discussions focused on running LLMs locally.
    *   [Link](https://www.reddit.com/r/LocalLLaMA/)

### YouTube Channels & Videos

*   **LangChain:** [Channel Link](https://www.youtube.com/@LangChain)
*   **LlamaIndex:** [Channel Link](https://www.youtube.com/@LlamaIndex)
*   **James Briggs:** Excellent tutorials on Agents, LangChain, AutoGen, etc. [Channel Link](https://www.youtube.com/@jamesbriggs)
*   **Sam Witteveen:** Deep dives into AI concepts, frameworks, and papers. [Channel Link](https://www.youtube.com/@samwitteveenai)
*   **AI Jason:** Practical AI application development tutorials. [Channel Link](https://www.youtube.com/@AIJason)
*   **Prompt Engineering (DeepLearning.AI):** Covers techniques relevant to agent prompting. [Playlist Link](https://www.youtube.com/playlist?list=PLkDaE6sCZn6FAr-4t2qRP_EqQ7DpSdg-Q)

---

## News & Recent Releases

Keeping track of the rapidly evolving Agentic AI landscape.

*   **(Placeholder)** This section can link to key AI newsletters (e.g., The Batch, Last Week in AI), blogs, or a dedicated `NEWS.md` file within the repo tracking major framework/model releases relevant to agents.
*   **Key AI Blogs:**
    *   [Google AI Blog](https://ai.googleblog.com/)
    *   [OpenAI Blog](https://openai.com/blog/)
    *   [Microsoft Research Blog](https://www.microsoft.com/en-us/research/blog/)
    *   [Anthropic News](https://www.anthropic.com/news)
    *   [Hugging Face Blog](https://huggingface.co/blog)

---

## Example Implementations (Internal Link)

*   [`./examples/`](./examples/) - Explore practical examples categorized by framework, task, and complexity. See the [Examples README](./examples/README.md) for structure.


*   **(Placeholder)** [`./examples/`](./examples/) - Explore practical examples categorized by framework, task, and complexity. (Link to be created later when the folder exists).

---

## Contributing

Your contributions are always welcome! Please take a look at the [Contribution Guidelines](./CONTRIBUTING.md) first.
