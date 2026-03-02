---
title: "07 — Inference & RAG in Practice (Bridge Note)"
draft: false
---

# 07 — Inference & RAG in Practice (Bridge Note)

This note connects model-building concepts to what we actually do in studio notebooks.

## What changes between training and class practice

- **Training time:** model parameters are learned from massive datasets.
- **Inference time (our studio):** parameters are fixed; we shape outputs with prompts and context.

## Core levers we control in notebooks

1. **Prompt design**
   - clear goal, role, constraints, and output format
2. **System instructions**
   - stable behavior contract across turns
3. **Context injection**
   - provide relevant source text directly in the prompt
4. **Retrieval (RAG)**
   - fetch relevant chunks via embeddings and attach them before generation

## Why retrieval helps

LLMs are fluent but not guaranteed factual. Retrieval helps by grounding answers in selected source material for the current query.

## Minimal studio loop

1. Draft prompt
2. Generate
3. Evaluate (quality + factual risk)
4. Add/revise context (or retrieval)
5. Verify key claims
6. Finalize

## Notebook map

- [01 – System Prompt Playground](../samples/01-system-prompt.ipynb)
- [02 – Simple RAG + Personas + Chat Memory](../samples/02-simple-rag-personas.ipynb)
- [03 – Embeddings + Tiny Semantic Search](../samples/03-embeddings-semantic-search.ipynb)
- [04 – Hugging Face Model Loading Quickstart](../samples/04-huggingface-model-loading-quickstart.ipynb)
