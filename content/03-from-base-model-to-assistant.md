---
title: "03 — From Base Model to Assistant"
draft: false
---

# 03 — From Base Model to Assistant

After pre-training, models are powerful but not yet reliable assistants.

## Why post-training is needed

A base model mainly predicts likely continuations. That means:

- it may not follow instructions consistently
- it may over-complete or change style unexpectedly
- it may produce plausible but unhelpful output

Post-training aligns behavior with how we want an assistant to respond.

## Supervised Fine-Tuning (SFT)

In SFT, the model is trained on conversation-style examples:

- user asks a question
- assistant gives a target response
- training repeats across many tasks and tones

The goal is to make the model imitate high-quality assistant behavior.

## Conversation format matters

Models are trained with structured role patterns (user/assistant/system styles).

Key idea:

- it is still one token sequence
- role formatting helps the model separate “question” from “answer” behavior

## Human + synthetic data pipelines

Modern post-training usually mixes:

- human-authored examples
- model-generated examples reviewed/filtered by humans

This enables scale while keeping quality control.

## Big-picture takeaway

When students chat with an assistant model, they are interacting with:

1. pre-trained language patterns
2. plus behavior shaping from instruction datasets

So assistant behavior is trained behavior — not pure emergent “truth reasoning.”

## Notebook link (practice)

Hands-on companion:

- [01 – System Prompt Playground ](../samples/01-system-prompt.ipynb)

What to focus on in that notebook:

- baseline vs system prompt behavior
- persona switching with a simple list
- prompt contract for consistent classroom outputs

## Bridge to studio practice

In practical notebooks, this post-training background appears as:

- better instruction following than raw base-style behavior
- sensitivity to system prompt and role formatting
- need for iterative prompting plus external verification for reliability
