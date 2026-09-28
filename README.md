# LLM Career OS

A portable, zero-dollar learning and career system for becoming unusually strong at LLMs and Generative AI.

> **The repository is the source of truth. The AI is the replaceable tool.**

This system is designed so that your learning does **not** depend on ChatGPT, Claude, Gemini, a specific account, a subscription, a model, or even the continued existence of today's AI tools.

You can use the same repository with any AI system that can read text/files and help you reason, code, research, or review.

---

## 1. The goal

The goal is not simply to "learn LLMs."

The goal is to become capable of:

- understanding LLMs from first principles
- implementing important mechanisms yourself
- building reliable LLM systems
- evaluating and debugging them scientifically
- understanding training, adaptation, inference, RAG, agents, and multimodal systems
- reading papers and reproducing important ideas
- designing meaningful experiments
- explaining technical decisions clearly
- producing public evidence of your ability
- rapidly learning new AI developments without starting over every time the ecosystem changes

The core loop is:

**Learn → Build → Break → Measure → Explain → Publish → Update**

---

## 2. The most important rule

### Own your learning state.

Do not make an AI conversation your permanent memory.

Instead, store durable knowledge and progress in this repository:

- what you know
- what you do not know
- what you built
- what failed
- what you measured
- what you decided
- what you read
- what you want to learn next
- what another AI needs to know to continue helping you

An AI session is temporary.

This repository is persistent.

That makes the system portable.

---

## 3. You can use this with ANY AI

You do **not** need a particular AI account.

You can use:

- ChatGPT
- Claude
- Gemini
- another hosted assistant
- a local/open-source model
- a future AI system that does not exist yet
- multiple AIs during the same project

The workflow stays the same.

Only the interface changes.

### The invariant

```text
Your Git repository
        ↓
Your current context + roadmap + evidence
        ↓
Any AI assistant
        ↓
Learning / coding / research / review
        ↓
Results written back to the repository
        ↓
Git commit
        ↓
Next AI can continue
```

The AI should read from the repository and write useful state back into it.

---

# 4. How to start

## Step 1 — Put this repository under your own GitHub account

Create a private or public GitHub repository and push this folder.

For example:

```bash
cd llm-career-os

git init
git add .
git commit -m "Initial LLM Career OS"
git branch -M main
git remote add origin <YOUR_GITHUB_REPOSITORY>
git push -u origin main
```

Do not commit secrets, API keys, passwords, private credentials, or private company information.

The included `.gitignore` is the first line of protection, but always review files before committing.

---

## Step 2 — Read the operating system files

Start with these files:

1. `ai-context/SYSTEM.md`
2. `ai-context/CURRENT_CONTEXT.md`
3. `ai-context/LEARNING_PROTOCOL.md`
4. `ROADMAP.md`
5. `90-DAY-ROADMAP.md`
6. `progress/MILESTONES.md`
7. `progress/KNOWLEDGE_MAP.md`

Then run:

`00-foundation/DAY-01-DIAGNOSTIC.md`

Do **not** blindly start from beginner material.

You already have professional AI/software experience. The diagnostic exists to identify what should be skipped, what should be patched, and where deeper work is justified.

---

# 5. The universal AI handoff protocol

This is the most important part of the system.

Whenever you start a session with a new AI, give it the repository context before asking it to teach you.

## Minimum handoff

Provide these files:

```text
ai-context/SYSTEM.md
ai-context/CURRENT_CONTEXT.md
ai-context/LEARNING_PROTOCOL.md
```

For project work, also provide:

```text
ai-context/PROJECT_CONTEXT.md
projects/<current-project>/...
```

For research work, provide the relevant paper notes and experiment files.

For a roadmap decision, provide:

```text
ROADMAP.md
90-DAY-ROADMAP.md
progress/KNOWLEDGE_MAP.md
progress/MILESTONES.md
```

### Universal opening prompt

Use this with any AI:

```text
You are helping me operate my LLM Career OS.

The attached repository is the source of truth for my learning state.
Do not assume that your own conversation history is available later.
Do not restart from beginner material unless the repository or diagnostic shows a real gap.

First:
1. Read ai-context/SYSTEM.md
2. Read ai-context/CURRENT_CONTEXT.md
3. Read ai-context/LEARNING_PROTOCOL.md
4. Read the relevant roadmap/project/progress files
5. Identify my current state and the highest-value next step

Then:
- challenge my assumptions when appropriate
- prioritize understanding over memorization
- prefer implementation and experiments over passive explanation
- help me get unstuck quickly
- distinguish stable knowledge from fast-changing ecosystem facts
- do not invent current facts; verify them when freshness matters
- update the repository with durable results rather than leaving important state only in chat

Before finishing, tell me:
1. what we accomplished
2. what I learned
3. what remains uncertain
4. what should be written to the repository
5. the next concrete action
```

This prompt is intentionally provider-neutral.

---

# 6. Switching from one AI to another

Suppose you start with ChatGPT today and use Claude tomorrow.

Nothing important should be lost.

### Before leaving AI #1

Ask:

```text
Review this session and identify anything that should become durable knowledge or progress in my repository.

Update or propose changes for:
- CURRENT_CONTEXT.md
- KNOWLEDGE_MAP.md
- MISTAKES.md
- DECISIONS.md
- the relevant project/experiment notes
- SESSION_TEMPLATE.md if useful

Do not write temporary conversational details into the repository.
```

Commit the changes.

### When entering AI #2

Give it the repository context and say:

```text
Continue from the repository state.
Do not repeat completed work.
Identify the next highest-value step and begin there.
```

That is the entire portability mechanism.

---

# 7. You can use multiple AIs at the same time

You do not need to choose one permanent AI.

Different systems can have different jobs.

For example:

```text
AI A → primary learning / implementation
AI B → adversarial review
AI C → paper explanation
AI D → coding/debugging
AI E → alternative architecture critique
Local model → offline experimentation
```

The repository remains the shared state.

### Example

You implement attention with AI A.

You ask AI B:

> "Review this implementation. Look specifically for conceptual mistakes, masking errors, tensor-shape assumptions, and places where my explanation is misleading."

You ask AI C:

> "Explain the relevant paper and identify whether my implementation actually captures the paper's core idea."

You then record the final understanding in the repository.

The AIs disagree.

**The repository records the evidence and your current conclusion — not the authority of any particular AI.**

---

# 8. Free-first policy

This Career OS is intentionally designed to work with a **$0 budget**.

That means:

- free/open-source learning resources first
- local execution when practical
- public papers and documentation when available
- free software before paid software
- small experiments before expensive experiments
- existing hardware before buying hardware
- no paid course requirement
- no subscription dependency
- no proprietary API dependency for core learning

Paid tools can be useful later, but they must never become a prerequisite for understanding the underlying technology.

### Important distinction

There are three different things:

1. **Knowledge** — should remain portable.
2. **Experiments** — should remain reproducible where practical.
3. **Convenience tools** — may change constantly.

Do not confuse #3 with #1.

---

# 9. Do not hard-code today's AI ecosystem into the curriculum

AI changes quickly.

Model names, API formats, pricing, free tiers, context limits, hosted services, benchmarks, and frameworks can become obsolete.

Therefore:

### Stable knowledge belongs in the curriculum

Examples:

- gradient descent
- backpropagation
- tokenization concepts
- embeddings
- attention
- Transformer blocks
- autoregressive language modeling
- optimization
- retrieval
- evaluation methodology
- inference concepts
- distributed systems principles

### Fast-changing facts must be verified

Examples:

- current model capabilities
- current API syntax
- current pricing
- free quotas
- model context limits
- current hardware support
- current leaderboards
- hosted-service availability
- current framework APIs

See `resources/FRESHNESS_POLICY.md`.

If an AI tells you a current ecosystem fact, verify it when it matters.

---

# 10. The repository structure

```text
llm-career-os/
│
├── README.md                         ← This document
├── START-HERE.md                     ← First session entry point
├── ROADMAP.md                        ← Long-term direction
├── 90-DAY-ROADMAP.md                 ← Initial acceleration plan
│
├── ai-context/                       ← Portable AI context
│   ├── SYSTEM.md                     ← How the system should operate
│   ├── CURRENT_CONTEXT.md            ← Current state
│   ├── LEARNING_PROTOCOL.md          ← Learning rules
│   ├── PROJECT_CONTEXT.md            ← Project-level context
│   └── AI_HANDOFF.md                 ← Handoff instructions
│
├── 00-foundation/                    ← Diagnostics + foundations
├── 01-transformers/                  ← Transformer mechanics
├── 02-llm-internals/                 ← LLM internals
├── 03-llm-engineering/               ← Application engineering
├── 04-rag/                           ← Retrieval + RAG
├── 05-agents/                        ← Tool use + agents
├── 06-fine-tuning/                   ← Adaptation
├── 07-inference/                     ← Inference + systems
├── 08-multimodal/                    ← Multimodal models
├── 09-evaluation/                    ← Evaluation
├── 10-research/                      ← Research skills
│
├── projects/                         ← Real projects
├── experiments/                      ← Controlled experiments
├── papers/                           ← Paper notes + reproductions
├── prompts/                          ← Useful prompts/prompt experiments
│
├── progress/                         ← Learning state
│   ├── MILESTONES.md
│   ├── KNOWLEDGE_MAP.md
│   ├── SESSION_TEMPLATE.md
│   ├── WEEKLY_REVIEW.md
│   ├── MISTAKES.md
│   ├── DECISIONS.md
│   └── PUBLIC_ARTIFACTS.md
│
└── resources/                        ← External resources
    ├── BACKLOG.md
    ├── RESOURCE_INDEX.md
    ├── PAPER_QUEUE.md
    ├── TOOLS.md
    └── FRESHNESS_POLICY.md
```

The structure can evolve.

Do not preserve folders merely because they exist. Change the system when the workflow proves that a different structure works better.

---

# 11. What should be committed to Git?

Commit things that preserve learning state.

Good commits include:

```text
Add attention implementation and explanation
Record failed KV-cache experiment
Update knowledge map after Transformer study
Add paper reproduction notes
Document RAG retrieval failure
Complete Week 3 review
Add benchmark results for chunking experiment
```

Avoid commits containing:

- API keys
- passwords
- tokens
- private credentials
- proprietary company data
- private customer data
- huge generated datasets
- unnecessary model weights
- temporary files

Use `.gitignore` and common sense.

---

# 12. How a normal learning session works

A good session looks roughly like this:

```text
1. Read current context
        ↓
2. Choose ONE concrete objective
        ↓
3. Attempt it yourself
        ↓
4. Use AI as teacher / pair programmer / reviewer
        ↓
5. Implement something
        ↓
6. Break it deliberately
        ↓
7. Measure what happened
        ↓
8. Explain the result without AI help
        ↓
9. Record durable knowledge
        ↓
10. Commit to Git
```

The objective is not to have a productive conversation.

The objective is to become more capable.

---

# 13. The 30-minute and 2-day rules

## 30-minute rule

If you are completely stuck for around 30 focused minutes:

1. identify the exact blocker
2. ask for a hint or narrower explanation
3. try again
4. inspect a minimal working example
5. continue

Do not spend three hours staring at the same error because you think using help means you failed.

## 2-day rule

If a learning problem blocks progress for more than two focused days:

- reduce scope
- build a smaller version
- reproduce the idea on toy data
- document the blocker
- move forward
- revisit later

Deep learning matters.

Getting permanently stuck does not.

---

# 14. AI should not do all the thinking

Use AI heavily, but use it deliberately.

### Good uses

- explain a difficult concept
- challenge your reasoning
- review code
- generate test cases
- suggest experiments
- compare implementation approaches
- identify likely bugs
- help read unfamiliar code
- turn a paper into implementation questions
- act as an adversarial reviewer

### Dangerous uses

- copying code you cannot explain
- accepting explanations without testing them
- asking AI to solve every exercise before attempting it
- treating model output as evidence
- letting AI decide what you "know"
- letting a conversation become your only record

The target is **AI-assisted expertise**, not AI-dependent expertise.

---

# 15. Evidence-based mastery

A topic is not considered mastered because you read about it.

For important topics, aim to be able to:

1. explain it simply
2. explain the mathematics when relevant
3. implement a minimal version
4. use a modern implementation
5. debug a broken implementation
6. design an experiment around it
7. interpret the results
8. identify failure modes
9. explain limitations
10. know when **not** to use it

That is why this repository contains code, experiments, notes, mistakes, and public artifacts — not just bookmarks.

---

# 16. Public evidence

If appropriate, turn serious work into public evidence:

- GitHub repositories
- technical notes
- experiment reports
- paper reproductions
- demos
- technical articles
- thoughtful LinkedIn posts
- open-source contributions

See:

`progress/PUBLIC_ARTIFACTS.md`

The objective is not to manufacture activity.

The objective is to make real capability observable.

---

# 17. What happens when an AI disappears?

Nothing important should break.

If tomorrow:

- your AI subscription expires
- an AI provider changes its model
- a model becomes unavailable
- a company shuts down a product
- an API changes
- a free tier disappears
- a new model becomes much better

your repository still contains:

- your roadmap
- your knowledge
- your projects
- your experiments
- your mistakes
- your decisions
- your research notes
- your current state

You simply connect another tool to the repository.

That is the point of this architecture.

---

# 18. The long-term architecture

Think of the system as five layers:

```text
┌──────────────────────────────────────────────┐
│  YOU                                         │
│  judgment · curiosity · goals · decisions    │
└──────────────────────┬───────────────────────┘
                       │
┌──────────────────────▼───────────────────────┐
│  GIT REPOSITORY                              │
│  knowledge · progress · projects · evidence  │
└──────────────────────┬───────────────────────┘
                       │
┌──────────────────────▼───────────────────────┐
│  AI ASSISTANTS                               │
│  teaching · coding · critique · research     │
└──────────────────────┬───────────────────────┘
                       │
┌──────────────────────▼───────────────────────┐
│  TOOLS / FRAMEWORKS / MODELS                 │
│  PyTorch · libraries · APIs · model vendors  │
└──────────────────────┬───────────────────────┘
                       │
┌──────────────────────▼───────────────────────┐
│  HARDWARE / COMPUTE                          │
│  Mac · local machines · optional cloud       │
└──────────────────────────────────────────────┘
```

The lower layers can change.

Your capability and learning record should survive.

---

# 19. The 90-day and 12-month plans

Use both clocks.

### 90 days

The purpose is acceleration:

- foundations
- Transformer implementation
- LLM internals
- application engineering
- RAG
- evaluation
- tool use
- agents
- adaptation
- inference
- one serious portfolio-grade system

See `90-DAY-ROADMAP.md`.

### 12 months

The purpose is depth and differentiation:

- stronger foundations
- adaptation and systems
- specialization
- research capability
- public technical evidence
- open-source contribution
- deeper experimental work

See `ROADMAP.md`.

The roadmap is a hypothesis, not a prison.

Your diagnostic results and actual progress should change it.

---

# 20. A simple weekly operating rhythm

A default week can look like:

```text
Mon–Wed   Learn + implement
Thu–Fri   Build + experiment
Saturday  Write / explain / publish
Sunday    Review + papers + frontier scan + rest
```

But output matters more than calendar purity.

A week with one deep implementation and one excellent experiment is more valuable than a week of consuming 20 tutorials.

---

# 21. The rule for AI-generated repository changes

When an AI changes this repository, ask:

> **Will this still be useful if I switch to a completely different AI tomorrow?**

If yes, it probably belongs in the repository.

If no, it may belong only in the conversation.

This single question prevents a lot of unnecessary context pollution.

---

# 22. Start here today

If this is your first day with the repository:

```text
1. Put the repository on GitHub.
2. Read ai-context/SYSTEM.md.
3. Read ai-context/CURRENT_CONTEXT.md.
4. Run 00-foundation/DAY-01-DIAGNOSTIC.md.
5. Record the results.
6. Update progress/KNOWLEDGE_MAP.md.
7. Start the highest-value topic identified by the diagnostic.
8. Commit the result.
```

Do not spend the first week designing the perfect learning system.

**Use the system. Improve the system from evidence.**

---

## Final principle

> **You own the knowledge, the evidence, and the learning state. AI is the interface you can replace.**

The goal is not to become excellent at using one AI.

The goal is to become excellent enough at LLMs that **any new AI becomes another tool you can learn to use.**
