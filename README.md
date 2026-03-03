# awesome-llm-tools

> A curated directory of essential LLM tools spanning the full stack: from model preparation and quantization to inference engines, local agents, agent frameworks, RAG pipelines, vector databases, fine-tuning, and more.

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

---

## Table of Contents

1. [Pre-Prep & Model Optimization](#1-pre-prep--model-optimization)
2. [Inference Engines](#2-inference-engines)
   - [Desktop / Local](#desktop--local)
   - [Server / Production](#server--production)
3. [Local Agents](#3-local-agents)
   - [Coding Agents & IDE Extensions](#coding-agents--ide-extensions)
   - [Autonomous Agents](#autonomous-agents)
   - [Audio / Voice Agents](#audio--voice-agents)
   - [General-Purpose Local Agents](#general-purpose-local-agents)
4. [Libraries & Frameworks](#4-libraries--frameworks)
   - [Python](#python)
   - [JavaScript / TypeScript](#javascript--typescript)
   - [Java](#java)
   - [Kotlin](#kotlin)
   - [Go](#go)
   - [Rust](#rust)
5. [Prompt Optimization](#5-prompt-optimization)
6. [Context Optimization](#6-context-optimization)
7. [Agent Memory](#7-agent-memory)
8. [RAG Pipelines](#8-rag-pipelines)
9. [Vector Databases](#9-vector-databases)
10. [Fine-Tuning](#10-fine-tuning)
11. [Miscellaneous](#11-miscellaneous)

---

## 1. Pre-Prep & Model Optimization

Tools for quantization, compression, and preparing models for efficient inference.

| Tool | Description | Stars | License |
|------|-------------|-------|---------|
| [AutoGPTQ](https://github.com/AutoGPTQ/AutoGPTQ) | GPTQ Post-Training Quantization for LLMs; 2–4 bit weight quantization | ![Stars](https://img.shields.io/github/stars/AutoGPTQ/AutoGPTQ?style=flat-square) | MIT |
| [AutoAWQ](https://github.com/casper-hansen/AutoAWQ) | Activation-aware Weight Quantization (AWQ) for 4-bit models | ![Stars](https://img.shields.io/github/stars/casper-hansen/AutoAWQ?style=flat-square) | MIT |
| [bitsandbytes](https://github.com/bitsandbytes-foundation/bitsandbytes) | 8-bit & 4-bit quantization for PyTorch; enables QLoRA training | ![Stars](https://img.shields.io/github/stars/bitsandbytes-foundation/bitsandbytes?style=flat-square) | MIT |
| [llm-compressor](https://github.com/vllm-project/llm-compressor) | Hugging Face–native compression toolkit from the vLLM team (SmoothQuant, AWQ, GPTQ) | ![Stars](https://img.shields.io/github/stars/vllm-project/llm-compressor?style=flat-square) | Apache-2.0 |
| [SmoothQuant](https://github.com/mit-han-lab/smoothquant) | W8A8 quantization by migrating outliers from activations to weights | ![Stars](https://img.shields.io/github/stars/mit-han-lab/smoothquant?style=flat-square) | MIT |
| [optimum](https://github.com/huggingface/optimum) | Hugging Face toolkit for hardware-accelerated model export and quantization (ONNX, OpenVINO) | ![Stars](https://img.shields.io/github/stars/huggingface/optimum?style=flat-square) | Apache-2.0 |
| [llmcompressor](https://github.com/neuralmagic/compressed-tensors) | Neural Magic's compressed-tensors format & quantization tools | ![Stars](https://img.shields.io/github/stars/neuralmagic/compressed-tensors?style=flat-square) | Apache-2.0 |
| [quanto](https://github.com/huggingface/quanto) | PyTorch quantization toolkit supporting W4/W8/A8 and QAT | ![Stars](https://img.shields.io/github/stars/huggingface/quanto?style=flat-square) | Apache-2.0 |
| [intel/neural-compressor](https://github.com/intel/neural-compressor) | Intel's model compression tool with sparsity, quantization, and pruning | ![Stars](https://img.shields.io/github/stars/intel/neural-compressor?style=flat-square) | Apache-2.0 |
| [gguf-tools](https://github.com/antirez/gguf-tools) | CLI utilities for inspecting and editing GGUF model files | ![Stars](https://img.shields.io/github/stars/antirez/gguf-tools?style=flat-square) | BSD-2 |
| [Wanda](https://github.com/locuslab/wanda) | Pruning LLMs by weights and activation norms; removes weights per-output with no retraining | ![Stars](https://img.shields.io/github/stars/locuslab/wanda?style=flat-square) | MIT |

---

## 2. Inference Engines

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

### Server / Production

Designed for high-throughput, multi-user, and production API serving.

| Tool | Description | Key Feature | GPU Support |
|------|-------------|-------------|-------------|
| [vLLM](https://github.com/vllm-project/vllm) | State-of-the-art serving engine with PagedAttention & continuous batching | Highest throughput | NVIDIA, AMD, TPU |
| [TGI (Text Generation Inference)](https://github.com/huggingface/text-generation-inference) | Hugging Face's production-grade Rust/Python server | Flash Attention, tensor parallelism | NVIDIA, AMD, Gaudi |
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

---

## 3. Local Agents

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
| [Plandex](https://github.com/plandex-ai/plandex) | CLI Agent | Terminal | ✅ OpenAI-compat | Long-running terminal agent for complex tasks |
| [SWE-agent](https://github.com/princeton-nlp/SWE-agent) | CLI Agent | Terminal | ✅ Via API | Autonomous GitHub issue solver |
| [OpenHands (OpenDevin)](https://github.com/All-Hands-AI/OpenHands) | Web + CLI | Browser / Terminal | ✅ OpenAI-compat | Full autonomous software engineering agent |
| [Claude Code](https://www.anthropic.com/claude-code) | CLI Agent | Terminal | ❌ Cloud (Claude) | Anthropic's terminal agent; code onboarding, PR generation, powerful edits |
| [Jules](https://jules.google/) | Async Agent | GitHub | ❌ Cloud (Gemini) | Google's async coding agent; works in the background on GitHub issues |
| [Browser-Use](https://github.com/browser-use/browser-use) | Browser Agent | Browser | ✅ OpenAI-compat | Enable AI to control your browser; web automation agent |
| [Neovim + llm.nvim](https://github.com/huggingface/llm.nvim) | Plugin | Neovim | ✅ Native | HuggingFace's Neovim LLM plugin |

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

### Autonomous Agents

Full autonomous agents that can plan, act, use tools, and run 24/7 without constant human supervision.

| Tool | Description | Language | Notes |
|------|-------------|----------|-------|
| [OpenClaw](https://github.com/openclaw-ai/openclaw) | Self-hosted autonomous agent; multi-channel gateway, self-installing tools, persistent memory | TypeScript | 100k+ GitHub stars |
| [TinyClaw](https://github.com/tinyclaw-ai/tinyclaw) | Lightweight personal AI companion; multi-agent team (coder, writer, researcher) with live dashboard & file-based task queue | Python | Personal, multi-channel |
| [OpenFang](https://www.openfang.sh/) | Agent OS: 7 autonomous capability packages, 16 security layers, 40 channel adapters, 30 pre-built agents, MCP & A2A | Rust | Self-hosted |
| [NullClaw](https://github.com/nullclaw/nullclaw) | Fastest, smallest autonomous AI assistant infra; hybrid host + WASM, edge-optimised | Zig | Self-hosted |
| [ZeroClaw](https://github.com/zeroclaw-labs/zeroclaw) | Fast, small autonomous AI assistant infra; deploy anywhere, hot-swap any component | Rust | Self-hosted |

### General-Purpose Local Agents

| Tool | Description | Notes |
|------|-------------|-------|
| [Open WebUI](https://github.com/open-webui/open-webui) | Feature-rich self-hosted web UI for Ollama / OpenAI APIs | Tools, RAG, image gen built-in |
| [AnythingLLM](https://github.com/Mintplex-Labs/anything-llm) | All-in-one local AI app with agents, RAG, tools | Desktop + Docker |
| [LibreChat](https://github.com/danny-avila/LibreChat) | Multi-provider AI chat with agents, plugins, RAG | Self-hosted |
| [SillyTavern](https://github.com/SillyTavern/SillyTavern) | Advanced frontend for character-based AI interactions | Self-hosted |
| [PrivateGPT](https://github.com/zylon-ai/private-gpt) | Production-ready private document Q&A agent | 100% local |
| [Dash (Agno)](https://github.com/agno-agi/dash) | Self-learning data / text-to-SQL agent grounded in 6 layers of context; inspired by OpenAI's internal impl | Built on Agno framework |
| [visual-explainer](https://github.com/nicobailon/visual-explainer) | Agent skill that generates rich HTML pages and slide decks for diagrams, diff reviews, plan audits, and project recaps | Agent skill / tool |

---

## 4. Libraries & Frameworks

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
| [Semantic Kernel](https://github.com/microsoft/semantic-kernel) | Microsoft's SDK for integrating LLMs into .NET/Python/Java apps | Enterprise, .NET ecosystem |
| [Atomic Agents](https://github.com/BrainBlend-AI/atomic-agents) | Modular, dependency-injection-based agent framework | Composable, testable agents |
| [Camel](https://github.com/camel-ai/camel) | Communicative Agents framework; role-play multi-agent | Research, agent communication patterns |
| [OpenAI Agents SDK](https://github.com/openai/openai-agents-python) | Official OpenAI Python SDK for building agents | OpenAI-native agent workflows |
| [Google ADK](https://google.github.io/adk-docs/) | Google's Agent Development Kit — modular, model-agnostic framework with multi-agent orchestration, rich tool ecosystem, built-in eval | Google Cloud / Gemini agents |
| [aisuite](https://github.com/andrewyng/aisuite) | Simple unified interface to multiple Generative AI providers, by Andrew Ng | Multi-provider prototyping |
| [swarm](https://github.com/openai/swarm) | OpenAI's educational framework for lightweight ergonomic multi-agent orchestration | Learning multi-agent patterns |
| [guidance](https://github.com/guidance-ai/guidance) | Interleave generation, prompting, and logic control in a continuous flow matching LLM processing | Constrained, structured generation |
| [outlines](https://github.com/outlines-dev/outlines) | Library for reliable structured generation (JSON, regex, grammar) from LLMs and diffusers, by dottxt.ai | Structured outputs |
| [Multi-Agent Orchestrator](https://github.com/awslabs/multi-agent-orchestrator) | AWS framework for managing multiple AI agents and complex multi-turn conversations | Enterprise multi-agent systems |
| [rowboat](https://github.com/rowboatlabs/rowboat) | AI-powered multi-agent builder with no-code UI, powered by OpenAI Agents SDK | Rapid agent prototyping |
| [Medusa](https://github.com/FasterDecoding/Medusa) | Framework accelerating LLM generation with multiple decoding heads; no specialized hardware | Inference acceleration |
| **Core Libraries** |
| [transformers](https://github.com/huggingface/transformers) | HuggingFace's flagship model library; 300k+ models, inference & fine-tuning for every major architecture | Foundation library |
| [accelerate](https://github.com/huggingface/accelerate) | HuggingFace library to run PyTorch training/inference on any hardware with minimal code changes | Multi-GPU / mixed-precision |
| [sentence-transformers](https://github.com/UKPLab/sentence-transformers) | Easy-to-use library for state-of-the-art sentence, text, and image embeddings | Embeddings / semantic search |
| [tiktoken](https://github.com/openai/tiktoken) | OpenAI's fast BPE tokenizer; used to count tokens before sending to APIs | Tokenization |
| [openai](https://github.com/openai/openai-python) | Official OpenAI Python SDK | OpenAI API client |
| [anthropic](https://github.com/anthropics/anthropic-sdk-python) | Official Anthropic Python SDK | Claude API client |
| [google-genai](https://github.com/googleapis/python-genai) | Official Google Gen AI Python SDK for Gemini models | Gemini API client |
| [google-adk](https://pypi.org/project/google-adk/) | Google Agent Development Kit Python package | Google ADK agents |

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
| [ai](https://www.npmjs.com/package/ai) | Vercel AI SDK — stream-first unified API for LLMs, RSC support, tool calling | Universal LLM SDK for JS/TS |
| [genkit](https://www.npmjs.com/package/genkit) | Google's GenKit — production AI flows, plugins, tracing, evaluation | Google Cloud / Firebase AI apps |
| [openai](https://github.com/openai/openai-node) | Official OpenAI Node.js / TypeScript SDK | OpenAI API client |
| [anthropic](https://github.com/anthropics/anthropic-sdk-typescript) | Official Anthropic TypeScript SDK | Claude API client |
| [ollama-js](https://github.com/ollama/ollama-js) | Official Ollama JavaScript library | Local model client |
| [@google/genai](https://github.com/googleapis/js-genai) | Official Google Gen AI JS/TS SDK for Gemini models | Gemini API client |
| [@google/adk](https://www.npmjs.com/package/@google/adk) | Google Agent Development Kit for Node.js | Google ADK agents |

### Java

| Framework | Description | Best For |
|-----------|-------------|----------|
| [Semantic Kernel](https://github.com/microsoft/semantic-kernel) | Microsoft's cross-language AI SDK | Enterprise, .NET / Java ecosystem |
| [Spring AI](https://github.com/spring-projects/spring-ai) | Spring Framework for AI / LLM integration; prompt chaining, routing, RAG | Spring Boot apps |
| [LangChain4j](https://github.com/langchain4j/langchain4j) | Java port of LangChain; chains, tools, agents, RAG | Java LLM apps |
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

---

## 5. Prompt Optimization

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

---

## 6. Context Optimization

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

---

## 7. Agent Memory

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

---

## 8. RAG Pipelines

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

---

## 9. Vector Databases

Purpose-built stores for high-dimensional vector embeddings.

| Database | Type | Best For | License |
|----------|------|----------|---------|
| [Chroma](https://github.com/chroma-core/chroma) | Open-source, Python-native | Local dev, prototyping, RAG | Apache-2.0 |
| [Qdrant](https://github.com/qdrant/qdrant) | Open-source, Rust-built, cloud option | Production, fast filtering, hybrid search | Apache-2.0 |
| [Milvus](https://github.com/milvus-io/milvus) | Open-source, Kubernetes-scale | Billion-vector scale, enterprise | Apache-2.0 |
| [Weaviate](https://github.com/weaviate/weaviate) | Open-source, GraphQL API | Semantic + GraphQL queries, hybrid search | BSD-3 |
| [pgvector](https://github.com/pgvector/pgvector) | PostgreSQL extension | Existing PostgreSQL users, <1M vectors | PostgreSQL |
| [LanceDB](https://github.com/lancedb/lancedb) | Embedded, serverless, columnar | Serverless RAG, edge apps | Apache-2.0 |
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

## 10. Fine-Tuning

Frameworks and tools for fine-tuning, alignment, and PEFT methods.

### Training Frameworks

| Tool | Description | Methods | Memory Efficient |
|------|-------------|---------|-----------------|
| [Unsloth](https://github.com/unslothai/unsloth) | 2–5× faster fine-tuning; 70–90% less VRAM via custom CUDA/Triton kernels | QLoRA, LoRA, GRPO | ✅✅ |
| [Axolotl](https://github.com/axolotl-ai-cloud/axolotl) | YAML-configured fine-tuning for any model; multi-GPU with DeepSpeed/FSDP | LoRA, QLoRA, Full, DPO, ORPO, GRPO | ✅ |
| [LLaMA-Factory](https://github.com/hiyouga/LLaMA-Factory) | User-friendly fine-tuning with Web UI + CLI; 100+ model support | LoRA, QLoRA, Full, SFT, DPO, PPO, ORPO | ✅ |
| [TRL (HuggingFace)](https://github.com/huggingface/trl) | HuggingFace library for RL-based LLM training | SFT, DPO, GRPO, PPO, Reward Modeling | ✅ |
| [PEFT (HuggingFace)](https://github.com/huggingface/peft) | Parameter-Efficient Fine-Tuning methods library | LoRA, QLoRA, Prefix Tuning, Adapters, IA³ | ✅ |
| [torchtune](https://github.com/pytorch/torchtune) | PyTorch's native fine-tuning library; no frills, pure PyTorch | LoRA, QLoRA, Full | ✅ |
| [OpenRLHF](https://github.com/OpenRLHF/OpenRLHF) | High-performance RLHF training framework (Ray + DeepSpeed) | PPO, DPO, GRPO, SFT | ✅ |
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

## 11. Miscellaneous

Tools that are useful across multiple categories or don't fit neatly into a single section.

| Tool | Description | Stars | License |
|------|-------------|-------|---------|
| [llmfit](https://github.com/AlexsJones/llmfit) | Rust TUI/CLI that scans your hardware and shows which models from 100+ providers will fit and run on it | ![Stars](https://img.shields.io/github/stars/AlexsJones/llmfit?style=flat-square) | MIT |
| [llm-checker](https://github.com/Sunwood-ai-labs/llm-checker) | Python CLI that scans hardware (Apple Silicon, NVIDIA, AMD, Intel Arc), scores compatible models on quality/speed/fit, Ollama integration + built-in MCP server | ![Stars](https://img.shields.io/github/stars/Sunwood-ai-labs/llm-checker?style=flat-square) | MIT |
| [selfhostllm](https://github.com/erans/selfhostllm) | Web calculator estimating GPU memory requirements and max concurrent requests for self-hosted LLM inference | ![Stars](https://img.shields.io/github/stars/erans/selfhostllm?style=flat-square) | MIT |

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
