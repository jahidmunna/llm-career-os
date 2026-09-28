# First 90 Days — LLM / GenAI Acceleration

## Mission

Move from experienced AI/Data Scientist toward technically credible LLM/GenAI specialist through deliberate building, evaluation, and research literacy.

The roadmap is adaptive. The **weekly outcome** matters more than rigid daily scheduling.

---

# WEEK 0 — BASELINE

## Goal

Discover what you already know.

Complete:

`00-foundation/DAY-01-DIAGNOSTIC.md`

Also answer:

- What parts of PyTorch can I use without documentation?
- Can I derive/implement a training loop?
- Can I explain backpropagation?
- Can I explain attention mathematically?
- Can I build and evaluate an LLM application today?
- Which LLM systems have I actually shipped?

### Output

Update:

- `progress/KNOWLEDGE_MAP.md`
- `ai-context/CURRENT_CONTEXT.md`

---

# WEEK 1 — MATH PATCH + PYTORCH

Do not spend three weeks passively studying mathematics.

Patch only the gaps exposed by the diagnostic.

## Focus

- vectors/matrices
- dot products
- matrix multiplication
- gradients
- chain rule
- softmax
- cross-entropy
- autograd

## Build

1. Tiny tensor/math exercises.
2. A minimal PyTorch training loop.
3. A tiny neural network.

## Optional deeper exercise

Implement a small automatic differentiation engine or study a micrograd-style implementation.

### Gate

You can explain:

`forward → loss → gradient → update`

and inspect the major tensors in a PyTorch model.

---

# WEEK 2 — TOKENIZATION + EMBEDDINGS + LANGUAGE MODELING

## Learn

- tokens
- vocabulary
- BPE intuition
- embeddings
- logits
- next-token prediction
- cross-entropy

## Build

- inspect a real tokenizer
- visualize/inspect embeddings
- build a tiny character/token language model

### Gate

Explain:

`text → tokens → embeddings → model → logits → probabilities → next token`

---

# WEEK 3 — ATTENTION FROM FIRST PRINCIPLES

## Learn

- Q/K/V
- scaled dot-product attention
- causal mask
- multi-head attention

## Build

Implement attention manually in PyTorch.

## Break it

Intentionally test:

- incorrect masking
- wrong tensor shapes
- different sequence lengths
- different head dimensions

### Gate

Explain why causal masking is required for autoregressive language modeling.

---

# WEEK 4 — TRANSFORMER

## Learn

- Transformer block
- residual connections
- normalization
- feed-forward layer
- positional representations
- RoPE concept
- decoder-only architecture

## Build

A tiny GPT-style model.

Train it locally.

### Deliverable

Clean GitHub repository with:

- architecture diagram
- training instructions
- sample outputs
- known limitations

### Gate

Whiteboard the model without notes.

---

# WEEK 5 — MODERN LLM MENTAL MODEL

## Learn

- pretraining
- instruction tuning
- preference optimization
- prompting
- decoding
- temperature
- top-k/top-p
- context windows
- inference

## Read

Start the paper workflow:

`problem → contribution → figure/table → implementation → experiment → explanation`

### Deliverable

First paper implementation note.

---

# WEEK 6 — LLM APPLICATION ENGINEERING

## Learn

- structured outputs
- schemas
- validation
- retries
- context engineering
- deterministic vs stochastic behavior

## Build

A structured extraction system.

## Measure

- valid-output rate
- correction rate
- latency
- failure categories

### Gate

You can explain why "the model produced a bad answer" is not a sufficient debugging diagnosis.

---

# WEEK 7 — EMBEDDINGS + RETRIEVAL

## Learn

- embedding spaces
- cosine/dot-product similarity
- dense retrieval
- lexical retrieval
- chunking

## Build

Local retrieval system.

## Experiment

Compare:

- two chunking strategies
- two retrieval configurations

### Deliverable

Experiment report with a baseline.

---

# WEEK 8 — RAG

## Learn

- retrieval pipeline
- context construction
- reranking
- grounding
- citation
- retrieval failure modes

## Build

Complete local RAG system.

## Evaluate

Create a small test set and label:

- retrieval success
- answer correctness
- grounding

### Gate

You can identify whether a failure came from:

- retrieval
- context construction
- generation
- evaluation

---

# WEEK 9 — EVALUATION

## Learn

- evaluation datasets
- task-specific metrics
- human evaluation
- model-based evaluation
- LLM-as-judge limitations
- regression testing

## Build

Reusable evaluation harness for the RAG system.

### Deliverable

A before/after comparison for at least one system change.

---

# WEEK 10 — TOOL USE

## Learn

- function/tool calling
- schemas
- tool selection
- tool results
- state

## Build

A minimal tool-using LLM loop without an agent framework.

## Break

Test:

- invalid arguments
- missing arguments
- tool failure
- wrong tool selection
- repeated tool calls

---

# WEEK 11 — AGENTS

## Learn

- workflow vs agent
- loops
- planning
- state
- memory
- guardrails
- failure recovery

## Build

One narrow agent for a measurable task.

Do not build a generic "AI assistant."

### Evaluate

- task completion
- tool accuracy
- unnecessary actions
- failure recovery
- cost/latency where measurable

---

# WEEK 12 — ADAPTATION + INFERENCE

Split the week.

## Adaptation

Understand:

- supervised fine-tuning
- PEFT
- LoRA
- QLoRA
- dataset quality
- evaluation before/after tuning

Run a small local or free-compute experiment if practical.

## Inference

Understand:

- KV cache
- quantization
- memory
- throughput
- latency

Run a local benchmark.

---

# DAYS 85–90 — SYNTHESIS

Choose one project combining several capabilities.

Good shape:

`retrieval + tool use + structured output + evaluation`

or another technically meaningful system.

## Final 90-day portfolio

Aim to have:

1. Transformer implementation
2. Tiny language model
3. RAG system
4. Evaluation harness
5. Tool-use system
6. Adaptation experiment
7. Inference benchmark
8. One polished project
9. One technical write-up
10. Updated knowledge map

---

# WEEKLY RHYTHM

Default schedule:

### Mon–Wed
Learn + implement.

### Thu–Fri
Build + experiment.

### Saturday
Write a technical artifact:

- README
- experiment report
- paper note
- technical post

### Sunday
Read one important paper section, inspect a new development, or rest.

Do not force weekly publication if there is nothing technically meaningful to publish.

---

# 90-DAY SUCCESS TEST

At Day 90, you should be able to discuss and demonstrate:

- Transformer architecture
- attention
- LLM training/inference basics
- RAG
- evaluation
- tool use
- agents
- fine-tuning concepts
- inference optimization basics

More importantly, you should have **evidence** rather than claims.
