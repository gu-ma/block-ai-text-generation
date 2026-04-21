---
title: "02 — Pretraining & Base Models"
draft: false
---

# 02 — Pretraining & Base Models

Pre-training is where an LLM learns general language patterns at scale.

## Step 1: Build the training corpus

Typical pipeline:

- crawl large public web sources
- filter low-quality or risky content
- extract clean text from raw HTML
- remove duplicates
- remove sensitive information where possible

Result: a large text dataset (often measured in trillions of tokens).

## Step 2: Tokenization

Before training, text is split into **tokens**.

- models do not process words as humans do
- models process token IDs in a sequence
- tokenization balances vocabulary size and sequence length

Important classroom point:

- LLM mistakes sometimes come from token-level representation limits.

## Step 3: Next-token training

Core objective:

- given previous tokens, predict the next token probability distribution
- compare prediction with the real next token
- adjust parameters
- repeat many, many times

This process produces a **base model**.

## What a base model is

A base model is:

- a strong text continuation engine
- a statistical memory of internet-scale text
- not yet optimized for helpful assistant behavior

## Practical implication

Base models can be impressive, but they may:

- drift off-format
- sound confident when wrong
- continue text in unwanted directions

That is exactly why post-training exists.

## Bridge to studio practice

In studio notebooks, we usually work with already-trained models:

- we do not retrain parameters
- we control behavior through prompts and context
- we use retrieval/context injection when factual grounding matters


## Activity

<iframe
  src="https://ai.massol.me/h5p/embed.html?activity=block-ai-text-generation/02-pretraining-base-models"
  style="width:100%; height:clamp(560px, 30vh, 900px); border:0; display:block;"
  title="Activity"
  loading="lazy"
></iframe>
