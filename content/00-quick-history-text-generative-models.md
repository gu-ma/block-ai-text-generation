---
title: "00 — Quick History of Text Generative Models"
draft: false
---

# 00 — Quick History of Text Generative Models

This short timeline gives context for how we moved from simple probabilistic text models to modern LLMs.

## 1) Statistical language models (1990s–2000s)

- **n-gram models** estimated the next word from a short local context (for example, previous 2–4 words).
- They were simple and fast, but had weak long-range coherence and sparse-data limits.

## 2) Early neural language models

- Word embeddings + neural networks improved generalization compared with pure count-based methods.
- Models could capture smoother semantic relationships between words.

## 3) RNN era (2010s)

- **RNNs** modeled sequences token by token with a recurrent hidden state.
- They improved sequence modeling over n-grams, but struggled with long dependencies.

## 4) LSTM/GRU improvements

- **LSTM** and **GRU** architectures introduced gating mechanisms.
- These reduced vanishing-gradient issues and improved memory over longer spans.

## 5) Seq2Seq + Attention

- Encoder-decoder setups became strong for translation and structured generation tasks.
- **Attention** improved focus on relevant source tokens and became a key bridge to transformers.

## 6) Transformer era (2017 → today)

- Transformers replaced recurrence with **self-attention**.
- This enabled better long-range modeling, high parallelism in training, and large-scale model growth.
- Modern foundation models and assistant-style LLMs build on this paradigm.

## Practical takeaway for students

Each step improved one major bottleneck: context length, training efficiency, or controllability. Current LLMs are powerful, but still probabilistic generators that require verification and critical use.
