# Learning Guide: Microsoft Semantic Kernel

Microsoft Semantic Kernel is an open-source SDK that allows developers to integrate Large Language Models (LLMs) with conventional programming languages like C#, Python, and Java. It acts as an orchestration layer, making it easier to build AI agents, plugins, and complex AI workflows by combining AI prompts with native code functions.

**Key Concepts for Agentic AI:**
*   Kernel: The central orchestrator that processes requests.
*   Plugins: Collections of related functions (semantic or native).
*   Functions:
    *   Semantic Functions: Defined by prompts run by an AI model.
    *   Native Functions: Regular code (e.g., Python, C# methods) decorated to be callable by the Kernel.
*   Connectors: Interface with AI models (OpenAI, Azure OpenAI, Hugging Face) and memory sources.
*   Memory: Integrating short-term (context) and long-term (vector databases) memory.
*   Planners: Automatically orchestrate function calls to fulfill a user's goal (e.g., Handlebars Planner, Stepwise Planner).
*   Agent Building: Implicitly supported by combining planning, functions (tools), and memory.

**Core Links:**
*   [GitHub (Multi-language)](https://github.com/microsoft/semantic-kernel)
*   [Documentation Hub](https://learn.microsoft.com/en-us/semantic-kernel/overview/)
*   [Python Documentation](https://learn.microsoft.com/en-us/semantic-kernel/python/)
*   [C# Documentation](https://learn.microsoft.com/en-us/semantic-kernel/dotnet/)
*   [YouTube Playlist](https://www.youtube.com/playlist?list=PLlrxD0HtieHjr_S3__N45tRElcE-_23r_)
*   [Blog](https://devblogs.microsoft.com/semantic-kernel/)

---

## LearnLM 1.5 Prompt: Semantic Kernel Learning Plan

*Copy and paste the following prompt into a powerful LLM like Google's LearnLM 1.5 (or similar advanced model) to generate a personalized learning plan.*

**Prompt:**

"Act as an expert AI curriculum designer specializing in integrating LLMs into software applications. I am a developer proficient in [Specify your language: Python, C#, or Java] and want to build AI-powered features and agents by combining LLM capabilities with my existing codebase.

My goal is to learn the **Microsoft Semantic Kernel** SDK ([Specify language version]) to orchestrate AI workflows, create plugins (semantic and native functions), manage memory, and utilize planners for agent-like behavior.

Please generate a structured, step-by-step learning plan covering:

1.  **Semantic Kernel Fundamentals:** Core concepts (Kernel, Plugins, Semantic Functions, Native Functions, Connectors, Memory, Planners) and the overall philosophy.
2.  **Setup & Basic Invocation:** Installing the SDK, configuring the Kernel with an LLM Connector (e.g., OpenAI, Azure OpenAI), and invoking a simple semantic function (prompt).
3.  **Creating Semantic Functions:** Defining prompts using the Handlebars template syntax, managing prompt files.
4.  **Creating Native Functions:** Writing regular code functions in [Your Language] and decorating/registering them so the Kernel can call them as tools.
5.  **Building Plugins:** Organizing semantic and native functions into logical Plugins.
6.  **Chaining Functions:** Manually invoking sequences of functions.
7.  **Using Memory:** Integrating vector databases (e.g., ChromaDB, Qdrant, Azure AI Search) via Memory Connectors for RAG or conversational memory.
8.  **Implementing Planners:** Understanding how Planners (like Handlebars, Stepwise) automatically orchestrate function calls based on a user goal. Building simple agent-like applications using planners.
9.  **Connectors:** Exploring different AI model connectors and memory connectors.
10. **Debugging & Best Practices:** Tips for debugging Semantic Kernel applications and structuring code effectively.
11. **Project Ideas:** Suggest 1-2 projects using Semantic Kernel (e.g., an email summarizer plugin, a simple agent that uses a native function tool and memory).
12. **Resource Mapping:** Link learning objectives to specific Semantic Kernel documentation pages (concepts, cookbook/examples), relevant GitHub samples, or official blog posts/videos.

Structure the plan logically, focusing on practical coding exercises in [Your Language] and gradually building up to using planners."

---
