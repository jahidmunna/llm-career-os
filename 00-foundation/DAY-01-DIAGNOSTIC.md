# Day 1 Diagnostic

## Purpose

This is not an exam.

Its purpose is to prevent wasting weeks learning things you already know and to expose the highest-value gaps.

Answer **without searching** first.

Use diagrams, equations, pseudocode, or plain language.

---

## A. Deep Learning

### 1. Backpropagation
Explain how a parameter gets updated after computing a loss.

### 2. Autograd
What does an automatic differentiation system actually calculate/store?

### 3. Optimization
Why can a smaller learning rate make training slower, and why can a larger one make training unstable?

---

## B. LLM Foundations

### 4. Tokenization
What is a tokenizer doing and why does tokenization matter?

### 5. Embeddings
What is an embedding and why can dot products between embeddings be useful?

### 6. Next-token prediction
How does next-token prediction create a training objective?

---

## C. Transformers

### 7. Attention
Given Q, K, V, describe the computation.

### 8. Scaling
Why is attention commonly scaled by the square root of the key dimension?

### 9. Causal masking
Why is it necessary for autoregressive generation?

### 10. Transformer block
Describe the major components of a decoder-only Transformer block.

### 11. Positional information
Why does a Transformer need information about token position?

---

## D. LLM Training / Adaptation

### 12. Pretraining vs instruction tuning
What changes conceptually?

### 13. Fine-tuning vs prompting
When might fine-tuning be preferable?

### 14. LoRA
What problem is parameter-efficient fine-tuning trying to solve?

---

## E. Inference

### 15. Generation
What happens when a model generates one new token?

### 16. Sampling
What do temperature, top-k, and top-p change?

### 17. KV cache
What problem does the KV cache solve?

---

## F. LLM Engineering

### 18. RAG
Where does retrieval happen in an LLM application?

### 19. RAG failure
If the final answer is wrong, how would you determine whether retrieval or generation caused the failure?

### 20. Evaluation
How would you prove that an LLM application improved?

---

## G. Agents

### 21. Tool use
What information must an LLM receive to reliably call a tool?

### 22. Agent vs workflow
What makes a system agentic rather than simply a deterministic workflow?

---

## H. Your existing professional experience

Answer factually:

### 23. What LLM/GenAI systems have you personally built?

### 24. Which LLM frameworks/libraries have you used professionally?

### 25. Have you deployed an LLM system? If yes, what was the architecture?

### 26. Have you fine-tuned a model? If yes, how?

### 27. Have you built an evaluation system for an LLM application?

---

# Scoring

For questions 1–22:

- 0 = cannot explain
- 1 = vague/partial
- 2 = technically correct
- 3 = technically correct + can reason about failure modes

Do not optimize for the score.

The purpose is to identify gaps.

---

# Output

Record:

- strongest 5 areas
- weakest 5 areas
- surprising gaps
- topics that should be skipped
- topics that need immediate attention

Update:

`progress/KNOWLEDGE_MAP.md`

and

`ai-context/CURRENT_CONTEXT.md`
