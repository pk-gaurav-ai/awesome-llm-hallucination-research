# Datasets

Benchmark datasets used for training or evaluating hallucination-detection and factuality methods, referenced in the accompanying paper and citation audit.

- **TruthfulQA**
  Source: [github.com/sylinrl/TruthfulQA](https://github.com/sylinrl/TruthfulQA) (official release accompanying Lin et al., 2022)
  Description: 817 adversarially-written questions across 38 categories designed to elicit imitative human falsehoods and misconceptions.
  Use in this repo: primary benchmark referenced for Type X (reasoning-induced/confidence hallucination) and truthfulness evaluation in the paper's §2.3.

- **HaluEval**
  Source: [github.com/RUCAIBox/HaluEval](https://github.com/RUCAIBox/HaluEval) (official release accompanying Li et al., 2023)
  Description: 35,000 examples — 5,000 general ChatGPT-response queries plus 30,000 task-specific (QA, dialogue, summarization) samples with human-labeled hallucinated vs. non-hallucinated responses.
  Use in this repo: cited in §1 as evidence that LLMs both generate and fail to recognize hallucinated content.

- **RAGTruth**
  Source: [github.com/ParticleMedia/RAGTruth](https://github.com/ParticleMedia/RAGTruth) (official release accompanying Niu et al., 2024)
  Description: ~18,000 naturally generated RAG responses with case- and word-level manual hallucination annotations.
  Use in this repo: cited in §5.1 and §6 as evidence that retrieval-augmented generation does not eliminate hallucination.

- **FActScore Knowledge Source & Atomic-Fact Annotations**
  Source: distributed as part of [github.com/shmsw25/FActScore](https://github.com/shmsw25/FActScore) (official release accompanying Min et al., 2023)
  Description: Wikipedia-derived knowledge source plus human/model-annotated atomic facts for biography generations, used to compute claim-level factual precision.
  Use in this repo: underpins the "atomic factuality evaluation" approach discussed in §5.3.
