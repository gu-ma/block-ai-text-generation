
# Block: AI – Text Generation

This block introduces how large language models (LLMs) work at a big-picture level. Students build practical mental models of the full pipeline (pre-training, post-training, reinforcement learning), understand what LLMs can and cannot do, and apply a critical workflow for creative and academic use.

## Learning Objectives

By the end of this block, you will be able to:

- Explain the three-stage LLM pipeline in simple terms (pre-training, post-training, reinforcement learning)
- Distinguish base models from assistant models and describe why behavior changes after post-training
- Identify common LLM failure modes (hallucinations, overconfidence, token-level limitations)
- Use a practical verification workflow when integrating LLMs into creative or research tasks

## Bridge: From Training to Studio Inference

This block has two complementary views:

- **How models are built** (history, pre-training, post-training)
- **How models are used** (prompting, inference, retrieval, verification)

In studio, we do not train LLMs from scratch. We work at **inference time**:

- shape behavior with prompts and system instructions
- improve factual reliability with retrieval/context
- evaluate and verify outputs before final use

## Session Timeline Overview

- **Part 1 (Lecture + Discussion, ~40–50 min):**
  - Big-picture map of how LLMs are built
  - Base model vs assistant model
  - Why hallucinations and other limitations happen
- **Part 2 (Guided Studio, ~60–75 min):**
  - Prompting and evaluation workflow
  - Verification routines and critical use in practice
- **Debrief (10–15 min):**
  - Reflection on trust, authorship, and responsible integration

## Part 1: Big Picture + Core Concepts

**Format:** Lecture + guided discussion

- **NotebookLM:**
  - [Notebook link](https://notebooklm.google.com/notebook/4558b471-595c-4407-98c8-bffd0d3ff6c6)

Use this NotebookLM 👆 to listen to an interactive podcast, watch a video summary, review core sources, ask questions, and generate quick study summaries before or after class.
> If you’re **taking this class asynchronously**, use the notebook as your primary resource instead of the slides.

- **Slides:**
  - [Presentation](https://ai.massol.me/block-ai-text-generation-slides/)
- **Core notes:**
  - [00 – Quick History of Text Generative Models](./content/00-quick-history-text-generative-models.md)
  - [01 – Big Picture LLM Pipeline](./content/01-big-picture-llm-pipeline.md)
  - [02 – Pretraining & Base Models](./content/02-pretraining-base-models.md)
  - [03 – From Base Model to Assistant](./content/03-from-base-model-to-assistant.md)
  - [07 – Inference & RAG in Practice (Bridge Note)](./content/07-inference-and-rag-in-practice.md)

## Part 2: Studio + Critical Practice

**Format:** Guided workshop

- **Practice notes:**
  - [04 – Hallucinations, Tools, and Context](./content/04-hallucinations-tools-and-context.md)
  - [05 – LLM Psychology and Limitations](./content/05-llm-psychology-and-limitations.md)
  - [06 – Studio Workflow and Critical Practice](./content/06-studio-workflow-and-critical-practice.md)

- **Samples notebooks (Jupyter / Colab):**
  - [01 – System Prompt Playground ](./samples/01-system-prompt.ipynb)
  - [02 – Simple RAG + Personas + Chat Memory ](./samples/02-simple-rag-personas.ipynb)
  - [03 – Embeddings + Tiny Semantic Search ](./samples/03-embeddings-semantic-search.ipynb)
  - [04 – Hugging Face Model Loading Quickstart](./samples/04-huggingface-model-loading-quickstart.ipynb)

## Preparation (Between classes)

- Watch: [Intro to Large Language Models (Andrej Karpathy)](https://www.youtube.com/watch?v=zjkBMFhNj_g)
- Read in order: content notes 01 → 06
- Bring one concrete use case where you want to use an LLM (drafting, research, ideation, coding, etc.)

## Going Further

- [How does GPT work? (simple explainer)](https://confusedbit.dev/posts/how_does_gpt_work/)
- [Transformers explained (video)](https://www.youtube.com/watch?v=SZorAJ4I-sA)
- [Deep Dive into LLMs like ChatGPT](https://www.youtube.com/watch?v=7xTGNNLPyMI)

## Tools

- [OpenWebUI](https://openwebui.com/)
- [Ollama](https://ollama.com/)
- [Hugging Face](https://huggingface.co/)
- [Google Colab](https://colab.research.google.com/)
