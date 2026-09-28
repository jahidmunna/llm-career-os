# Current Context

Last updated: 2026-09-28

## Current mission

Build deep, portable expertise in LLMs and Generative AI while maintaining the ability to adapt rapidly as the field changes.

The goal is not merely to use LLM frameworks. The goal is to understand the underlying mechanisms well enough to build, debug, evaluate, adapt, and explain LLM systems independently.

## Current stage

Day 1 — Baseline diagnostic completed; foundational learning beginning.

## Learning mode

The learning process should proceed **one concrete concept at a time**.

For each concept:

1. Explain one concept.
2. Give one focused example.
3. Give one exercise.
4. Let the user attempt it.
5. Correct misconceptions.
6. Record the durable learning.
7. Only then move to the next concept.

Do not present multiple lessons or exercises at once unless explicitly requested.

## Current technical position

The user has professional AI/LLM application experience.

Existing practical experience includes:

- Building an internal VOC assistant for network engineers to diagnose problems and identify root causes.
- LangChain.
- Local LLM experimentation using MLX.
- TinyLlama 1.1B and other local models including Qwen.
- LoRA fine-tuning of TinyLlama 1.1B for internal usage.
- RAG design using hybrid retrieval concepts.
- Semantic and lexical retrieval.
- Metadata-aware retrieval.
- Retrieval metrics including Precision@K, Recall@K, and nDCG@K.
- Tool-calling concepts including tool selection and parameter extraction.
- Prompt-injection-related work.
- Manual evaluation of LLM systems.

Do not restart from generic software engineering, Python, or basic AI application material.

## Current capability profile

### Strong / practical

- LLM application engineering
- RAG architecture
- Hybrid retrieval
- Semantic and lexical retrieval
- Metadata-aware retrieval
- LangChain
- Local LLM experimentation
- Basic tool calling
- LoRA practical usage
- Retrieval evaluation metrics

### Working / partial

- Optimization intuition
- Learning-rate intuition
- Agent vs workflow concepts
- LLM evaluation methodology
- Deep-learning fundamentals

### Significant gaps

- Backpropagation mechanics
- Automatic differentiation / autograd
- Neural-network mechanics
- Tokenization details
- Embeddings
- Next-token prediction
- Attention
- Q/K/V
- Scaled dot-product attention
- Causal masking
- Transformer blocks
- Positional information
- Pretraining
- Instruction tuning
- Inference mechanics
- Sampling
- KV cache
- Underlying mechanics of LoRA

## Important diagnostic observations

The user initially described gradient descent as helping backpropagation. This indicates a conceptual distinction between:

- calculating gradients through backpropagation
- using gradients to update parameters through gradient descent/optimization

needs to be established.

The user understands the general learning-rate tradeoff but currently describes it in terms of reaching/skipping a global minimum. This should be refined later into a more accurate understanding of optimization landscapes.

The user's tokenization model is currently word-oriented. Modern LLM tokenization needs to be learned from a subword/token perspective.

The user has practical LoRA experience despite not currently being able to explain the underlying training mechanics. This should be used as a bridge into deep-learning fundamentals rather than treated as a beginner topic.

## Agent diagnostic

The user initially reversed the workflow/agent distinction.

Current correction:

A mostly predetermined sequence such as:

User → LLM → Search → LLM → Answer

is generally a workflow.

A system where the model repeatedly determines what action to take based on observations is agentic:

User → LLM decides → Tool → observation → LLM decides → Tool → ...

The important distinction is runtime control over the next action, not simply the number of steps.

## Evaluation diagnostic

The user demonstrated familiarity with retrieval evaluation:

- Precision@5
- Recall@5
- nDCG@5

However, end-to-end LLM evaluation and systematic RAG failure analysis remain areas to develop.

Current evaluation experience is primarily manual, including work around prompt injection. No automated LLM evaluation harness has yet been built.

## Current learning priority

The highest-value path is:

1. Backpropagation and gradient descent distinction
2. Neural-network computation and computation graphs
3. Autograd
4. Tokenization
5. Embeddings
6. Next-token prediction
7. Attention / QKV
8. Causal masking
9. Transformer block
10. Transformer implementation
11. LLM training
12. Inference
13. LoRA mechanics
14. Evaluation
15. Modern LLM systems

The curriculum should connect each theoretical concept to the user's existing practical experience.

## Current active lesson

### Concept: Backpropagation vs Gradient Descent

Core distinction:

- Backpropagation calculates gradients of the loss with respect to parameters.
- Gradient descent / an optimizer uses those gradients to update parameters.

Example:

```text
w_new = w_old - learning_rate * gradient