# awesome-llm-tools

> A curated directory of essential LLM tools spanning the full stack: from model preparation and quantization to inference engines, local agents, agent frameworks, RAG pipelines, vector databases, fine-tuning, and more.

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

---

## Table of Contents

1. [Local Agents](#1-local-agents)
   1. [Coding Agents & IDE Extensions](#coding-agents--ide-extensions)
   2. [Autonomous Agents](#autonomous-agents)
   3. [AI Browsers](#ai-browsers)
   4. [Low-code & Visual Flow](#low-code--visual-flow)
   5. [Research & Knowledge Agents](#research--knowledge-agents)
   6. [Computer Use & OS Agents](#computer-use--os-agents)
   7. [Audio / Voice Agents](#audio--voice-agents)
   8. [General-Purpose Local Agents](#general-purpose-local-agents)
2. [Libraries & Frameworks](#2-libraries--frameworks)
   1. [Python](#python)
   2. [JavaScript / TypeScript](#javascript--typescript)
   3. [Java](#java)
   4. [Kotlin](#kotlin)
   5. [Go](#go)
   6. [Rust](#rust)
3. [Prompt Optimization](#3-prompt-optimization)
4. [Context Optimization](#4-context-optimization)
5. [Agent Memory](#5-agent-memory)
6. [RAG Pipelines](#6-rag-pipelines)
7. [Vector Databases](#7-vector-databases)
8. [Inference Engines](#8-inference-engines)
   1. [Desktop / Local](#desktop--local)
   2. [Server / Production](#server--production)
9. [Fine-Tuning](#9-fine-tuning)
   1. [Training Frameworks](#training-frameworks)
   2. [PEFT Methods](#peft-methods-techniques)
   3. [Data & Alignment Tools](#data--alignment-tools)
10. [Model Preparation & Quantization](#10-model-preparation--quantization)
11. [Benchmarks & Leaderboards](#11-benchmarks--leaderboards)
12. [Miscellaneous](#12-miscellaneous)
13. [Related Resources](#13-related-resources)

---

## 1. Local Agents

### Coding Agents & IDE Extensions

| Tool | Type | Editor | Local LLM? | Notes |
|------|------|--------|------------|-------|
| [Continue](https://github.com/continuedev/continue) | Extension | VS Code / JetBrains | ✅ Native | Best open-source local AI coding assistant |
| [Cursor](https://cursor.com) | IDE Fork | VS Code | ⚠️ Via proxy | AI-first IDE; local LLMs via ngrok workaround |
| [Windsurf](https://codeium.com/windsurf) | IDE Fork | VS Code | ⚠️ Partial | Codeium's agentic IDE |
| [Aider](https://github.com/Aider-AI/aider) | CLI Agent | Terminal | ✅ Ollama/Llama.cpp | AI pair programmer in the terminal |
| [Cline](https://github.com/cline/cline) | Extension | VS Code | ✅ OpenAI-compat | Autonomous coding agent in VS Code |
| [KiloCode](https://github.com/Kilo-Org/kilocode) | Extension | VS Code / JetBrains / CLI | ✅ Local | Open-source; supports many local & cloud LLMs |
| [OpenCode](https://github.com/opencode-ai/opencode) | CLI Agent | Terminal | ✅ 75+ providers | Go-based TUI agent with LSP, Git-context; 26k+ stars |
| [Kiro](https://kiro.dev) | IDE | Standalone (Code OSS) | ⚠️ Cloud (Bedrock) | AWS's spec-driven agentic IDE; agent hooks & steering |
| [Antigravity](https://antigravity.dev) | In-editor Agent | VS Code / JetBrains | ✅ Via API | Google DeepMind AI coding assistant |
| [Qoder](https://qoder.ai) | IDE | Standalone | ⚠️ Cloud (multi-model) | Alibaba's agentic IDE; repo-scale context, Repo Wiki, Quest mode |
| [Copilot (GitHub)](https://github.com/features/copilot) | Extension | VS Code / JetBrains / Neovim | ❌ Cloud only | Industry standard; cloud-only |
| [Cody (Sourcegraph)](https://sourcegraph.com/cody) | Extension | VS Code / JetBrains | ✅ Via API | Enterprise code search + AI |
| [Tabby](https://github.com/TabbyML/tabby) | Self-hosted | VS Code / JetBrains / Vim | ✅ Self-hosted | Self-hosted coding assistant server |
| [Fauxpilot](https://github.com/fauxpilot/fauxpilot) | Self-hosted | VS Code (Copilot compat) | ✅ Self-hosted | Open-source GitHub Copilot alternative |
| [Void](https://github.com/voideditor/void) | IDE Fork | VS Code | ✅ Native | Open-source Cursor alternative |
| [Ghostwriter](https://replit.com/ai) | IDE Extension | Replit | ❌ Cloud | Replit's AI-powered pair programmer |
| [Amazon Q](https://aws.amazon.com/q/) | Extension / AWS | VS Code / JetBrains | ❌ Cloud | AWS's generative AI assistant for coding and automation |
| [Tabnine](https://www.tabnine.com/) | Extension | VS Code / JetBrains | ✅ Local | Enterprise-grade local/cloud AI code completions |
| [TurboPilot](https://github.com/ravenscroftj/turbopilot) | Self-hosted | VS Code (Copilot compat) | ✅ Local | Self-hosted Copilot clone using llama.cpp to run Salesforce Codegen |
| [v0](https://v0.dev) | Web Tool | Browser | ❌ Cloud | Prompt-driven UI generation for React and Next.js by Vercel |
| [Lovable](https://lovable.dev) | Web Tool | Browser | ❌ Cloud | Conversational full-stack app generation from natural language |
| [Warp](https://www.warp.dev/) | AI Terminal | Terminal | ✅ Local + Cloud | AI-native terminal with natural language commands, agent mode, and team sharing |
| [Warp Oz](https://www.warp.dev/oz) | Autonomous Agent | Terminal | ✅ Cloud | Warp's autonomous terminal agent; runs multi-step tasks end-to-end with full shell context |
| [goose](https://github.com/block/goose) | CLI Agent | Terminal | ✅ Local | Open-source, extensible AI agent that goes beyond code suggestions |
| [Roo-Code](https://github.com/RooCodeInc/Roo-Code) | In-editor Agent | VS Code | ✅ OpenAI-compat | Autonomous coding agent formerly known as Roo-Cline |
| [crush](https://github.com/charmbracelet/crush) | CLI Agent | Terminal | ✅ Local | Glamorous AI coding agent for the terminal by Charm |
| [Plandex](https://github.com/plandex-ai/plandex) | CLI Agent | Terminal | ✅ OpenAI-compat | Long-running terminal agent for complex tasks |
| [SWE-agent](https://github.com/princeton-nlp/SWE-agent) | CLI Agent | Terminal | ✅ Via API | Autonomous GitHub issue solver |
| [OpenHands (OpenDevin)](https://github.com/All-Hands-AI/OpenHands) | Web + CLI | Browser / Terminal | ✅ OpenAI-compat | Full autonomous software engineering agent |
| [kilocode](https://github.com/Kilo-Org/kilocode) | In-editor Agent | VS Code | ✅ Mixed | AI coding assistant for planning, building, and fixing code |
| [humanlayer](https://github.com/humanlayer/humanlayer) | Middleware | API | ✅ Layer | Human-in-the-loop layer for AI agents to solve hard problems in complex codebases |
| [ProxyAI](https://github.com/carlrobertoh/ProxyAI) | IDE Plugin | JetBrains | ✅ Native | Open-source AI copilot for JetBrains IDEs |
| [Claude Code](https://www.anthropic.com/claude-code) | CLI Agent | Terminal | ❌ Cloud (Claude) | Anthropic's terminal agent; code onboarding, PR generation, powerful edits |
| [Jules](https://jules.google/) | Async Agent | GitHub | ❌ Cloud (Gemini) | Google's async coding agent; works in the background on GitHub issues |
| [Browser-Use](https://github.com/browser-use/browser-use) | Browser Agent | Browser | ✅ OpenAI-compat | Enable AI to control your browser; web automation agent |
| [Neovim + llm.nvim](https://github.com/huggingface/llm.nvim) | Plugin | Neovim | ✅ Native | HuggingFace's Neovim LLM plugin |

### Autonomous Agents

Full autonomous agents that can plan, act, use tools, and run 24/7 without constant human supervision.

| Tool | Description | Language | Notes |
|------|-------------|----------|-------|
| [OpenClaw](https://github.com/openclaw-ai/openclaw) | Self-hosted autonomous agent; multi-channel gateway, self-installing tools, persistent memory | TypeScript | 100k+ GitHub stars |
| [TinyClaw](https://github.com/tinyclaw-ai/tinyclaw) | Lightweight personal AI companion; multi-agent team (coder, writer, researcher) with live dashboard & file-based task queue | Python | Personal, multi-channel |
| [OpenFang](https://www.openfang.sh/) | Agent OS: 7 autonomous capability packages, 16 security layers, 40 channel adapters, 30 pre-built agents, MCP & A2A | Rust | Self-hosted |
| [NullClaw](https://github.com/nullclaw/nullclaw) | Fastest, smallest autonomous AI assistant infra; hybrid host + WASM, edge-optimised | Zig | Self-hosted |
| [ZeroClaw](https://github.com/zeroclaw-labs/zeroclaw) | Fast, small autonomous AI assistant infra; deploy anywhere, hot-swap any component | Rust | Self-hosted |
| [SuperAgent](https://github.com/homanp/superagent) | Deploy LLM Agents to production; provides an API for agent creation and management | Node.js | Agent Platform |
| [ix](https://github.com/kreneskyp/ix) | Autonomous GPT-4 agent platform; provides a full-featured UI for agent orchestration | Python | Agent OS |
| [waggledance.ai](https://github.com/agi-merge/waggle-dance) | Concurrent system of AI Agents implementing Plan-Validate-Solve approach | Python | Goal Solving |
| [GPT Pilot](https://github.com/Pythagora-io/gpt-pilot) | Dev tool that writes scalable apps from scratch with developer oversight | Python | Agentic Dev |
| [Davika](https://github.com/stitionai/devika) | Agentic AI software engineer capable of complex coding tasks | Python | Open-source |
| [n8n](https://github.com/n8n-io/n8n) | Multi-agent workflow automation; combines AI nodes with 400+ business process integrations | Node.js | Low-code |
| [Sauna](https://www.sauna.ai) | Context-compounding assistant that learns taste and detects patterns proactively | Python | Personal assistant |
| [AgentMail](https://www.agentmail.to) | Dedicated email inboxes for AI agents to communicate and act on emails | API / Service | Agent Tool |
| [MetaGPT](https://github.com/geekan/MetaGPT) | Multi-agent framework that assigns roles (Product Manager, Architect, Coder) to agents | Python | Software engineering |
| [ChatDev](https://github.com/OpenBMB/ChatDev) | Virtual software company powered by multiple agents; simulates a full dev cycle | Python | Agentic Dev |
| [GPT Prompt Engineer](https://github.com/mshumer/gpt-prompt-engineer) | Automated prompt engineering; generates, tests, and ranks prompts to find the best | Python | Automation |

### AI Browsers

| Tool | Description | Platform |
|------|-------------|----------|
| [Perplexity Comet](https://www.perplexity.ai/comet) | Perplexity's AI-native browser with built-in search intelligence and agentic web interaction | Web / Desktop |
| [Dia](https://www.diabrowser.com/) | AI browser from The Browser Company (makers of Arc); chat with tabs, write, learn, shop with privacy controls | macOS |
| [Browserbase](https://www.browserbase.com/) | Serverless cloud browser infrastructure for AI agents; Playwright, Puppeteer, Selenium at scale with stealth mode | Cloud / API |
| [ChatGPT Atlas](https://chatgpt.com/atlas/) | OpenAI's agentic interface for web-aware tasks and autonomous browsing within ChatGPT | Web |
| [Page Assist](https://github.com/n4ze3m/page-assist) | Browser Extension | Chrome/Firefox | ✅ Local | Use locally running AI models to assist in web browsing via sidebar |
| [nanobrowser](https://github.com/nanobrowser/nanobrowser) | Browser Extension | Chrome | ✅ Local | Open-source Chrome extension for AI-powered web automation |
| [MultiOn](https://www.multion.ai/) | AI browser agent that can book flights, shop, and navigate complex sites autonomously | Cloud / API | Agentic Web |
| [Skyvern](https://github.com/Skyvern-ai/Skyvern) | Browser automation agent using LLMs to automate complex browser-based workflows | Python / Playwright | Open-source |

### Low-code & Visual Flow

| Tool | Type | Description |
| :--- | :--- | :--- |
| [Flowise](https://github.com/FlowiseAI/Flowise) | Visual Flow | Drag & drop UI to build customized LLM flows using LangChainJS |
| [Langflow](https://github.com/logspace-ai/langflow) | Visual Flow | Low-code RAG and agentic workflow designer for Python developers |
| [Dify](https://github.com/langgenius/dify) | App Platform | LLM application development platform with visual orchestration and backend features |
| [Chainlit](https://github.com/Chainlit/chainlit) | UI Framework | Build Python LLM apps with a professional look and feel in minutes |
| [Flock](https://github.com/Onelevenvy/flock) | Low-code | Workflow-based platform for building chatbots, RAG, and coordinating agent teams |
| [DemoGPT](https://github.com/melih-unsal/DemoGPT) | Visual Flow | Create quick demos by just using prompts; applies ToT approach on LangChain docs |

### Research & Knowledge Agents

| Tool | Description | Platform |
|------|-------------|----------|
| [Perplexica](https://github.com/ItzCrazyKns/Perplexica) | AI-powered search engine. An OpenSource alternative to Perplexity AI | Self-hosted |
| [DocsGPT](https://github.com/arc53/docsgpt) | GPT-powered chat for documentation search & assistance | Web |
| [Chaindesk](https://github.com/gmpetrov/databerry) | The no-code platform for semantic search and documents retrieval | Web |
| [Paper QA](https://github.com/whitead/paper-qa) | LLM Chain for answering questions from documents with citations | Python |
| [DB-GPT](https://github.com/csunny/DB-GPT) | Interact with your data and environment privately with local LLMs | Web |
| [gpt-researcher](https://github.com/assafelovic/gpt-researcher) | Autonomous agent designed for comprehensive online research | Python |
| [SurfSense](https://github.com/MODSetter/SurfSense) | Personal knowledge assistant; alternative to NotebookLM / Perplexity / Glean | Self-hosted |
| [open-notebook](https://github.com/lfnovo/open-notebook) | Open-source implementation of NotebookLM with local model support | Web |
| [RD-Agent](https://github.com/microsoft/RD-Agent) | Autonomous agent for automating industrial R&D processes | Python |
| [local-deep-researcher](https://github.com/langchain-ai/local-deep-researcher) | Fully local web research and report writing assistant | Python / LangGraph |
| [maestro](https://github.com/murtaza-nasir/maestro) | AI-powered research application designed to streamline complex tasks | Web |
| [Phind](https://phind.com/) | AI-powered search engine for developers; answers complex technical questions with sources | Web |
| [Metaphor](https://metaphor.systems/) | Language model powered search engine that understands internet-scale context | Web |
| [You.com](https://you.com/) | AI search assistant with customized experiences and strict data privacy | Web |
| [Komo](https://komo.ai/) | AI-powered search engine focused on quick, relevant results | Web |

### Computer Use & OS Agents

| Tool | Description | Platform |
|------|-------------|----------|
| [OmniParser](https://github.com/microsoft/OmniParser) | Pure vision-based GUI agent screen parsing tool | Python / Model |
| [cua](https://github.com/trycua/cua) | Docker container environment specialized for Computer-Use AI agents | Docker |
| [self-operating-computer](https://github.com/OthersideAI/self-operating-computer) | Framework enabling multimodal models to operate a computer keyboard/mouse | Python |
| [Agent-S](https://github.com/simular-ai/Agent-S) | Open agentic framework that uses computers like a human | Python |
| [openwork](https://github.com/different-ai/openwork) | Open-source alternative to Claude Cowork powered by OpenCode | Desktop |
| [mobile-use](https://github.com/minitap-ai/mobile-use) | AI agent that controls Android or iOS devices via natural language | Python |

### Audio / Voice Agents

> For speech/audio **models**, see the companion models repo.

| Tool | Description | Local? | Task |
|------|-------------|--------|------|
| [faster-whisper](https://github.com/SYSTRAN/faster-whisper) | CTranslate2-based Whisper reimplementation; 4× faster with less memory | ✅ | Speech-to-Text |
| [whisper.cpp](https://github.com/ggerganov/whisper.cpp) | C/C++ port of Whisper; runs on CPU with no dependencies | ✅ | Speech-to-Text |
| [Piper](https://github.com/rhasspy/piper) | Fast, local neural text-to-speech engine | ✅ | Text-to-Speech |
| [Kokoro-FastAPI](https://github.com/remsky/Kokoro-FastAPI) | FastAPI wrapper for Kokoro TTS with OpenAI-compatible API | ✅ | Text-to-Speech |
| [Coqui TTS](https://github.com/idiap/coqui-ai-TTS) | Community fork of Coqui TTS toolkit; multi-voice & multilingual | ✅ | Text-to-Speech |
| [SpeechBrain](https://github.com/speechbrain/speechbrain) | All-in-one speech toolkit (ASR, TTS, speaker ID, emotion recognition) | ✅ | Multi-task |
| [Home Assistant Wyoming](https://github.com/rhasspy/wyoming) | Protocol + server for local voice pipelines (STT/TTS/wake-word) | ✅ | Voice Pipeline |
| [Speecht5 (HuggingFace)](https://github.com/microsoft/SpeechT5) | Microsoft's unified speech-text pre-training framework | ✅ | ASR + TTS |
| [Vapi](https://vapi.ai/) | Voice AI platform for building low-latency conversational agents with natural speech | ❌ Cloud | API / Voice |
| [Retell AI](https://www.retellai.com/) | Real-time conversational AI for developers to build natural-sounding voice agents | ❌ Cloud | API / Voice |

### General-Purpose Local Agents

| Tool | Description | Notes |
|------|-------------|-------|
| [Open WebUI](https://github.com/open-webui/open-webui) | Feature-rich self-hosted web UI for Ollama / OpenAI APIs | Tools, RAG, image gen built-in |
| [AnythingLLM](https://github.com/Mintplex-Labs/anything-llm) | All-in-one local AI app with agents, RAG, tools | Desktop + Docker |
| [LibreChat](https://github.com/danny-avila/LibreChat) | Multi-provider AI chat with agents, plugins, RAG | Self-hosted |
| [SillyTavern](https://github.com/SillyTavern/SillyTavern) | Advanced frontend for character-based AI interactions | Self-hosted |
| [Lobe Chat](https://github.com/lobehub/lobe-chat) | Modern design AI chat framework; support for multiple backends, plugins, and RAG | Docker / Vercel |
| [ChatBox](https://github.com/ChatBoxAI/ChatBox) | User-friendly desktop client app for AI models (Ollama, OpenAI, Claude, etc.) | Windows/macOS/Linux |
| [PrivateGPT](https://github.com/zylon-ai/private-gpt) | Production-ready private document Q&A agent | 100% local |
| [Dash (Agno)](https://github.com/agno-agi/dash) | Self-learning data / text-to-SQL agent grounded in 6 layers of context; inspired by OpenAI's internal impl | Built on Agno framework |
| [visual-explainer](https://github.com/nicobailon/visual-explainer) | Agent skill that generates rich HTML pages and slide decks for diagrams, diff reviews, plan audits, and project recaps | Agent skill / tool |

---

## 2. Libraries & Frameworks

### Python

| Framework | Description | Best For |
|-----------|-------------|----------|
| [LangChain](https://github.com/langchain-ai/langchain) | The most widely adopted LLM framework; chains, tools, agents, RAG | Rapid prototyping, complex chains |
| [LangGraph](https://github.com/langchain-ai/langgraph) | Graph-based agent orchestration (state machines) from LangChain team | Deterministic multi-agent workflows |
| [LlamaIndex](https://github.com/run-llama/llama_index) | Data framework for LLM applications; advanced RAG & agents | Data-heavy, enterprise knowledge systems |
| [AutoGen](https://github.com/microsoft/autogen) | Microsoft's async multi-agent conversation framework | Collaborative multi-agent problem solving |
| [CrewAI](https://github.com/crewAIInc/crewAI) | Role-based multi-agent orchestration; fast & standalone | Specialized crew workflows |
| [Pydantic AI](https://github.com/pydantic/pydantic-ai) | Type-safe agent framework by Pydantic team | Production-grade, type-safe pipelines |
| [Agno (Phidata)](https://github.com/agno-agi/agno) | Lightweight, fast multi-modal agent framework | Multi-modal agents with memory & storage |
| [Haystack](https://github.com/deepset-ai/haystack) | Pipeline-based NLP / RAG framework for production | Production NLP & search pipelines |
| [Smolagents](https://github.com/huggingface/smolagents) | Minimal, powerful agents library by Hugging Face | Code agents, tool calling |
| [Atomic Agents](https://github.com/BrainBlend-AI/atomic-agents) | Modular, dependency-injection-based agent framework | Composable, testable agents |
| [CAMEL-AI](https://github.com/camel-ai/camel) | Role-playing communicative multi-agent framework; research and multi-agent systems | Multi-agent Communication |
| [OpenAI Agents SDK](https://github.com/openai/openai-agents-python) | Official OpenAI Python SDK for building agents | OpenAI-native agent workflows |
| [Google ADK](https://google.github.io/adk-docs/) | Google's Agent Development Kit — modular, model-agnostic framework with multi-agent orchestration, rich tool ecosystem, built-in eval | Google Cloud / Gemini agents |
| [aisuite](https://github.com/andrewyng/aisuite) | Simple unified interface to multiple Generative AI providers, by Andrew Ng | Multi-provider prototyping |
| [swarm](https://github.com/openai/swarm) | OpenAI's educational framework for lightweight ergonomic multi-agent orchestration | Learning multi-agent patterns |
| [guidance](https://github.com/guidance-ai/guidance) | Interleave generation, prompting, and logic control in a continuous flow matching LLM processing | Constrained, structured generation |
| [outlines](https://github.com/outlines-dev/outlines) | Library for reliable structured generation (JSON, regex, grammar) from LLMs and diffusers, by dottxt.ai | Structured outputs |
| [Multi-Agent Orchestrator](https://github.com/awslabs/multi-agent-orchestrator) | AWS framework for managing multiple AI agents and complex multi-turn conversations | Enterprise multi-agent systems |
| [rowboat](https://github.com/rowboatlabs/rowboat) | AI-powered multi-agent builder with no-code UI, powered by OpenAI Agents SDK | Rapid agent prototyping |
| [Medusa](https://github.com/FasterDecoding/Medusa) | Framework accelerating LLM generation with multiple decoding heads; no specialized hardware | Inference acceleration |
| [LMQL](https://lmql.ai/) | Programming language for LLMs based on logic programming; enables robust prompting | Advanced Prompting |
| [Griptape](https://github.com/griptape-ai/griptape) | Python framework for AI workflows and pipelines with chain of thought reasoning | Workflows |
| [Embedchain](https://github.com/embedchain/embedchain) | Framework to easily create LLM powered bots over any dataset | RAG Builder |
| [SymbolicAI](https://github.com/Xpitfire/symbolicai) | Neuro-symbolic framework for building applications with LLMs at the core | Hybrid AI |
| [Ludwig](https://github.com/ludwig-ai/ludwig) | Low-code framework for building custom AI models like LLMs and other deep neural networks | Low-code ML |
| **Core Libraries** |
| [transformers](https://github.com/huggingface/transformers) | HuggingFace's flagship model library; 300k+ models, inference & fine-tuning for every major architecture | Foundation library |
| [accelerate](https://github.com/huggingface/accelerate) | HuggingFace library to run PyTorch training/inference on any hardware with minimal code changes | Multi-GPU / mixed-precision |
| [sentence-transformers](https://github.com/UKPLab/sentence-transformers) | Easy-to-use library for state-of-the-art sentence, text, and image embeddings | Embeddings / semantic search |
| [tiktoken](https://github.com/openai/tiktoken) | OpenAI's fast BPE tokenizer; used to count tokens before sending to APIs | Tokenization |
| [openai](https://github.com/openai/openai-python) | Official OpenAI Python SDK | OpenAI API client |
| [anthropic](https://github.com/anthropics/anthropic-sdk-python) | Official Anthropic Python SDK | Claude API client |
| [google-genai](https://github.com/googleapis/python-genai) | Official Google Gen AI Python SDK for Gemini models | Gemini API client |
| [google-adk](https://pypi.org/project/google-adk/) | Google Agent Development Kit Python package | Google ADK agents |
| [llm](https://github.com/simonw/llm) | CLI tool + Python library for running prompts against any LLM; extensible via plugins (Ollama, Claude, Gemini, etc.) | CLI / scripting |

### JavaScript / TypeScript

| Framework | Description | Best For |
|-----------|-------------|----------|
| [LangChain.js](https://github.com/langchain-ai/langchainjs) | Official JS/TS port of LangChain | Full-stack JS LLM apps |
| [LlamaIndex.TS](https://github.com/run-llama/LlamaIndexTS) | TypeScript version of LlamaIndex | RAG in Node/Deno/edge |
| [VoltAgent](https://github.com/voltagent/voltagent) | TypeScript-native open-source agentic framework | TypeScript-first developers |
| [Mastra](https://github.com/mastra-ai/mastra) | TypeScript agent framework with workflows, memory, tools | Modern Node.js AI apps |
| [Vercel AI SDK](https://github.com/vercel/ai) | Full-stack AI toolkit for Next.js / React | AI-powered web UIs |
| [GenKit (Firebase)](https://github.com/firebase/genkit) | Google's framework for production AI flows in JS/TS | Firebase / Google Cloud apps |
| [Bee Agent Framework](https://github.com/i-am-bee/bee-agent-framework) | IBM's open-source TypeScript agent framework | Enterprise TypeScript agents |
| **Core Libraries** |
| [openai](https://github.com/openai/openai-node) | Official OpenAI Node.js / TypeScript SDK | OpenAI API client |
| [anthropic](https://github.com/anthropics/anthropic-sdk-typescript) | Official Anthropic TypeScript SDK | Claude API client |
| [@google/genai](https://github.com/googleapis/js-genai) | Official Google Gen AI JS/TS SDK for Gemini models | Gemini API client |
| [ollama-js](https://github.com/ollama/ollama-js) | Official Ollama JavaScript library | Local model client |
| [ai](https://www.npmjs.com/package/ai) | Vercel AI SDK — stream-first unified API for LLMs, RSC support, tool calling | Universal LLM SDK for JS/TS |
| [genkit](https://www.npmjs.com/package/genkit) | Google's GenKit — production AI flows, plugins, tracing, evaluation | Google Cloud / Firebase AI apps |
| [@google/adk](https://www.npmjs.com/package/@google/adk) | Google Agent Development Kit for Node.js | Google ADK agents |

### Java

| Framework | Description | Best For |
|-----------|-------------|----------|
| [Semantic Kernel](https://github.com/microsoft/semantic-kernel) | Microsoft's cross-language AI SDK | Enterprise, .NET / Java ecosystem |
| [Spring AI](https://github.com/spring-projects/spring-ai) | Spring Framework for AI / LLM integration; prompt chaining, routing, RAG | Spring Boot apps |
| [LangChain4j](https://github.com/langchain4j/langchain4j) | Java port of LangChain; chains, tools, agents, RAG | Java LLM apps |
| [Quarkus AI](https://quarkus.io/ai/) | Official Quarkiverse extension for seamless LangChain4j integration and native compilation | Quarkus / Native AI |
| [Apache Camel AI](https://camel.apache.org/components/next/ai-summary.html) | Enterprise integration components (LangChain4j, DJL) for intelligent flows | Integration / AI Flows |
| [Google ADK Java](https://google.github.io/adk-docs/) | Google's Agent Development Kit for Java — same multi-agent, tool-use capabilities as the Python SDK | Google Cloud / Gemini Java agents |
| **Core Libraries** |
| [DJL (Deep Java Library)](https://github.com/deepjavalibrary/djl) | Amazon's engine-agnostic deep learning library for Java; run HuggingFace & PyTorch models | Java ML inference |
| [openai-java](https://github.com/openai/openai-java) | Official OpenAI Java SDK | OpenAI API client |

### Kotlin

| Framework | Description | Best For |
|-----------|-------------|----------|
| [Koog](https://github.com/JetBrains/koog) | JetBrains' pure-Kotlin agent framework; multiplatform (JVM, Android, iOS, WASM), fault-tolerant with retries & state restore | Enterprise Kotlin / multiplatform agents |
| **Core Libraries** |
| [DJL (Kotlin)](https://github.com/deepjavalibrary/djl) | Amazon's DJL works seamlessly in Kotlin; run PyTorch, ONNX, HuggingFace models on JVM | Kotlin ML inference |
| [Kotlin OpenAI client](https://github.com/aallam/openai-kotlin) | Multiplatform OpenAI API client for Kotlin (JVM, Android, JS, Native) | OpenAI API client |

### Go

| Framework | Description | Best For |
|-----------|-------------|----------|
| [LangChainGo](https://github.com/tmc/langchaingo) | Go port of LangChain; chains, tools, memory, RAG | Go LLM apps |
| [Eino](https://github.com/cloudwego/eino) | ByteDance's LLM framework inspired by LangChain & ADK; reusable components, multi-agent coordination | High-performance Go services |
| [adk-go](https://github.com/google/adk-go) | Google's Agent Development Kit for Go — multi-agent orchestration, tool use, Gemini/Vertex AI integration | Google ADK Go agents |
| **Core Libraries** |
| [go-openai](https://github.com/sashabaranov/go-openai) | Unofficial but most widely used OpenAI Go client; OpenAI, Azure OpenAI support | OpenAI API client |
| [ollama-go](https://github.com/ollama/ollama/tree/main/api) | Official Ollama Go API client | Local model client |

### Rust

| Framework | Description | Best For |
|-----------|-------------|----------|
| [Rig](https://github.com/0xPlaygrounds/rig) | Modular, production-ready Rust library; 20+ providers, 10+ vector stores, WASM support | Performance-critical Rust agents |
| [LLM-Chain](https://github.com/sobelio/llm-chain) | Structured multi-step LLM workflows in Rust; prompt templates, chains, tool calling | Type-safe Rust pipelines |
| **Core Libraries** |
| [candle](https://github.com/huggingface/candle) | HuggingFace's minimalist Rust ML framework; GPU support, WASM-ready, no Python dependency | Rust-native ML inference |
| [async-openai](https://github.com/64bit/async-openai) | Async Rust client for OpenAI API; idiomatic, type-safe | OpenAI API client |
| [ollama-rs](https://github.com/pepperoni21/ollama-rs) | Async Rust client for the Ollama API | Local model client |
| [aichat](https://github.com/sigoden/aichat) | All-in-one Rust CLI with shell integration, RAG, agents, and 20+ LLM providers | CLI / scripting |

---

## 3. Prompt Optimization

Tools for systematic prompt engineering, evaluation, and automated optimization.

| Tool | Description | Approach |
|------|-------------|----------|
| [DSPy](https://github.com/stanfordnlp/dspy) | Stanford's framework for programming (not prompting) LLMs — declarative, auto-optimized | Automatic |
| [PromptFoo](https://github.com/promptfoo/promptfoo) | CLI/CI tool for testing, evaluating, and red-teaming prompts | Evaluation |
| [Langfuse](https://github.com/langfuse/langfuse) | Open-source LLM observability with prompt management, tracing, evals | Monitoring |
| [PromptLayer](https://promptlayer.com) | Prompt versioning, logging, and A/B testing SaaS | Management |
| [LangSmith](https://smith.langchain.com) | LangChain's debugging, testing, and evaluation platform | Evaluation |
| [Promptflow (Azure)](https://github.com/microsoft/promptflow) | Microsoft's end-to-end LLM app development and evaluation | Azure |
| [PromptPerfect](https://promptperfect.jina.ai) | AI-driven auto-optimization of prompts for any model | Automatic |
| [Agenta](https://github.com/agenta-ai/agenta) | Open-source LLM dev platform: prompt playground, evaluation | Evaluation |
| [EvalPlus](https://github.com/evalplus/evalplus) | Rigorous code evaluation framework for LLMs | Code eval |
| [Opik](https://github.com/comet-ml/opik) | Open-source LLM evaluation and tracing by Comet | Evaluation |
| [OPRO](https://github.com/google-deepmind/opro) | Google DeepMind's optimization by prompting — LLM as optimizer | Automatic |
| [TextGrad](https://github.com/zou-group/textgrad) | Automatic differentiation through text for prompt/system optimization | Gradient-based |
| [DeepEval](https://github.com/confident-ai/deepeval) | Unit testing framework for LLMs; test-driven development for RAG & agents | Evaluation |
| [Giskard](https://github.com/Giskard-AI/giskard) | Open-source testing framework for LLMs and ML models; automated red-teaming | Evaluation |

---

## 4. Context Optimization

Tools and techniques for managing, compressing, and optimizing the LLM context window.

| Tool | Description | Technique |
|------|-------------|-----------|
| [LLMLingua](https://github.com/microsoft/LLMLingua) | Microsoft's prompt compression library; removes redundant tokens | Compression |
| [LongLLMLingua](https://github.com/microsoft/LLMLingua) | Extension for long-context scenarios with key information extraction | Compression |
| [Rerankers](https://github.com/AnswerDotAI/rerankers) | Unified interface for cross-encoder rerankers to prioritize context | Reranking |
| [FlashAttention](https://github.com/Dao-AILab/flash-attention) | IO-aware exact attention algorithm; enables longer context efficiently | Kernel optimization |
| [RoPE scaling / YaRN](https://github.com/jquesnelle/yarn) | Context length extension techniques (RoPE NTK, YaRN) | Positional Encoding |
| [LongRoPE](https://github.com/microsoft/LongRoPE) | Microsoft's long-context RoPE extension method | Positional Encoding |
| [Sliding Window Attention](https://github.com/mistralai/mistral-src) | Mistral's local attention mechanism for efficient long contexts | Architecture |
| [Semantic Chunking](https://github.com/aurelio-labs/semantic-chunker) | Context-aware document chunking based on semantic similarity | Chunking |
| [LlamaIndex Context Management](https://docs.llamaindex.ai/en/stable/module_guides/querying/response_synthesizers/) | Built-in context window management in LlamaIndex pipelines | Pipeline |
| [Context Caching (Gemini)](https://cloud.google.com/vertex-ai/generative-ai/docs/context-cache/context-cache-overview) | Reuse prompt prefixes across requests to reduce latency + cost | Caching |
| [claude-context-mode](https://github.com/mksglu/claude-context-mode) | Stops context loss from large outputs; smart snippets, fuzzy search, progressive throttling, subagent routing for Claude | Context Management |
| [LMCache](https://github.com/LMCache/LMCache) | KV Cache sharing layer; share and reuse KV caches across requests for faster inference and higher throughput | Caching |
| [GPTCache](https://github.com/zilliztech/GPTCache) | A Library for Creating Semantic Cache for LLM Queries to reduce costs | Semantic Caching |

---

## 5. Agent Memory

Persistent, long-term, and working memory systems for AI agents.

| Tool | Description | Memory Type | Self-hosted |
|------|-------------|-------------|-------------|
| [Mem0](https://github.com/mem0ai/mem0) | Intelligent memory layer for AI; multi-level (user, session, agent) memory with LLM-based extraction | Semantic + Graph | ✅ |
| [Letta (MemGPT)](https://github.com/letta-ai/letta) | OS-inspired agent memory; tiered main/external context (formerly MemGPT) | Hierarchical + Persistent | ✅ |
| [Zep](https://github.com/getzep/zep) | Temporal knowledge graph memory for assistants; extracts entities & relations | Knowledge Graph | ✅ |
| [Cognee](https://github.com/topoteretes/cognee) | Structured memory with knowledge graphs built from conversation history | Knowledge Graph | ✅ |
| [Memary](https://github.com/kingjulio8238/memary) | Open-source memory system for agents with routing and self-healing | Semantic | ✅ |
| [LangMem](https://github.com/langchain-ai/langmem) | LangChain's long-term memory SDK for LangGraph agents | Semantic | ✅ |
| [Graphiti (Zep)](https://github.com/getzep/graphiti) | Real-time knowledge graph for AI agents from the Zep team | Knowledge Graph | ✅ |
| [R2R (Retrieval to Reasoning)](https://github.com/SciPhi-AI/R2R) | Production-ready RAG + memory system with knowledge graphs | Hybrid | ✅ |
| [ReMemory](https://github.com/agentscope-ai/reme) | Memory Management Kit for agents; compacts history, writes summaries to file, semantic recall via MemorySearch | File + Semantic | ✅ |
| [supermemory](https://github.com/supermemoryai/supermemory) | Personal AI second brain; fast, scalable memory engine and application | Second Brain | ✅ |
| [memU](https://github.com/NevaMind-AI/memU) | Open-source memory framework for AI companions and persona-driven agents | Persona Memory | ✅ |
| [quivr](https://github.com/StanGirard/quivr) | Open-source RAG framework that acts as your generative AI second brain | Second Brain | ✅ |

---

## 6. RAG Pipelines

Frameworks and tools for building Retrieval-Augmented Generation systems.

| Tool | Description | Best For |
|------|-------------|----------|
| [LlamaIndex](https://github.com/run-llama/llama_index) | Data-first framework; 150+ connectors, advanced indexing, sub-question agents | Document-heavy RAG |
| [Haystack](https://github.com/deepset-ai/haystack) | Modular pipeline framework for enterprise RAG & search; 50+ integrations | Production pipelines |
| [LangChain](https://github.com/langchain-ai/langchain) | End-to-end RAG chains with rich integrations and agent-based retrieval | Flexible RAG prototyping |
| [Ragas](https://github.com/explodinggradients/ragas) | Reference-free RAG evaluation (faithfulness, relevance, recall) | RAG Evaluation |
| [TRULENS](https://github.com/truera/trulens) | LLM app evaluation and RAG feedback functions | Evaluation + Observability |
| [FlashRAG](https://github.com/RUC-NLPIR/FlashRAG) | Modular unified framework for reproducible RAG research | Research |
| [Pathway](https://github.com/pathwaycom/pathway) | Real-time streaming RAG pipeline framework | Live data RAG |
| [R2R](https://github.com/SciPhi-AI/R2R) | Production RAG system with hybrid search, knowledge graphs, eval | Production |
| [Cognita](https://github.com/truefoundry/cognita) | Modular, production-ready RAG framework by TrueFoundry | Organized, modular RAG |
| [Verba](https://github.com/weaviate/verba) | Weaviate-powered open-source RAG chatbot | Weaviate + RAG |
| [DSPy](https://github.com/stanfordnlp/dspy) | Declarative RAG pipelines with auto-optimization of retrieval | Optimized RAG |
| [Camel RAG](https://github.com/camel-ai/camel) | RAG tools within the CAMEL multi-agent framework | Multi-agent + RAG |
| [PageIndex](https://github.com/VectifyAI/PageIndex) | Vectorless, reasoning-based RAG; builds a hierarchical document index and uses LLM reasoning over it instead of embeddings | No-vector RAG |
| [GraphRAG](https://github.com/microsoft/graphrag) | Microsoft's graph-based RAG; builds knowledge graph communities and uses hierarchical summarisation for global question answering | Knowledge Graph RAG |
| [HashIndex](https://github.com/JasonHonKL/HashIndex) | Ultra-fast LLM-optimised document indexing without vector search; hash-based retrieval | No-vector RAG |
| [LightRAG](https://github.com/HKUDS/LightRAG) | Dual-level retrieval system combining graph and vector search for deep context awareness | Graph + Vector RAG |
| [vanna](https://github.com/vanna-ai/vanna) | Open-source Python RAG framework for SQL generation and related functionality | Text-to-SQL RAG |
| [graphiti](https://github.com/getzep/graphiti) | Real-time knowledge graph for AI agents with temporal awareness | Knowledge Graph |
| [onyx](https://github.com/onyx-dot-app/onyx) | Enterprise AI platform connected to company docs, apps, and people | Enterprise RAG |
| [crawl4ai](https://github.com/unclecode/crawl4ai) | Open-source web crawler and scraper designed for LLMs and AI agents | Web Crawling |
| [Firecrawl](https://github.com/mendableai/firecrawl) | API to scrape and crawl websites into clean, LLM-ready markdown or structured data | Web Scraper / API |
| [Docling](https://github.com/DS4SD/docling) | IBM's open-source toolkit to transform unstructured documents (PDF, etc.) into structured data for AI | Document Parser |
| [claude-context](https://github.com/zilliztech/claude-context) | Make entire codebase the context for any coding agent | Codebase RAG |
| [pipeshub-ai](https://github.com/pipeshub-ai/pipeshub-ai) | Extensible workplace AI platform for enterprise search and workflow automation | Enterprise RAG |

---

## 7. Vector Databases

Purpose-built stores for high-dimensional vector embeddings.

| Database | Type | Best For | License |
|----------|------|----------|---------|
| [Chroma](https://github.com/chroma-core/chroma) | Open-source, Python-native | Local dev, prototyping, RAG | Apache-2.0 |
| [Qdrant](https://github.com/qdrant/qdrant) | Open-source, Rust-built, cloud option | Production, fast filtering, hybrid search | Apache-2.0 |
| [Milvus](https://github.com/milvus-io/milvus) | Open-source, Kubernetes-scale | Billion-vector scale, enterprise | Apache-2.0 |
| [Weaviate](https://github.com/weaviate/weaviate) | Open-source, GraphQL API | Semantic + GraphQL queries, hybrid search | BSD-3 |
| [pgvector](https://github.com/pgvector/pgvector) | PostgreSQL extension | Existing PostgreSQL users, <1M vectors | PostgreSQL |
| [LanceDB](https://github.com/lancedb/lancedb) | Embedded, serverless, columnar | Serverless RAG, edge apps | Apache-2.0 |
| [zvec](https://github.com/alibaba/zvec) | In-process embedded vector database; lightweight and extremely fast (AliBaba) | Embedded RAG, local search | Apache-2.0 |
| [Faiss](https://github.com/facebookresearch/faiss) | Library, not a DB | Raw ANN search in Python/C++ | MIT |
| [Annoy](https://github.com/spotify/annoy) | Library, memory-mapped | Static indexes, read-heavy | Apache-2.0 |
| [Vespa](https://github.com/vespa-engine/vespa) | Full search engine with vector support | Hybrid text + vector at scale | Apache-2.0 |
| [Marqo](https://github.com/marqo-ai/marqo) | End-to-end multimodal tensor search | Image + text search | SSPL |
| [Turbopuffer](https://turbopuffer.com) | Serverless vector DB on object storage | Low-cost, high-scale cloud | Proprietary |
| **Managed / Cloud** | | | |
| [Pinecone](https://pinecone.io) | Fully managed cloud vector DB | Managed, auto-scaling, <50ms p95 | Proprietary |
| [Zilliz Cloud](https://zilliz.com) | Managed Milvus; enterprise-grade | Managed Milvus | Proprietary |
| [Weaviate Cloud](https://weaviate.io/pricing) | Managed Weaviate | Managed hybrid search | Proprietary |

---

## 8. Inference Engines

### Desktop / Local

Optimized for personal hardware — laptops, workstations, or edge devices.

| Tool | Description | Backends | GUI |
|------|-------------|----------|-----|
| [llama.cpp](https://github.com/ggerganov/llama.cpp) | The foundational C/C++ LLM inference engine; cross-platform CPU+GPU, GGUF format, powers most local tools | CUDA, Metal, Vulkan, ROCm | ✅ Web (built-in server) |
| [Ollama](https://github.com/ollama/ollama) | "Docker for LLMs" — one-command model pull & run, OpenAI-compatible API | llama.cpp, MLX | Web UI via Open WebUI |
| [LM Studio](https://lmstudio.ai) | Polished cross-platform desktop app; model discovery, local server, chat | llama.cpp, MLX | ✅ Native |
| [GPT4All](https://github.com/nomic-ai/gpt4all) | Privacy-first desktop app; curated model library, no GPU required | llama.cpp | ✅ Native |
| [Jan](https://github.com/janhq/jan) | ChatGPT-like open-source desktop app; local-first, extensions | llama.cpp, TensorRT | ✅ Native |
| [koboldcpp](https://github.com/LostRuins/koboldcpp) | Single-binary llama.cpp with a web UI for creative writing & roleplay | llama.cpp | ✅ Web |
| [text-generation-webui](https://github.com/oobabooga/text-generation-webui) | Feature-rich Gradio web UI with multi-backend support (Oobabooga) | llama.cpp, ExLlamaV2, GPTQ, AWQ | ✅ Web |
| [llamafile](https://github.com/Mozilla-Ocho/llamafile) | Single-file executable LLMs that run on any OS without install | llama.cpp | ✅ Web |
| [MLC LLM](https://github.com/mlc-ai/mlc-llm) | Universal LLM deployment framework; targets CPU, GPU, Mobile, WebGPU | TVM | ✅ Web |
| [LocalAI](https://github.com/mudler/LocalAI) | Self-hosted OpenAI-compatible REST API for LLMs, images, audio | llama.cpp, GPU backends | ✅ Web |
| [OpenLLM](https://github.com/bentoml/OpenLLM) | Open-source platform for deploying and operating LLMs in production via BentoML | Multiple | ✅ Web |
| [msty](https://msty.app/) | Simple, clean desktop app for running local and online AI models side-by-side | llama.cpp | ✅ Native |
| [Open Interpreter](https://github.com/KillianLucas/open-interpreter) | Locally running implementation of OpenAI's Code Interpreter; executes code in the terminal | llama.cpp, Ollama | ✅ Terminal |
| [bitnet.cpp](https://github.com/microsoft/BitNet) | Official inference framework for 1-bit LLMs (BitNet b1.58); fast lossless CPU inference | CPU (NPU/GPU coming) | ❌ |
| [PowerInfer](https://github.com/SJTU-IPADS/PowerInfer) | CPU/GPU inference engine exploiting neuron activation locality for faster inference | CUDA + CPU | ❌ |
| [exo](https://github.com/exo-explore/exo) | Distributed inference engine that clusters multiple devices (macOS, Linux) into a single GPU for running frontier models | Metal, CUDA | ✅ Dashboard |
| [distributed-llama](https://github.com/b4rtaz/distributed-llama) | Connect home devices into a powerful cluster to accelerate LLM inference | C++ | ❌ |
| [ik_llama.cpp](https://github.com/ikawrakow/ik_llama.cpp) | llama.cpp fork with additional SOTA quants and improved performance | llama.cpp fork | ❌ |
| [FastFlowLM](https://github.com/FastFlowLM/FastFlowLM) | Optimized inference engine for running LLMs on AMD Ryzen™ AI NPUs | AMD NPU | ❌ |
| [lemonade](https://github.com/lemonade-sdk/lemonade) | Local LLM server with GPU and NPU Acceleration | Multiple | ❌ |

### Server / Production

Designed for high-throughput, multi-user, and production API serving.

| Tool | Description | Key Feature | GPU Support |
|------|-------------|-------------|-------------|
| [vLLM](https://github.com/vllm-project/vllm) | State-of-the-art serving engine with PagedAttention & continuous batching | Highest throughput | NVIDIA, AMD, TPU |
| [TGI (Text Generation Inference)](https://github.com/huggingface/text-generation-inference) | Hugging Face's production-grade Rust/Python server | Flash Attention, tensor parallelism | NVIDIA, AMD, Gaudi |
| [flashinfer](https://github.com/flashinfer-ai/flashinfer) | High-performance kernel library for LLM serving | Kernel optimization | NVIDIA |
| [SGLang](https://github.com/sgl-project/sglang) | Fast structured generation runtime with RadixAttention | Structured outputs | NVIDIA |
| [LiteLLM](https://github.com/BerriAI/litellm) | Unified OpenAI-compatible proxy for 100+ LLM providers | Provider routing | Cloud + Local |
| [Triton Inference Server](https://github.com/triton-inference-server/server) | NVIDIA's enterprise multi-framework model serving | Multi-model, multi-GPU | NVIDIA |
| [Ray Serve](https://github.com/ray-project/ray) | Scalable model serving via Ray distributed framework | Autoscaling | Any |
| [FastChat](https://github.com/lm-sys/FastChat) | Multi-model API server and chat UI (LLM Arena backend) | Multi-model | NVIDIA |
| [Aphrodite Engine](https://github.com/PygmalionAI/aphrodite-engine) | vLLM fork with extra quantization methods and creative writing focus | GPTQ, AWQ, EXL2 | NVIDIA |
| [TensorRT-LLM](https://github.com/NVIDIA/TensorRT-LLM) | NVIDIA's peak-performance compiled inference for Blackwell/Hopper | FP8, NVFP4 | NVIDIA |
| [Llama.cpp server](https://github.com/ggerganov/llama.cpp/tree/master/examples/server) | Built-in OpenAI-compatible HTTP server inside llama.cpp | Cross-platform CPU+GPU | Any |
| [ClawRouter](https://github.com/BlockRunAI/ClawRouter) | Agent-native LLM cost router; 15-dimension classifier routes to cheapest capable model in <1ms, 41+ providers, x402 micropayments | Any | Any |
| [Portkey Gateway](https://github.com/Portkey-AI/gateway) | Unified API for 100+ open & closed-source models with caching, fallbacks, retries, load-balancing, and edge deployment | Any | Any |
| [Nano-vLLM](https://github.com/GeeeekExplorer/nano-vllm) | Lightweight vLLM implementation built from scratch for minimal serving overhead | Least overhead | NVIDIA |
| [gpustack](https://github.com/gpustack/gpustack) | Simple, scalable AI model deployment on GPU clusters; managing multiple nodes easily | Multi-node | NVIDIA/AMD |
| [mini-sglang](https://github.com/sgl-project/mini-sglang) | Lightweight yet high-performance inference framework for LLMs based on SGLang | Fast serving | NVIDIA |
| [vllm-gfx906](https://github.com/nlzy/vllm-gfx906) | vLLM optimized for AMD gfx906 GPUs (Radeon VII, MI50, MI60) | AMD specialized | AMD |
| [llm-scaler](https://github.com/intel/llm-scaler) | Run and scale LLMs on Intel Arc™ Pro B60 GPUs | Intel specialized | Intel |

---


## 9. Fine-Tuning

Frameworks and tools for fine-tuning, alignment, and PEFT methods.

### Training Frameworks

| Tool | Description | Methods | Memory Efficient |
|------|-------------|---------|-----------------|
| [Unsloth](https://github.com/unslothai/unsloth) | 2–5× faster fine-tuning; 70–90% less VRAM via custom CUDA/Triton kernels | QLoRA, LoRA, GRPO | ✅✅ |
| [Axolotl](https://github.com/axolotl-ai-cloud/axolotl) | YAML-configured fine-tuning for any model; multi-GPU with DeepSpeed/FSDP | LoRA, QLoRA, Full, DPO, ORPO, GRPO | ✅ |
| [LLaMA-Factory](https://github.com/hiyouga/LLaMA-Factory) | User-friendly fine-tuning with Web UI + CLI; 100+ model support | LoRA, QLoRA, Full, SFT, DPO, PPO, ORPO | ✅ |
| [TRL (HuggingFace)](https://github.com/huggingface/trl) | HuggingFace library for RL-based LLM training | SFT, DPO, GRPO, PPO, Reward Modeling | ✅ |
| [PEFT (HuggingFace)](https://github.com/huggingface/peft) | Parameter-Efficient Fine-Tuning methods library | LoRA, QLoRA, Prefix Tuning, Adapters, IA³ | ✅ |
| [OpenRLHF](https://github.com/OpenRLHF/OpenRLHF) | High-performance RLHF framework built on Ray, vLLM, ZeRO-3, and DeepSpeed | RLHF, PPO, DPO, GRPO, SFT | ✅ |
| [Kiln](https://github.com/kiln-ai/kiln) | Fine-tuning tool with synthetic data generation and dataset collaboration | SFT / Synthetic Data | ✅ |
| [augmentoolkit](https://github.com/e-p-armstrong/augmentoolkit) | Tool for training open-source LLMs on new factual datasets | Fact Training | ✅ |
| [torchtune](https://github.com/pytorch/torchtune) | PyTorch's native fine-tuning library; no frills, pure PyTorch | LoRA, QLoRA, Full | ✅ |
| [Megatron-LM](https://github.com/NVIDIA/Megatron-LM) | NVIDIA's framework for training & fine-tuning at massive scale | Full FT, tensor/pipeline parallelism | ✅ (multi-node) |
| [DeepSpeed](https://github.com/microsoft/DeepSpeed) | Microsoft's deep learning optimization library; ZeRO memory optimization | Full FT, ZeRO-1/2/3 | ✅✅ |

### PEFT Methods (Techniques)

| Method | Description | Implementation |
|--------|-------------|----------------|
| LoRA | Low-Rank Adaptation; trains small rank-decomposition matrices | PEFT, Unsloth, Axolotl |
| QLoRA | Quantized LoRA; 4-bit base + LoRA adapters | PEFT + bitsandbytes |
| DoRA | Weight-decomposed LoRA; often outperforms LoRA | Unsloth, PEFT |
| GaLore | Gradient Low-Rank Projection for full-parameter training efficiency | PEFT |
| Adapters | Small bottleneck modules inserted between layers | PEFT, AdapterHub |
| Prefix Tuning | Learned prefix tokens prepended to each Transformer layer | PEFT |

### Data & Alignment Tools

| Tool | Description |
|------|-------------|
| [Alpaca Eval](https://github.com/tatsu-lab/alpaca_eval) | Automated instruction-following model evaluation |
| [Open Instruct](https://github.com/allenai/open-instruct) | AllenAI's framework for instruction tuning with SFT/DPO/RL |
| [DPO Trainer (TRL)](https://huggingface.co/docs/trl/dpo_trainer) | Direct Preference Optimization trainer in TRL |
| [DataTrove](https://github.com/huggingface/datatrove) | Large-scale data processing pipeline for pre-training data |
| [Distilabel](https://github.com/argilla-io/distilabel) | Synthetic data generation and AI feedback pipeline |
| [Argilla](https://github.com/argilla-io/argilla) | Open-source data annotation platform for LLM datasets |

---
 
 ## 10. Model Preparation & Quantization
 
 Tools for merging, quantizing, and optimizing models before deployment.
 
 | Tool | Description | Best For |
 |------|-------------|----------|
 | [mergekit](https://github.com/arcee-ai/mergekit) | Powerful toolkit for merging multiple LLMs (SLERP, TIES, DARE, Passthrough) | Model Merging |
 | [bitsandbytes](https://github.com/TimDettmers/bitsandbytes) | Lightweight wrapper for CUDA custom functions, particularly 8-bit optimizers and 4-bit quantization | Quantization Base |
 | [AutoGPTQ](https://github.com/PanQiQi/AutoGPTQ) | Easy-to-use LLM quantization package based on the GPTQ algorithm | GPTQ Quantization |
 | [AutoAWQ](https://github.com/casper-hansen/AutoAWQ) | Efficient LLM quantization package based on the AWQ algorithm | AWQ Quantization |
 | [GGUF (llama.cpp)](https://github.com/ggerganov/llama.cpp/blob/master/examples/quantize/README.md) | The standard quantization format for CPU/local inference | Local Quantization |
 | [ExLlamaV2](https://github.com/turboderp/exllamav2) | Fast inference for EXL2 quantized models on NVIDIA GPUs | GPU Optimization |
 
 ---
 
 | [outlines](https://github.com/dottxt-ai/outlines) | Structured outputs and generation control for LLMs | ![Stars](https://img.shields.io/github/stars/dottxt-ai/outlines?style=flat-square) | Apache-2.0 |
 
 ---
 
 ## 11. Benchmarks & Leaderboards
 
 | Resource | Description |
 |----------|-------------|
 | [LMSYS Chatbot Arena](https://chat.lmsys.org/?leaderboard) | Crowdsourced open platform for LLM evaluation; ELO-based leaderboard |
 | [Open LLM Leaderboard](https://huggingface.co/spaces/HuggingFaceH4/open_llm_leaderboard) | HuggingFace's tracking of open-source LLMs across multiple benchmarks |
 | [MMLU](https://github.com/hendrycks/test) | Massive Multitask Language Understanding benchmark |
 | [HumanEval](https://github.com/openai/human-eval) | OpenAI's benchmark for evaluating code generation |
 | [SWE-bench](https://github.com/princeton-nlp/SWE-bench) | Evaluation for software engineering agents on real GitHub issues |
 | [LiveCodeBench](https://livecodebench.github.io/leaderboard.html) | Holistic and contamination-free evaluation of LLMs for code |
 
 ---
 
 ## 12. Miscellaneous

Tools that are useful across multiple categories or don't fit neatly into a single section.

| Tool | Description | Stars | License |
|------|-------------|-------|---------|
| [llmfit](https://github.com/AlexsJones/llmfit) | Rust TUI/CLI that scans your hardware and shows which models from 100+ providers will fit and run on it | ![Stars](https://img.shields.io/github/stars/AlexsJones/llmfit?style=flat-square) | MIT |
| [llm-checker](https://github.com/Sunwood-ai-labs/llm-checker) | Python CLI that scans hardware (Apple Silicon, NVIDIA, AMD, Intel Arc), scores compatible models on quality/speed/fit, Ollama integration + built-in MCP server | ![Stars](https://img.shields.io/github/stars/Sunwood-ai-labs/llm-checker?style=flat-square) | MIT |
| [selfhostllm](https://github.com/erans/selfhostllm) | Web calculator estimating GPU memory requirements and max concurrent requests for self-hosted LLM inference | ![Stars](https://img.shields.io/github/stars/erans/selfhostllm?style=flat-square) | MIT |
| [gitingest](https://github.com/coderamp-labs/gitingest) | Converts any GitHub repo into a single prompt-friendly text dump; replace "hub" with "ingest" in any GitHub URL | ![Stars](https://img.shields.io/github/stars/coderamp-labs/gitingest?style=flat-square) | MIT |
| [Repomix](https://github.com/yamadashy/repomix) | Pack your codebase into AI-friendly formats; similar to gitingest but focused on Node ecosystem | ![Stars](https://img.shields.io/github/stars/yamadashy/repomix?style=flat-square) | MIT |
| [Stenography](https://stenography.dev/) | Automatic code documentation using AI to explain complex logic in natural language | ![Stars](https://img.shields.io/github/stars/stenography-ai/stenography?style=flat-square) | Proprietary |
| [Mintlify](https://mintlify.com/) | AI-powered documentation writer that monitors code changes to keep docs in sync | ![Stars](https://img.shields.io/github/stars/mintlify/mintlify?style=flat-square) | Proprietary |
| [Phoenix](https://github.com/Arize-ai/phoenix) | Open-source AI observability platform for tracing, evaluating, and monitoring LLM apps | ![Stars](https://img.shields.io/github/stars/Arize-ai/phoenix?style=flat-square) | Apache-2.0 |
| [OpenLIT](https://github.com/openlit/openlit) | Open-source GenAI and LLM observability platform native to OpenTelemetry | ![Stars](https://img.shields.io/github/stars/openlit/openlit?style=flat-square) | Apache-2.0 |
| [Openllmetry](https://github.com/traceloop/openllmetry) | Open-source observability for LLM applications based on OpenTelemetry | ![Stars](https://img.shields.io/github/stars/traceloop/openllmetry?style=flat-square) | Apache-2.0 |
| [MLflow](https://github.com/mlflow/mlflow) | Open-source platform for the machine learning lifecycle, including LLM tracking | ![Stars](https://img.shields.io/github/stars/mlflow/mlflow?style=flat-square) | Apache-2.0 |
| [Trigger.dev](https://github.com/triggerdotdev/trigger.dev) | Background jobs platform for long-running AI workflows and dependable agents | ![Stars](https://img.shields.io/github/stars/triggerdotdev/trigger.dev?style=flat-square) | Apache-2.0 |
| [context7](https://github.com/upstash/context7) | Up-to-date code documentation for LLMs and AI code editors | ![Stars](https://img.shields.io/github/stars/upstash/context7?style=flat-square) | MIT |
| [deepwiki-open](https://github.com/AsyncFuncAI/deepwiki-open) | AI-powered wiki generator for GitHub/Gitlab/Bitbucket repositories | ![Stars](https://img.shields.io/github/stars/AsyncFuncAI/deepwiki-open?style=flat-square) | MIT |
| [cai](https://github.com/aliasrobotics/cai) | Cybersecurity AI framework (CAI) for AI security testing | ![Stars](https://img.shields.io/github/stars/aliasrobotics/cai?style=flat-square) | MIT |
| [speakr](https://github.com/murtaza-nasir/speakr) | Personal, self-hosted web application for transcribing audio recordings | ![Stars](https://img.shields.io/github/stars/murtaza-nasir/speakr?style=flat-square) | MIT |
| [presenton](https://github.com/presenton/presenton) | Open-source AI presentation generator and API | ![Stars](https://img.shields.io/github/stars/presenton/presenton?style=flat-square) | MIT |
| [Gorilla](https://github.com/ShishirPatil/gorilla) | Large Language Model-Connected APIs; enables LLMs to use 1600+ APIs | ![Stars](https://img.shields.io/github/stars/ShishirPatil/gorilla?style=flat-square) | Apache-2.0 |
| [LlamaHub](https://github.com/emptycrown/llama-hub) | A library of data loaders for LLMs made by the community | ![Stars](https://img.shields.io/github/stars/emptycrown/llama-hub?style=flat-square) | MIT |
| [OmniGen2](https://github.com/VectorSpaceLab/OmniGen2) | Exploration into advanced multimodal generation | ![Stars](https://img.shields.io/github/stars/VectorSpaceLab/OmniGen2?style=flat-square) | MIT |
| [4o-ghibli-at-home](https://github.com/TheAhmadOsman/4o-ghibli-at-home) | Self-hosted AI photo stylizer for performance and privacy | ![Stars](https://img.shields.io/github/stars/TheAhmadOsman/4o-ghibli-at-home?style=flat-square) | MIT |
| [Observer](https://github.com/Roy3838/Observer) | Local micro-agents that observe, log and react to system events | ![Stars](https://img.shields.io/github/stars/Roy3838/Observer?style=flat-square) | MIT |
| [gabber](https://github.com/gabber-dev/gabber) | Tool to build AI apps that see, hear, and speak using screen/mic/cam | ![Stars](https://img.shields.io/github/stars/gabber-dev/gabber?style=flat-square) | MIT |
| [promptcat](https://github.com/sevenreasons/promptcat) | Zero-dependency prompt manager/catalog in a single HTML file | ![Stars](https://img.shields.io/github/stars/sevenreasons/promptcat?style=flat-square) | MIT |
| [heretic](https://github.com/p-e-w/heretic) | Fully automatic censorship removal for language models | ![Stars](https://img.shields.io/github/stars/p-e-w/heretic?style=flat-square) | MIT |
| [llama-swap](https://github.com/mostlygeek/llama-swap) | Reliable model swapping for local OpenAI compatible servers | ![Stars](https://img.shields.io/github/stars/mostlygeek/llama-swap?style=flat-square) | MIT |
| [outlines](https://github.com/dottxt-ai/outlines) | Structured outputs and generation control for LLMs | ![Stars](https://img.shields.io/github/stars/dottxt-ai/outlines?style=flat-square) | Apache-2.0 |


---

## Contributing

Contributions welcome! Please read [CONTRIBUTING.md](CONTRIBUTING.md) before submitting a PR.

**Format for new entries:**
- Use GitHub Stars badges where applicable
- Include a concise, accurate description
- Link to the primary GitHub repo or official site

---

## License

[![CC0](https://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg)](https://creativecommons.org/publicdomain/zero/1.0)

This list is released into the public domain under CC0.
