# Learnings from my projects

This document lists the repositories in my GitHub account and a short summary of what I did and what I learned from each project.

---

## aegis-911 — https://github.com/nihalpj/aegis-911
What I did:
- Built an AI-augmented emergency dispatch monorepo (server + web + infra + shared packages).
- Implemented operator console (React + Vite + Tailwind) and backend services (Node + Fastify + TypeScript).
- Wrote Docker Compose infra (Postgres, Redis, MinIO), Prisma migrations and Playwright e2e smoke tests.

What I learned:
- Designing a monorepo layout and cross-workspace development workflows.
- Running real-time systems: WebSockets, streaming STT (AssemblyAI), Twilio integrations and media handling.
- Local infra orchestration with Docker Compose and pragmatic testing with Playwright.

---

## AI-Launcher — https://github.com/nihalpj/AI-Launcher
What I did:
- Forked and extended an Android launcher (Kotlin) to be AI-first with conversational UI, semantic search and proactive suggestions.
- Integrated local LLM inference strategies (llama.cpp / small models) for on-device features.

What I learned:
- Android launcher architecture and lifecycle, Kotlin Android development and UI/UX for home screens.
- Practical constraints of running local LLMs on mobile and trade-offs (model size, latency, caching).
- Building semantic search and proactive suggestion UX inside a constrained launcher environment.

---

## AI-Product-Manager — https://github.com/nihalpj/AI-Product-Manager
What I did:
- Developed prototypes and documentation for AI-enabled product management tooling and workflows.
- Experimented with tooling to support product discovery, roadmapping and metrics.

What I learned:
- How to translate product requirements into technical scaffolding for AI-first product features.
- Prototyping patterns for combining human workflows with automated suggestion systems.

---

## AIAgentAntivirus — https://github.com/nihalpj/AIAgentAntivirus
What I did:
- Built a CLI security scanner for AI agent files that detects prompt-injection, suspicious code, and other AI-related vulnerabilities.
- Implemented scanning options, platform targeting, output formats (console/json/html/sarif) and exclude patterns.

What I learned:
- Static analysis patterns for agent artifacts and prompt-injection heuristics.
- Building a robust CLI (TypeScript) with options, parallel workers, and standardized output (SARIF).
- Packaging and distribution best practices for developer tools.

---

## Docskills (DocSLM) — https://github.com/nihalpj/Docskills
What I did:
- Built DocSLM: a domain-specialized small language model pipeline (Qwen3.5-0.8B fine-tune) for document-skills agents.
- Implemented the data engine, SFT and DPO training pipelines, verification stack, and deployment steps (llama.cpp / GGUF quantization).

What I learned:
- End-to-end model fine-tuning workflows (data engineering → SFT → DPO → quantization) and training on consumer GPUs (RTX 4090).
- Designing verifiable agent stacks for document processing with testable tooling and post-check verifiers.
- Packaging and shipping GGUF/llama.cpp artifacts for edge deployment.

---

## FlashRAG — https://github.com/nihalpj/FlashRAG
What I did:
- Forked/explored a comprehensive RAG toolkit to reproduce RAG baselines, run experiments, and test retrieval + generator components.
- Ran quick-start examples and experimented with retrievers, Faiss indexes and vLLM-backed generation.

What I learned:
- Practical RAG architecture: retriever-reranker-generator pipelines, corpus preprocessing and index building.
- How to evaluate and reproduce RAG experiments, and trade-offs between retrieval and model reasoning.
- Tooling around Faiss, sentence-transformers, and deployment considerations for RAG systems.

---

## leo / Leoo — https://github.com/nihalpj/Leoo
What I did:
- Built LEO: a Flask web app for the Lincoln Entomology Observers to record sightings, manage members, and generate reports.
- Implemented raw SQL queries, Bootstrap templates, search (ILIKE), flash messages and a small reporting dashboard.

What I learned:
- Building simple, pragmatic Flask apps with raw SQL for transparency and performance in complex queries.
- UX considerations for field-data entry, date formatting localization and avoiding duplicate records.
- When to use ORMs vs. raw SQL and how to design constrained forms and validations.

---

## Profile (nihalpj) — https://github.com/nihalpj/nihalpj
What I did:
- Maintained my personal profile README and bundled links to projects, contact info and tech skills.

What I learned:
- How to present project highlights and technical skills clearly on GitHub profiles.
- Keeping documentation concise and linking to deeper PRDs, docs and demos.

---

## Raaabit_Chatbot — https://github.com/nihalpj/Raaabit_Chatbot
What I did:
- Built a comprehensive RAG-enabled chatbot platform with FastAPI backends, a React frontend, and embedding/RAG service.
- Integrated Ollama for local LLM inference, PostgreSQL + pgvector for embeddings, and MinIO for document storage.
- Created management scripts for Docker/native deployments and documented dev workflows.

What I learned:
- Designing scalable RAG services with embedding storage (pgvector), document chunking and search UX.
- Integrating local LLM engines (Ollama) with real-time WebSocket streaming and JWT auth.
- Deployment patterns for mixed Docker/native stacks and debugging common operational issues.

---

## Test — https://github.com/nihalpj/Test
What I did:
- Used as a sandbox for quick experiments and small code snippets.

What I learned:
- Rapid prototyping workflows and lightweight repo hygiene for throwaway experiments.

---

## Why5AgenticModel — https://github.com/nihalpj/Why5AgenticModel
What I did:
- Implemented distillation scripts and a multi-stage distillation plan (teacher → student → on-policy → DPO) for Why5 model family.
- Created data generation, SFT training, on-policy rollouts and DPO pipelines with mock/real runs and guardrails.

What I learned:
- Distillation and curriculum design for instruction-following LLMs, including masked losses and guarded teacher behavior.
- On-policy correction workflows, DPO preference training and how to orchestrate a multi-stage distillation pipeline.
- Reproducible runbooks and how to mock-run the pipeline without GPUs for development.

---

If you'd like, I can:
- Add more detailed bullets per repo (commands, key files, or examples of code you wrote).
- Create/commit this file to another repository or a specific branch.
- Generate a short README-style web page using this content for your personal site.
