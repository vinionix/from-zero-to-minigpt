# Technical Overview — From Zero to MiniGPT

## 1. Purpose

This repository is a long-form engineering study of how modern language models are built. The goal is not to assemble a chatbot from high-level APIs, but to reconstruct the path from mathematical foundations to a small decoder-only Transformer and then use that model inside a complete LLM system.

The project deliberately separates **implemented work** from **planned work**. A roadmap item is not considered complete merely because a library can perform it; the underlying concept must be understood, implemented, tested and documented.

## 2. Learning and engineering method

Each stage follows the same loop:

1. understand the mathematical idea;
2. solve at least one small example manually;
3. implement the idea in code;
4. create tests for important behavior;
5. vary parameters and observe failures;
6. document results and limitations.

This creates a traceable progression from theory to implementation instead of a collection of disconnected notebooks.

## 3. Planned technical progression

```text
Basic mathematics
      ↓
Vectors, matrices, derivatives and probability
      ↓
Linear regression
      ↓
Logistic neuron / classification
      ↓
MLP + backpropagation
      ↓
Sequence modelling
      ↓
Embeddings
      ↓
Self-attention + causal masking
      ↓
Decoder-only Transformer
      ↓
MiniGPT
      ↓
Post-training / preference learning
      ↓
API + retrieval + tools + evaluations + security
```

Early stages prioritize Python and NumPy so the calculations remain visible. PyTorch is intentionally introduced later, after gradients and network mechanics have been implemented without automatic differentiation hiding the core process.

## 4. Repository architecture

The repository is organized as a sequence of learning modules rather than a single monolithic application. Planned top-level areas include foundations, experiments, tests and documentation.

Each module should contain enough context to answer four questions:

- What problem is being solved?
- What mathematics is required?
- How is the concept implemented?
- What did the experiment demonstrate or fail to demonstrate?

## 5. Validation criteria

A stage is only complete when it can be explained and reproduced. Useful evidence includes:

- derivations or worked examples;
- deterministic tests;
- plots or experiment outputs;
- comparisons between parameter choices;
- documented failure modes;
- notes describing assumptions and limitations.

This is important because a model that runs is not necessarily a model that is understood.

## 6. Final-system direction

The final stage is planned as a technical assistant for networking, infrastructure or cybersecurity. The system should combine:

- a language model;
- document retrieval;
- constrained tools;
- automated evaluations;
- observability;
- controls for prompt injection and unsafe tool usage.

That final system is intentionally downstream of the model-building work: the repository first studies how the model learns, then how a model is operated safely inside a software system.

## 7. Current maturity

This is an **active learning and implementation project**. The README roadmap is the source of truth for progression. Future capabilities listed in the roadmap should be interpreted as planned until their code, tests and notes are present in the corresponding module.

## 8. Portfolio value

The repository is intended to demonstrate:

- mathematical growth applied directly to AI;
- ability to learn difficult topics incrementally;
- implementation-first study rather than API-only usage;
- experimental discipline;
- testing and documentation habits;
- understanding of the path from model internals to production-oriented LLM systems.

## 9. Documentation policy

When a new stage is completed, its documentation should record:

- objective;
- prerequisites;
- equations and intuition;
- implementation choices;
- tests;
- experiment results;
- known limitations;
- next dependency in the roadmap.

This keeps the repository useful both as a learning journal and as technical evidence for code review or recruiting conversations.
