---
title: "04 — Hallucinations, Tools, and Context"
draft: false
---

# 04 — Hallucinations, Tools, and Context

Hallucinations are not rare bugs. They are a predictable side effect of how LLMs generate text.

## Why hallucinations happen

LLMs are optimized to produce likely next tokens, not to verify truth.

So when information is uncertain, the model may still produce fluent answers.

## Safer classroom mental model

- Treat outputs as **drafts**, not facts.
- Separate **fluency** from **reliability**.
- Require verification for factual claims.

## Mitigation strategies

1. Ask for uncertainty explicitly:
   - “If you are not sure, say so.”
2. Request source-grounded output:
   - “Answer only from the provided text.”
3. Use retrieval/tool support when possible:
   - web search
   - trusted documents in prompt context

## Parameters vs context window

Useful distinction:

- **Model parameters** = compressed statistical memory from training
- **Context window** = immediate working memory for the current task

Practical rule:

- If precision matters, place the relevant material in context.

## Embeddings primer (for retrieval)

Embeddings convert text into vectors so we can compare meaning using distance/similarity.

In practice:

- similar text chunks are closer in vector space
- we can retrieve the most relevant chunks for a user query
- retrieved context can then be fed back to the model before answering

Why this matters here:

- retrieval adds grounded context
- grounded context helps reduce hallucination risk on factual tasks

## Notebook link (practice)

Hands-on companion:

- [02 – Simple RAG + Personas + Chat Memory ](../samples/02-simple-rag-personas.ipynb)
- [03 – Embeddings + Tiny Semantic Search ](../samples/03-embeddings-semantic-search.ipynb)

Optional tooling extension:

- [04 – Hugging Face Model Loading Quickstart](../samples/04-huggingface-model-loading-quickstart.ipynb)

## Verification routine (minimal)

Before accepting an answer:

1. Check whether claims are factual or speculative
2. Verify key claims with external sources
3. Revise final output with citations or evidence
