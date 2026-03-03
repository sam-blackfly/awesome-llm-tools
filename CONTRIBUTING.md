# Contributing to awesome-llm-tools

Thank you for helping keep this list accurate and up-to-date! Please read the guidelines below before submitting a pull request.

---

## What belongs here

This list covers **tools, frameworks, and infrastructure** for working with LLMs — not models, papers, or datasets. A good entry is:

- Actively maintained (last commit within ~12 months)
- Open-source **or** a well-known commercial product with clear value
- Relevant to developers building with or deploying LLMs

---

## Adding an entry

### 1. Find the right section

| Section | Belongs here |
|---------|-------------|
| **Pre-Prep & Model Optimization** | Quantization, pruning, compression tools |
| **Inference Engines → Desktop/Local** | Local runtimes, desktop apps, single-machine inference |
| **Inference Engines → Server/Production** | High-throughput serving, API proxies, production stacks |
| **Local Agents → Coding Agents** | AI coding assistants, IDE extensions, CLI coding agents |
| **Local Agents → Autonomous Agents** | Self-hosted 24/7 autonomous agents |
| **Local Agents → Audio/Voice** | STT, TTS, voice pipeline tools |
| **Local Agents → General-Purpose** | Chat UIs, all-in-one local AI apps |
| **Agent Frameworks** | SDKs/libraries for building agents or LLM pipelines |
| **Prompt Optimization** | Prompt engineering, evaluation, observability |
| **Context Optimization** | Context compression, chunking, attention tricks |
| **Agent Memory** | Persistent/long-term memory systems for agents |
| **RAG Pipelines** | Retrieval-augmented generation frameworks |
| **Vector Databases** | Embedding stores |
| **Fine-Tuning** | Training frameworks, PEFT methods, alignment tools |
| **Miscellaneous** | Cross-cutting utilities that don't fit above |

### 2. Row format

Each entry must follow the table format of its section exactly. For most sections:

```markdown
| [Tool Name](https://github.com/org/repo) | Short description — what it does and why it stands out | ![Stars](https://img.shields.io/github/stars/org/repo?style=flat-square) | License |
```

- **Description**: one concise sentence; lead with the tool's primary function
- **Stars badge**: use the `flat-square` style; omit for non-GitHub tools
- **License**: use the SPDX identifier (e.g. `MIT`, `Apache-2.0`, `BSD-3`)

### 3. Placement

- Insert alphabetically **or** by relevance/popularity within a section — whichever reads better
- Do not add duplicate entries (check all sections before submitting)

---

## Updating an existing entry

- Correct factual errors (wrong URL, outdated description, wrong section)
- Update the license if it has changed
- Flag archived/unmaintained projects with a note or open an issue to discuss removal

---

## Removing an entry

Open an issue first to discuss removal. Good reasons to remove:

- Project archived or abandoned with no maintained fork
- Repo deleted or privatised
- Fundamentally broken / known security issues with no fix

---

## Pull request checklist

- [ ] Entry is in the correct section
- [ ] Description is accurate and concise (≤ 15 words preferred)
- [ ] Link goes to the primary GitHub repo or official site
- [ ] Stars badge uses `flat-square` style (for GitHub repos)
- [ ] License is correct
- [ ] No duplicate of an existing entry
- [ ] Markdown renders correctly (check with a local preview)

---

## Code of conduct

Be respectful and constructive. Submissions that are purely promotional or lack genuine utility for LLM developers will be declined.
