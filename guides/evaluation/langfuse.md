# Learning Guide: Langfuse

Langfuse is an open-source observability, analytics, and evaluation platform specifically designed for LLM applications. It helps developers trace, debug, monitor, and evaluate the performance and quality of complex LLM workflows, including agents and RAG pipelines.

**Key Concepts for Agentic AI:**
*   Tracing: Capturing the execution flow of LLM calls, tool usage, and agent steps.
*   Observations: Logging specific events (LLM generations, retrievals, tool calls) with inputs, outputs, costs, and latency.
*   Scores & Evaluations: Annotating traces with scores (manual or automated) to measure quality (e.g., relevance, correctness).
*   Datasets & Testing: Creating datasets from production traces or defining test cases to run evaluations.
*   Debugging UI: Visualizing traces, identifying errors, and analyzing performance bottlenecks.
*   Metrics & Analytics: Monitoring cost, latency, and quality scores over time.
*   Integration: SDKs (Python, JS/TS) for easy integration with frameworks like LangChain, LlamaIndex, OpenAI SDK, etc.

**Core Links:**
*   [GitHub](https://github.com/langfuse/langfuse)
*   [Website](https://langfuse.com/)
*   [Documentation](https://langfuse.com/docs)
*   [Blog](https://langfuse.com/blog)
*   [Discord Community](https://langfuse.com/discord)

---

## LearnLM 1.5 Prompt: Langfuse Learning Plan

*Copy and paste the following prompt into a powerful LLM like Google's LearnLM 1.5 (or similar advanced model) to generate a personalized learning plan.*

**Prompt:**

"Act as an expert AI curriculum designer specializing in LLMOps and evaluation. I am a [Python or JS/TS] developer building complex LLM applications, including agents and RAG systems using frameworks like [Mention your framework, e.g., LangChain, LlamaIndex, OpenAI SDK]. I need to understand how to effectively monitor, debug, and evaluate their performance and quality.

My goal is to learn how to use **Langfuse** (either self-hosted or cloud version) to gain deep observability into my LLM applications.

Please generate a structured, step-by-step learning plan covering:

1.  **Observability Fundamentals:** Why tracing and evaluation are critical for LLM applications (cost, latency, quality, debugging).
2.  **Langfuse Core Concepts:** Traces, Spans, Observations, Events, Scores, Datasets, Generations.
3.  **Setup & Integration:** Setting up Langfuse (cloud sign-up or local Docker deployment) and integrating the SDK (`langfuse-python` or `langfuse-node`) into a basic LLM application (e.g., a simple LangChain chain or OpenAI API call).
4.  **Tracing LLM Calls:** Capturing details of LLM interactions (prompts, completions, model parameters, usage).
5.  **Tracing Agent & RAG Pipelines:** Implementing tracing for more complex flows involving multiple steps, tool calls, and retrievals using framework integrations (e.g., Langfuse callback handlers for LangChain).
6.  **Manual Scoring & Annotation:** Using the Langfuse UI to manually review traces and assign quality scores.
7.  **Programmatic Scoring:** Adding automated scores (e.g., based on keywords, regex, or LLM-based evaluation) to traces via the SDK.
8.  **Datasets & Evaluations:** Creating datasets from traces or manually, defining evaluation metrics, and running evaluations to compare different prompts or models.
9.  **Debugging with Langfuse:** Using the UI to identify errors, analyze latency, compare traces, and understand agent behavior.
10. **Monitoring & Analytics:** Exploring the dashboards for cost, latency, and quality trends.
11. **Resource Mapping:** Link learning objectives to specific Langfuse documentation pages (quickstarts, integrations, concepts), recipes, or blog posts.

Structure the plan logically, emphasizing practical integration of the Langfuse SDK and usage of the UI for analysis."

---
