# LLM / Generative AI Mastery Roadmap

## North Star

Become a T-shaped LLM/GenAI specialist:

- **Deep:** LLM internals, training/adaptation, inference, evaluation, research
- **Broad:** RAG, agents, multimodal, LLMOps, product/system design
- **Portable:** able to move between models, frameworks, vendors, and AI assistants

The target is not "know every new AI tool."

The target is:

> Understand the underlying ideas well enough that new tools become learnable implementation details.

---

# The Operating Model

## 1. Learn by building

Every important concept should produce code, an experiment, or a concrete explanation.

## 2. Diagnose before studying

Do not assume a prerequisite is missing.

If you already know it, demonstrate it and move on.

If the diagnostic exposes a gap, patch only that gap.

## 3. Papers → Code → Experiment → Explanation

For important ideas:

1. Read the problem and contribution.
2. Implement a simplified version.
3. Run an experiment.
4. Compare against a baseline.
5. Explain what happened.
6. Record limitations.

## 4. The 2-day rule

If blocked for more than two focused days:

- reduce the scope
- create a smaller reproduction
- document the blocker
- move forward
- return later

Momentum matters more than perfect sequencing.

## 5. Public evidence

Build a visible body of work:

- GitHub
- technical write-ups
- experiment reports
- occasional LinkedIn posts when there is something worth sharing

Publishing is an output of learning, not the purpose of learning.

## 6. Free-first engineering

Primary resources:

- local Mac execution
- open-source models
- official documentation
- papers
- free educational material
- free compute when genuinely available

Do not make the curriculum depend on a specific provider's free-tier quota. Availability changes.

---

# Skill Map

## A. Mathematical and deep-learning foundations

Only learn what is necessary, and revisit math when a topic demands it.

- vectors and matrices
- dot products and matrix multiplication
- derivatives and gradients
- chain rule
- probability distributions
- softmax
- cross-entropy
- optimization
- backpropagation
- PyTorch/autograd

## B. Transformer / LLM internals

- tokenization
- embeddings
- self-attention
- multi-head attention
- causal masking
- positional representations
- RoPE
- residual streams
- normalization
- feed-forward blocks
- decoder-only architectures
- training objectives
- scaling
- instruction tuning
- preference optimization
- inference
- KV cache
- quantization

## C. LLM engineering

- prompting as interface design
- structured outputs
- tool calling
- context engineering
- retrieval
- reranking
- RAG
- evaluation
- observability
- reliability
- latency
- cost
- security

## D. Agents

- tool-use loops
- workflows vs agents
- state
- planning
- memory
- guardrails
- failure recovery
- evaluation

Frameworks come after understanding the underlying loop.

## E. Adaptation

- supervised fine-tuning
- PEFT
- LoRA
- QLoRA
- dataset construction
- data quality
- DPO / preference optimization
- evaluation before/after adaptation

## F. Systems

- inference memory
- KV cache
- batching
- quantization
- throughput
- latency
- serving
- CPU/GPU/Apple Silicon constraints
- distributed concepts

## G. Multimodal

- vision-language models
- document understanding
- OCR
- image reasoning
- audio/speech
- multimodal evaluation

## H. Research

- paper triage
- deep paper reading
- reproduction
- ablation
- benchmark design
- experiment design
- technical writing
- open-source contribution

---

# 12-Month Arc

## Months 1–3 — Foundations + Core LLM Engineering

Outcome:

- strong Transformer mental model
- tiny Transformer/GPT implementation
- RAG system
- evaluation harness
- tool-use system
- initial research reading habit

## Months 4–6 — Adaptation + Systems

Outcome:

- LoRA/QLoRA experiment
- inference/quantization benchmark
- deeper evaluation
- production-style LLM architecture
- first serious paper reproductions

## Months 7–9 — Specialization

Choose one primary specialization:

- LLM systems/inference
- agentic systems
- retrieval/document intelligence
- multimodal
- model adaptation/training
- evaluation/reliability

Keep secondary breadth.

## Months 10–12 — Research + Reputation

Outcome:

- substantial technical project
- meaningful open-source contribution
- multiple paper reproductions
- technical writing
- one original experiment/question
- strong public portfolio

The specialization can change after evidence; it is not a permanent decision.

---

# What "Mastered" Means

A topic is not mastered because you watched a course.

For an important topic, aim to be able to:

1. Explain it without notes.
2. Implement a minimal version.
3. Use a modern implementation.
4. Debug a failure.
5. Measure relevant behavior.
6. Explain limitations.
7. Know when not to use it.

Not every topic requires all seven. The deeper the topic, the more of these should be demonstrated.
