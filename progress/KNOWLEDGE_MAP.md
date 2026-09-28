# Knowledge Map

Use this file to distinguish:

- Known well
- Known practically
- Known superficially
- Currently learning
- Unknown
- Intentionally deferred

The status reflects demonstrated evidence, not familiarity with terminology.

## Foundations

| Topic | Status | Evidence |
|---|---|---|
| Python | Existing professional skill | Professional experience |
| Statistics | Existing professional skill | Professional experience |
| Classical ML | Existing professional skill | Professional experience |
| Optimization | Known superficially | Basic understanding of loss minimization and learning-rate effects |
| Neural networks | Unknown | Diagnostic |
| Backpropagation | Currently learning | Diagnostic revealed conceptual gap |
| Gradient descent | Known superficially | Correct general intuition; needs precise distinction from backpropagation |
| Autograd | Unknown | Diagnostic |
| PyTorch | To assess | Not yet directly assessed |

## LLM Foundations

| Topic | Status | Evidence |
|---|---|---|
| Tokenization | Known superficially | Understands basic tokenization idea; currently word-oriented mental model |
| Embeddings | Unknown | Diagnostic |
| Next-token prediction | Unknown | Diagnostic |
| Attention | Unknown | Diagnostic |
| Q/K/V | Unknown | Diagnostic |
| Scaled dot-product attention | Unknown | Diagnostic |
| Causal masking | Unknown | Diagnostic |
| Positional information | Unknown | Diagnostic |
| Transformers | Unknown | Diagnostic |
| Pretraining | Unknown | Diagnostic |
| Instruction tuning | Unknown | Diagnostic |
| Preference optimization | Unknown | Not yet assessed |
| Inference | Unknown | Diagnostic |
| Sampling | Unknown | Diagnostic |
| KV cache | Unknown | Diagnostic |
| Quantization | To assess | Practical local-model experience but internals not assessed |

## LLM Engineering

| Topic | Status | Evidence |
|---|---|---|
| Prompting | Known practically | Professional LLM work |
| Structured output | To assess | Not directly assessed |
| RAG | Known practically | Built/used retrieval systems |
| Hybrid retrieval | Known practically | Semantic + lexical retrieval experience |
| Metadata filtering | Known practically | Metadata-aware retrieval experience |
| Retrieval evaluation | Known practically | Precision@5, Recall@5, nDCG@5 |
| End-to-end LLM evaluation | Currently learning | Manual evaluation experience; no automated harness |
| Tool use | Known practically | Understands tool selection and parameter extraction |
| Agents | Known superficially | Practical exposure; workflow/agent distinction needs refinement |
| Observability | To assess | Not directly assessed |
| Prompt injection | Known practically | Internal work/experience |

## Fine-Tuning

| Topic | Status | Evidence |
|---|---|---|
| Fine-tuning concept | Known practically | Has performed model adaptation |
| LoRA | Known practically | Used LoRA on TinyLlama 1.1B |
| LoRA mechanics | Unknown | Underlying mathematical mechanism not yet explainable |
| Dataset construction | To assess | Not directly assessed |
| Evaluation before/after tuning | To assess | No systematic automated evaluation yet |

## Local LLM / Inference

| Topic | Status | Evidence |
|---|---|---|
| MLX | Known practically | Used for local model experiments |
| TinyLlama 1.1B | Known practically | Local experimentation + LoRA |
| Qwen models | Known practically | Local experimentation |
| Local model serving | To assess | Practical use exists; architecture not yet assessed |
| Inference optimization | Unknown | Diagnostic |
| KV cache | Unknown | Diagnostic |
| Quantization mechanics | To assess | Local-model exposure but underlying mechanics not assessed |

## Research

| Topic | Status | Evidence |
|---|---|---|
| Paper reading | Not assessed | — |
| Reproduction | Not assessed | — |
| Experiment design | Existing DS skill; LLM-specific assessment pending | Professional background |
| Technical writing | Existing professional skill; LLM-specific assessment pending | Professional experience |

## Current highest-priority gaps

1. Backpropagation
2. Neural-network computation
3. Autograd
4. Tokenization
5. Embeddings
6. Next-token prediction
7. Attention
8. Q/K/V
9. Causal masking
10. Transformer blocks
11. Inference mechanics
12. LoRA mechanics
13. Automated LLM evaluation
14. Agent architecture and evaluation

## Current learning rule

Do not mark a topic as mastered because it has been explained.

For important topics, evidence should eventually include:

1. Simple explanation
2. Mathematical understanding where relevant
3. Minimal implementation
4. Modern implementation
5. Debugging ability
6. Experiment
7. Interpretation of results
8. Failure modes
9. Limitations
10. Knowing when not to use it