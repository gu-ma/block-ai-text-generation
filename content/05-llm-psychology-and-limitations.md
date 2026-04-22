---
title: "05 — LLM Psychology and Limitations"
draft: false
---

# 05 — LLM Psychology and Limitations

“LLM psychology” is a useful shorthand for recurring behavior patterns.

## Token-level cognition

LLMs reason through token generation. This creates constraints:

- they need intermediate tokens to unfold complex reasoning
- rushed outputs often reduce quality
- wording of the prompt can strongly affect behavior

## Typical failure patterns

1. **Overconfident errors**
   - fluent but incorrect answers
2. **Counting/character mistakes**
   - tokenization makes some character-level tasks harder
3. **Format drift**
   - output may ignore requested structure
4. **Identity confusion**
   - model self-descriptions can be inconsistent without clear context

## Why this matters in class

Students should learn to treat LLM outputs as:

- useful collaborators
- not authoritative sources
- systems with uneven reliability across task types

## Better prompting for reliability

- ask for stepwise reasoning when needed
- define output format explicitly
- ask for confidence and uncertainty boundaries
- include reference material in prompt context

## Big takeaway

LLMs are powerful but jagged tools.

Success comes from combining:

- good prompt design
- task-aware verification
- human judgment

## Activity

<iframe
  src="https://ai.massol.me/h5p/embed.html?activity=block-ai-text-generation/05-llm-psychology-and-limitations"
  style="width:100%; height:500px; border:0; display:block;"
  title="Activity"
  loading="lazy"
></iframe>
