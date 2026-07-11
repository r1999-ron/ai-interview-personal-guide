# 🤖 AI Engineering Resources — Master Reference

> Curated by Ronak Sengupta | Last updated: 2026
> Everything needed for AI deployment, agentic systems, LLM engineering, RAG, observability, and interview prep — in one place.

---

## 📚 Table of Contents

1. [LLM APIs & Model Providers](#1-llm-apis--model-providers)
2. [Agentic Frameworks & Orchestration](#2-agentic-frameworks--orchestration)
3. [RAG & Vector Databases](#3-rag--vector-databases)
4. [Prompt Engineering](#4-prompt-engineering)
5. [AI Observability & Evaluation](#5-ai-observability--evaluation)
6. [Responsible AI & Guardrails](#6-responsible-ai--guardrails)
7. [MCP (Model Context Protocol)](#7-mcp-model-context-protocol)
8. [Embeddings & Semantic Search](#8-embeddings--semantic-search)
9. [AI Deployment & Infrastructure](#9-ai-deployment--infrastructure)
10. [Learning Paths & Courses](#10-learning-paths--courses)
11. [Papers Worth Reading](#11-papers-worth-reading)
12. [Blogs & Communities](#12-blogs--communities)
13. [Interview Prep — AI Engineering](#13-interview-prep--ai-engineering)
14. [Open Source Projects to Study](#14-open-source-projects-to-study)
15. [Tools & Productivity](#15-tools--productivity)

---

## 1. LLM APIs & Model Providers

### Anthropic (Claude)
| Resource | Link | What it covers |
|---|---|---|
| Claude API Docs | https://docs.anthropic.com | Messages API, tool use, streaming, vision |
| Claude Model Overview | https://docs.anthropic.com/en/docs/about-claude/models | Sonnet, Haiku, Opus — when to use each |
| Tool Use Guide | https://docs.anthropic.com/en/docs/build-with-claude/tool-use | Function calling, tool schemas, multi-tool |
| Prompt Engineering Guide | https://docs.anthropic.com/en/docs/build-with-claude/prompt-engineering/overview | Official Anthropic PE guide |
| Extended Thinking | https://docs.anthropic.com/en/docs/build-with-claude/extended-thinking | Claude's reasoning/thinking mode |
| Anthropic Cookbook | https://github.com/anthropic-ai/anthropic-cookbook | Practical code examples |

### OpenAI (GPT)
| Resource | Link | What it covers |
|---|---|---|
| OpenAI API Docs | https://platform.openai.com/docs | GPT-4o, function calling, assistants |
| Function Calling | https://platform.openai.com/docs/guides/function-calling | Tool use with OpenAI models |
| OpenAI Cookbook | https://github.com/openai/openai-cookbook | Code examples and patterns |
| Structured Outputs | https://platform.openai.com/docs/guides/structured-outputs | JSON mode, schema enforcement |

### Google (Gemini)
| Resource | Link | What it covers |
|---|---|---|
| Gemini API Docs | https://ai.google.dev/gemini-api/docs | Gemini Pro, Flash, multimodal |
| Google AI Studio | https://aistudio.google.com | Prototyping and testing Gemini |
| Vertex AI | https://cloud.google.com/vertex-ai | Enterprise Gemini deployment |

### Microsoft (Copilot / Azure OpenAI)
| Resource | Link | What it covers |
|---|---|---|
| Azure OpenAI | https://learn.microsoft.com/en-us/azure/ai-services/openai | Enterprise OpenAI on Azure |
| Microsoft Copilot Studio | https://www.microsoft.com/en-us/microsoft-copilot/microsoft-copilot-studio | Building Copilot agents |
| Semantic Kernel | https://learn.microsoft.com/en-us/semantic-kernel | Microsoft's AI orchestration SDK |

---

## 2. Agentic Frameworks & Orchestration

### LangChain
| Resource | Link | What it covers |
|---|---|---|
| LangChain Docs | https://python.langchain.com/docs | Chains, agents, tools, memory |
| LangChain Expression Language | https://python.langchain.com/docs/expression_language | LCEL — composable chains |
| LangChain Tools | https://python.langchain.com/docs/integrations/tools | Built-in tool integrations |
| LangSmith | https://smith.langchain.com | Tracing, eval, observability for LangChain |

### LangGraph
| Resource | Link | What it covers |
|---|---|---|
| LangGraph Docs | https://langchain-ai.github.io/langgraph | Stateful graph-based agents |
| LangGraph Quickstart | https://langchain-ai.github.io/langgraph/tutorials/introduction | Build your first LangGraph agent |
| LangGraph Checkpointing | https://langchain-ai.github.io/langgraph/concepts/persistence | State persistence and resumability |
| Multi-Agent with LangGraph | https://langchain-ai.github.io/langgraph/tutorials/multi_agent/multi-agent-collaboration | Multi-agent patterns |

### Other Frameworks
| Framework | Link | Best for |
|---|---|---|
| CrewAI | https://docs.crewai.com | Role-based multi-agent teams |
| AutoGen | https://microsoft.github.io/autogen | Microsoft's multi-agent framework |
| Haystack | https://docs.haystack.deepset.ai | NLP pipelines and RAG |
| DSPy | https://dspy.ai | Programmatic prompt optimization |
| Phidata | https://docs.phidata.com | Agent building with memory and tools |

---

## 3. RAG & Vector Databases

### RAG Fundamentals
| Resource | Link |
|---|---|
| RAG Paper (original) | https://arxiv.org/abs/2005.11401 |
| Advanced RAG Techniques | https://arxiv.org/abs/2312.10997 |
| RAG vs Fine-tuning | https://arxiv.org/abs/2312.05934 |
| Chunking Strategies Guide | https://www.pinecone.io/learn/chunking-strategies |

### Vector Databases
| Database | Docs | Best for |
|---|---|---|
| **Milvus** | https://milvus.io/docs | High-scale, hybrid search (BGE-M3) |
| **FAISS** | https://faiss.ai | In-memory, fast similarity search |
| Pinecone | https://docs.pinecone.io | Managed, easy to get started |
| Weaviate | https://weaviate.io/developers/weaviate | Hybrid search, multi-modal |
| Qdrant | https://qdrant.tech/documentation | Rust-based, fast filtering |
| ChromaDB | https://docs.trychroma.com | Lightweight, local dev |
| pgvector | https://github.com/pgvector/pgvector | Vector search in PostgreSQL |

### Embedding Models
| Model | Provider | Dimensions | Notes |
|---|---|---|---|
| text-embedding-3-small | OpenAI | 1536 | Cost-effective, good quality |
| text-embedding-3-large | OpenAI | 3072 | Best OpenAI quality |
| BGE-M3 | BAAI/HuggingFace | 1024 | Hybrid dense+sparse, multilingual |
| nomic-embed-text | Nomic | 768 | Open source, strong performance |
| voyage-3 | Voyage AI | 1024 | Strong retrieval quality |
| Gemini text-embedding | Google | 768 | Good for Gemini-based stacks |

---

## 4. Prompt Engineering

### Official Guides
| Resource | Link |
|---|---|
| Anthropic Prompt Engineering Guide | https://docs.anthropic.com/en/docs/build-with-claude/prompt-engineering/overview |
| OpenAI Prompt Engineering Guide | https://platform.openai.com/docs/guides/prompt-engineering |
| Google Prompt Design Guide | https://ai.google.dev/gemini-api/docs/prompting-strategies |
| DAIR.AI Prompt Engineering Guide | https://www.promptingguide.ai |

### Key Techniques
| Technique | Description | When to use |
|---|---|---|
| Zero-shot | No examples, direct instruction | Simple, well-defined tasks |
| Few-shot | 2-5 input/output examples | Nuanced classification, style |
| Chain-of-Thought (CoT) | Ask model to reason step-by-step | Multi-step reasoning, math |
| ReAct | Reason + Act loop | Agentic tool-calling tasks |
| Self-consistency | Sample multiple outputs, take majority | High-stakes single decisions |
| Constitutional AI | Define principles, check against them | Responsible AI enforcement |
| Role prompting | Assign persona to model | Domain-specific behavior |
| Output schemas | Force structured JSON/XML output | Downstream parsing reliability |

### System Prompt Structure (7 Components)
```
1. Role / Persona Definition
2. Task Definition / Classification Taxonomy  
3. Explicit Decision Rules / Priority Order
4. Tool-Use Instructions (explain before + after each call)
5. Output Format Specification
6. Constraints & Guardrails
7. Few-Shot Examples (sparingly)
```

---

## 5. AI Observability & Evaluation

### Observability Platforms
| Tool | Link | What it covers |
|---|---|---|
| LangSmith | https://smith.langchain.com | LangChain tracing, eval, datasets |
| Weights & Biases | https://wandb.ai | ML experiment tracking, LLM monitoring |
| Arize AI | https://arize.com | LLM observability, drift detection |
| Helicone | https://www.helicone.ai | LLM request logging, cost tracking |
| Braintrust | https://www.braintr.us | Eval platform for LLM apps |
| Phoenix (Arize) | https://phoenix.arize.com | Open-source LLM observability |
| Langfuse | https://langfuse.com | Open-source LLM observability |

### What to Observe in Production Agents
```
Execution layer:
  ✓ Tool call sequence (what tools were called, in what order)
  ✓ Tool inputs and outputs (what was passed, what came back)
  ✓ LLM call latency (per step and total)
  ✓ Token usage (input/output per call)
  ✓ Stop reason (tool_use vs end_turn vs max_tokens)

Quality layer:
  ✓ Hallucination patterns (claims not grounded in context)
  ✓ Grounding failures (answer not supported by retrieved docs)
  ✓ Escalation rate (% cases sent to human)
  ✓ Confidence distribution (% high/medium/low confidence decisions)
  ✓ Reasoning quality (does the chain of thought match the conclusion)

Business layer:
  ✓ Task completion rate (fully automated vs. escalated)
  ✓ Agreement rate with ground truth (in shadow mode)
  ✓ Cost per decision (total LLM cost / tasks processed)
```

### Evaluation Frameworks
| Framework | Link | Type |
|---|---|---|
| RAGAS | https://docs.ragas.io | RAG-specific eval metrics |
| DeepEval | https://docs.confident-ai.com | General LLM eval framework |
| TruLens | https://www.trulens.org | LLM app eval with feedback functions |
| Promptfoo | https://www.promptfoo.dev | Prompt testing and red-teaming |
| OpenAI Evals | https://github.com/openai/evals | OpenAI's eval framework |

### LLM-as-Judge Pattern
```python
JUDGE_PROMPT = """Score this response 1-5 on:
- Accuracy: correct answer to the question?
- Groundedness: supported by context, not hallucinated?
- Relevance: directly addresses what was asked?

Return ONLY JSON: {"accuracy": N, "groundedness": N, 
                   "relevance": N, "reasoning": "..."}

Question: {question}
Context: {context}  
Response: {response}"""
```

---

## 6. Responsible AI & Guardrails

### Key Concepts
| Concept | Description |
|---|---|
| Prompt Injection | Adversarial inputs that override system instructions |
| Hallucination | Model generates plausible but false information |
| Grounding | Anchoring responses to retrieved/verified context |
| PII Leakage | Personal data appearing in model outputs or logs |
| Jailbreaking | Bypassing model safety restrictions |
| Data Poisoning | Corrupting training/retrieval data to influence outputs |

### Guardrail Layers
```
Layer 1 — Input guardrails (before LLM call):
  • PII detection and redaction
  • Prompt injection detection
  • Input schema validation
  • Content filtering

Layer 2 — Prompt guardrails (system prompt design):
  • Explicit scope boundaries ("only answer questions about X")
  • Escalation rules ("if uncertain, say I don't know")
  • Conservative defaults ("flag for human review when...")

Layer 3 — Output guardrails (after LLM response):
  • PII scan on generated output
  • Off-topic detection
  • Groundedness check (is answer supported by context?)
  • Schema validation on structured outputs

Layer 4 — Action guardrails (before tool execution):
  • Permission tiers (read-only vs. low-risk write vs. high-risk write)
  • Confirmation required for high-risk actions
  • Audit logging of all agent actions
```

### Guardrail Tools
| Tool | Link |
|---|---|
| Guardrails AI | https://www.guardrailsai.com |
| NeMo Guardrails (NVIDIA) | https://github.com/NVIDIA/NeMo-Guardrails |
| Llama Guard | https://ai.meta.com/research/publications/llama-guard |
| Microsoft PyRIT | https://github.com/Azure/PyRIT |

---

## 7. MCP (Model Context Protocol)

| Resource | Link |
|---|---|
| MCP Official Docs | https://modelcontextprotocol.io |
| MCP Specification | https://spec.modelcontextprotocol.io |
| Anthropic MCP Intro | https://docs.anthropic.com/en/docs/build-with-claude/mcp |
| MCP Python SDK | https://github.com/modelcontextprotocol/python-sdk |
| MCP TypeScript SDK | https://github.com/modelcontextprotocol/typescript-sdk |
| MCP Server Examples | https://github.com/modelcontextprotocol/servers |

### MCP Concepts
```
MCP Server: exposes tools, resources, and prompts to AI agents
MCP Client: the AI application that connects to MCP servers
Tools: functions the model can call (like function calling)
Resources: data the model can read (files, DB records, APIs)
Prompts: reusable prompt templates exposed via MCP
Transport: stdio (local) or SSE (remote HTTP)
```

---

## 8. Embeddings & Semantic Search

### Understanding Embeddings
```
Key facts:
  • Embeddings are dense vectors where meaning = geometry
  • Cosine similarity measures angle (direction), not magnitude
  • More dimensions ≠ better retrieval — eval on your data
  • Different models = incompatible vector spaces (can't mix)
  • Model migration requires full re-embedding of corpus

Distance metrics:
  • Cosine similarity: best for semantic search (direction matters)
  • Dot product: faster, biased toward high-magnitude vectors  
  • Euclidean: sensitive to magnitude, less common for text
```

### Choosing Embedding Dimensions
| Dimensions | Use case | Trade-off |
|---|---|---|
| 384 | Narrow domain, speed-critical | Lower quality, cheapest |
| 768 | Most production RAG systems | Sweet spot quality/cost |
| 1536 | Broad domain, multilingual | Better quality, 2x cost |
| 3072 | Highest precision needs | Diminishing returns, expensive |

### Chunking Strategy Comparison
| Strategy | Best for | Trade-off |
|---|---|---|
| Fixed-size (512 chars) | Simple, fast | Can cut mid-sentence |
| Recursive (paragraph→sentence→word) | Most documents | Best default choice |
| Semantic (embedding-based) | High-quality retrieval | Expensive, slower |
| Document-structure (headers, sections) | Structured docs (PDFs, markdown) | Requires parsing |

---

## 9. AI Deployment & Infrastructure

### Deployment Stack Pattern
```
Agent (FastAPI/Flask)
    ↓
Docker container
    ↓
Kubernetes (production) or Railway/Render (pilot/MVP)
    ↓
CI/CD pipeline:
  commit → eval suite → build → staging → canary → prod
    ↓
Observability: traces + metrics + alerts
```

### Key Deployment Considerations
```
Stateless agents:    each request independent → safe to scale horizontally
Prompt versioning:   Git + eval gate + staged rollout (same as code)
Rate limiting:       LLM API limits hit before compute limits at scale
Checkpointing:       LangGraph + Redis → resume failed runs, don't restart
Context window:      monitor P95 token usage, alert before hitting ceiling
Cost tracking:       tokens × price per token per agent type
```

### Infrastructure Tools
| Tool | Purpose | Link |
|---|---|---|
| FastAPI | Python async API framework | https://fastapi.tiangolo.com |
| Docker | Containerization | https://docs.docker.com |
| Kubernetes | Container orchestration | https://kubernetes.io/docs |
| KEDA | K8s event-driven autoscaling | https://keda.sh |
| Railway | Simple container deployment | https://railway.app |
| Redis | State/cache/checkpointing | https://redis.io |
| Kafka | Event streaming | https://kafka.apache.org/documentation |

---

## 10. Learning Paths & Courses

### Certifications (Verified)
| Course | Provider | Link |
|---|---|---|
| Building with the Claude API | Anthropic | https://www.anthropic.com/learn |
| Introduction to MCP | Anthropic | https://www.anthropic.com/learn |
| Generative AI for Software Development | DeepLearning.AI / Coursera | https://www.coursera.org |

### Recommended Courses
| Course | Provider | Link | Level |
|---|---|---|---|
| LangChain for LLM Application Development | DeepLearning.AI | https://learn.deeplearning.ai | Beginner |
| Building Agentic RAG with LlamaIndex | DeepLearning.AI | https://learn.deeplearning.ai | Intermediate |
| Multi AI Agent Systems with CrewAI | DeepLearning.AI | https://learn.deeplearning.ai | Intermediate |
| LangGraph: Build Stateful AI Agents | DeepLearning.AI | https://learn.deeplearning.ai | Intermediate |
| LLMOps | DeepLearning.AI | https://learn.deeplearning.ai | Advanced |
| Evaluating and Debugging Generative AI | DeepLearning.AI | https://learn.deeplearning.ai | Advanced |
| Building Production-Ready RAG | Weights & Biases | https://www.wandb.courses | Advanced |

### Free Learning Resources
| Resource | Link | What it covers |
|---|---|---|
| fast.ai | https://www.fast.ai | Practical deep learning |
| Hugging Face Course | https://huggingface.co/learn | Transformers, fine-tuning |
| LLM University (Cohere) | https://docs.cohere.com/docs/llmu | LLM fundamentals |
| Prompt Engineering Guide | https://www.promptingguide.ai | Comprehensive PE reference |
| Chip Huyen's AI Engineering | https://huyenchip.com | Production AI systems |

---

## 11. Papers Worth Reading

### Foundational
| Paper | Year | Why it matters |
|---|---|---|
| Attention Is All You Need | 2017 | Transformer architecture — foundation of all LLMs |
| BERT | 2018 | Bidirectional transformers, embeddings |
| GPT-3 | 2020 | Few-shot learning, scale |
| RAG (Lewis et al.) | 2020 | Original RAG paper |
| Constitutional AI | 2022 | Anthropic's RLHF + principles approach |

### Agentic Systems
| Paper | Year | Why it matters |
|---|---|---|
| ReAct: Synergizing Reasoning and Acting | 2022 | Foundation of ReAct agent pattern |
| Toolformer | 2023 | LLMs that learn to use tools |
| HuggingGPT | 2023 | Multi-model task planning |
| AgentBench | 2023 | Benchmarking LLM agents |
| LLM-as-Judge | 2023 | Using LLMs to evaluate LLM outputs |

### RAG & Retrieval
| Paper | Year | Why it matters |
|---|---|---|
| REALM | 2020 | Retrieval-augmented language models |
| RETRO | 2021 | Retrieval-enhanced transformers |
| Self-RAG | 2023 | Adaptive retrieval — when to retrieve |
| RAGAS | 2023 | Evaluation framework for RAG pipelines |
| HyDE | 2022 | Hypothetical document embeddings |

---

## 12. Blogs & Communities

### Must-Read Blogs
| Blog | Link | Best for |
|---|---|---|
| Chip Huyen | https://huyenchip.com | Production AI, MLOps, AI engineering |
| Sebastian Raschka | https://sebastianraschka.com | LLMs, fine-tuning, practical ML |
| Lilian Weng (OpenAI) | https://lilianweng.github.io | Deep technical posts on agents, RAG |
| Eugene Yan | https://eugeneyan.com | Applied ML, RecSys, production systems |
| Simon Willison | https://simonwillison.net | LLM news, prompt injection, practical AI |
| The Batch (DeepLearning.AI) | https://www.deeplearning.ai/the-batch | Weekly AI news digest |
| Hugging Face Blog | https://huggingface.co/blog | Model releases, research |
| Anthropic Research | https://www.anthropic.com/research | Claude, interpretability, safety |

### Communities
| Community | Link |
|---|---|
| r/MachineLearning | https://reddit.com/r/MachineLearning |
| r/LocalLLaMA | https://reddit.com/r/LocalLLaMA |
| Hugging Face Forums | https://discuss.huggingface.co |
| LangChain Discord | https://discord.gg/langchain |
| AI Engineer Foundation | https://www.aieng.community |

---

## 13. Interview Prep — AI Engineering

### 📦 Curated Interview Prep Resources

| Resource | Link | What it covers |
|---|---|---|
| AI Interview Mastery Bundle | https://aidemy.trainercentralsite.in/clientapp/app/course/23022000000014019/course-details?previousPage=5 | Comprehensive AI interview preparation course |
| Agentic AI Problems | https://www.agenticprep.io/#preview | Practice problems specifically for agentic AI interviews |
| AI System Design (GitHub) | https://github.com/JoshithReddyAleti/AI_Engineer_Interview_Prep/tree/main | AI engineer system design patterns and prep material |

---

### Core Topics to Master
```
Agentic Systems:
  ✓ ReAct loop vs. DAG — when to use each
  ✓ Tool-calling: schema design, validation, retry logic
  ✓ State management across multi-step agents
  ✓ Multi-agent architectures: orchestrator + specialists
  ✓ LangGraph checkpointing for fault tolerance

RAG & Retrieval:
  ✓ Chunking strategies and trade-offs
  ✓ Embedding models: dimensions, distance metrics
  ✓ Hybrid search (dense + sparse)
  ✓ Retrieval failure modes and mitigations
  ✓ Re-ranking strategies

Prompt Engineering:
  ✓ System prompt structure (7 components)
  ✓ Temperature, top_p, max_tokens trade-offs
  ✓ Hallucination mitigation techniques
  ✓ Prompt versioning and regression eval

Production & Deployment:
  ✓ Context window management strategies
  ✓ Token optimization techniques
  ✓ Observability: what to trace, what to alert on
  ✓ Prompt CI/CD pipeline
  ✓ Scaling: K8s + multi-agent = both needed

Responsible AI:
  ✓ PII detection and redaction
  ✓ Prompt injection detection
  ✓ Guardrail layers (input/prompt/output/action)
  ✓ Human escalation design
  ✓ Audit trails for agent decisions
```

### Common Interview Questions (AI Deployment)
```
"Walk me through the most complex AI system you've built."
"How do you handle tool-call failures in an agentic loop?"
"Your agent works in dev but fails in production — debug it."
"Would you always use the largest/most capable model?"
"How do you decide when a problem needs an agent vs. a rule?"
"How do you test a prompt? What's your eval framework?"
"How would you scale this to 10x volume?"
"What breaks first if you scale to many concurrent users?"
"What does responsible AI mean in your day-to-day work?"
"How would you version prompts in a production system?"
```

### Case Study Framework (5 Steps)
```
1. SCOPE    — clarify assumptions before designing
2. TOOLS    — define inputs, tool signatures, outputs
3. FLOW     — control flow, confidence gates, human escalation
4. FAILURES — name failure modes before interviewer asks
5. ROLLOUT  — shadow mode → graduated rollout → monitoring
```

---

## 14. Open Source Projects to Study

| Project | Link | Why study it |
|---|---|---|
| LangChain | https://github.com/langchain-ai/langchain | Agentic orchestration patterns |
| LangGraph | https://github.com/langchain-ai/langgraph | Stateful graph agent design |
| AutoGPT | https://github.com/Significant-Gravitas/AutoGPT | Early autonomous agent reference |
| MemGPT | https://github.com/cpacker/MemGPT | Long-term memory for agents |
| DSPy | https://github.com/stanfordnlp/dspy | Programmatic prompt optimization |
| Guardrails AI | https://github.com/guardrails-ai/guardrails | Output validation patterns |
| LlamaIndex | https://github.com/run-llama/llama_index | RAG pipeline patterns |
| RAGAS | https://github.com/explodinggradients/ragas | RAG evaluation framework |
| Promptfoo | https://github.com/promptfoo/promptfoo | Prompt testing CLI |
| Langfuse | https://github.com/langfuse/langfuse | Open-source LLM observability |

---

## 15. Tools & Productivity

### Development Tools
| Tool | Purpose | Link |
|---|---|---|
| Claude Code | AI-powered terminal coding | https://claude.ai/code |
| Cursor | AI code editor | https://cursor.sh |
| GitHub Copilot | In-editor code completion | https://github.com/features/copilot |
| Aider | AI pair programming in terminal | https://aider.chat |

### Prototyping & Testing
| Tool | Purpose | Link |
|---|---|---|
| AI Studio (Google) | Test Gemini models | https://aistudio.google.com |
| Claude.ai | Test Claude models | https://claude.ai |
| OpenAI Playground | Test GPT models | https://platform.openai.com/playground |
| LangSmith Playground | Test and trace LangChain | https://smith.langchain.com |
| Promptfoo | Test prompts via CLI | https://www.promptfoo.dev |

### Reference Cheatsheets
```
Key API parameters:
  temperature    : 0.0 (deterministic) → 1.0 (creative)
  top_p          : nucleus sampling threshold
  top_k          : restrict to top k tokens
  max_tokens     : output length cap (cost + latency control)
  stop_sequences : stop generation on these strings

Context window sizes (approx.):
  Claude 3.5 Sonnet  : 200K tokens
  GPT-4o             : 128K tokens
  Gemini 1.5 Pro     : 1M tokens
  Gemini 2.0 Flash   : 1M tokens

Token cost rule of thumb:
  ~1 token ≈ 0.75 words (English)
  1 page of text ≈ 500-750 tokens
  1K tokens ≈ $0.001–$0.015 depending on model
```

---

## 🔖 Quick Reference — Patterns I Use Daily

### Retry with Exponential Backoff
```python
import time, random

def call_with_retry(fn, max_retries=4, base_delay=1.0):
    for attempt in range(max_retries):
        try:
            return fn()
        except Exception as e:
            if attempt == max_retries - 1:
                raise
            delay = base_delay * (2 ** attempt) + random.uniform(0, 1)
            time.sleep(delay)
```

### Cosine Similarity from Scratch
```python
import math

def cosine_similarity(a, b):
    dot = sum(x * y for x, y in zip(a, b))
    mag_a = math.sqrt(sum(x**2 for x in a))
    mag_b = math.sqrt(sum(x**2 for x in b))
    return dot / (mag_a * mag_b)
```

### Tool Call Handler (Claude API)
```python
def handle_tool_call(tool_name, tool_input, tool_registry):
    if tool_name not in tool_registry:
        return {"error": f"Unknown tool: {tool_name}"}
    try:
        return {"result": tool_registry[tool_name](**tool_input)}
    except Exception as e:
        return {"error": str(e)}
```

### LLM-as-Judge
```python
def judge(question, response, context, client, model):
    prompt = f"""Score 1-5 on accuracy and groundedness.
Return ONLY JSON: {{"accuracy": N, "groundedness": N, "reasoning": "..."}}
Question: {question}
Context: {context}
Response: {response}"""
    result = client.messages.create(
        model=model, max_tokens=200,
        messages=[{"role": "user", "content": prompt}]
    )
    return json.loads(result.content[0].text)
```

### PII Detection + Redaction
```python
import re

PII_PATTERNS = {
    "email": r"[\w.+-]+@[\w-]+\.[a-zA-Z]{2,}",
    "phone": r"\b\d{3}[-.]?\d{3}[-.]?\d{4}\b",
    "ssn":   r"\b\d{3}-\d{2}-\d{4}\b"
}

def redact_pii(text):
    for label, pattern in PII_PATTERNS.items():
        text = re.sub(pattern, f"[{label.upper()}_REDACTED]", text)
    return text
```

---

*Built and maintained by Ronak Sengupta — Senior AI/Software Engineer*
*GitHub: github.com/r1999-ron | Blog: medium.com/@ronaksengupta*
