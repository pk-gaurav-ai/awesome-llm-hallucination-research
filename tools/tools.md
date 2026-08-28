# Tools and Libraries

General-purpose, actively maintained open-source libraries for measuring or guarding against hallucination in LLM applications (as opposed to the paper-specific research code in [`../implementations/`](../implementations/)).

- **Ragas** — [github.com/explodinggradients/ragas](https://github.com/explodinggradients/ragas)
  Lightweight, reference-free evaluation library purpose-built for RAG pipelines. Ships faithfulness, answer-relevancy, context-precision, and context-recall metrics that map directly onto this paper's "evidence faithfulness" dimension.

- **DeepEval** — [github.com/confident-ai/deepeval](https://github.com/confident-ai/deepeval)
  Pytest-style open-source LLM evaluation framework with a built-in hallucination metric plus G-Eval, task-completion, and RAG-specific (faithfulness, contextual precision/recall) metrics for CI-integrated testing.

- **TruLens** — [github.com/truera/trulens](https://github.com/truera/trulens)
  Open-source, OpenTelemetry-native evaluation and tracing library built around the "RAG Triad" (context relevance, groundedness, answer relevance) for continuous production monitoring.

- **Guardrails AI** — [github.com/guardrails-ai/guardrails](https://github.com/guardrails-ai/guardrails)
  Wraps LLM API calls with validators (including hallucination/groundedness and PII checks) that can trigger corrective re-generation when an output fails a check.

- **SelfCheckGPT** (PyPI: `selfcheckgpt`) — see [`../implementations/`](../implementations/) for the source repository
  Installable as a standalone package (`pip install selfcheckgpt`) providing zero-resource, black-box consistency-based hallucination scoring that can be dropped into any generation pipeline.
