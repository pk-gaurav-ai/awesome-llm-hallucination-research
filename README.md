# Awesome LLM Hallucination Research

A curated collection of research papers, datasets, tools, implementations, and learning resources on **hallucination in Large Language Models for research and scholarly applications** — built around an AI-assisted research paper and an independent citation-integrity audit of that paper's references.

## Contents

- [Overview](#overview)
- [AI-Assisted Research Paper](#ai-assisted-research-paper)
- [Citation Integrity Audit](#citation-integrity-audit)
- [Survey and Review Papers](#survey-and-review-papers)
- [Foundational Papers and Benchmarks](#foundational-papers-and-benchmarks)
- [Detection Methods](#detection-methods)
- [Research Provenance / Citation-Aware Generation](#research-provenance--citation-aware-generation)
- [Retrieval-Augmented Generation and Grounding](#retrieval-augmented-generation-and-grounding)
- [Multimodal Hallucination](#multimodal-hallucination)
- [Datasets](#datasets)
- [Tools and Libraries](#tools-and-libraries)
- [GitHub Implementations](#github-implementations)
- [Tutorials and Learning Resources](#tutorials-and-learning-resources)
- [License](#license)

## Overview

Large Language Models (LLMs) are increasingly used as research assistants — for literature discovery, summarization, hypothesis generation, coding, and scholarly writing. Their central reliability problem is **hallucination**: fluent, plausible-sounding output that is unsupported, unverifiable, or factually wrong. This is not a single failure mode. It spans fabricated facts, entity/relation errors, temporal drift, contradiction of supplied evidence, unsupported inference, fabricated or non-supporting citations, quantitative errors, and overconfident reasoning.

This repository organizes that space around a research-oriented taxonomy (factual grounding, evidence faithfulness, research provenance, and reasoning/epistemic reliability) developed in the accompanying AI-assisted paper, together with a systematic citation-integrity audit that tested whether the paper's own AI-generated references could be trusted. Every scholarly resource linked below was independently checked for existence and correct metadata against a publisher page, DOI/arXiv record, or ACL Anthology entry — a citation is never included merely because it "looks" scholarly.

## AI-Assisted Research Paper

**"A Taxonomy of Hallucination Types in Large Language Models for Research Applications"**
[View Paper](paper/AI_Assisted_Research_Paper.pdf)

Proposes a four-dimension, ten-category taxonomy of research-oriented LLM hallucination and surveys current detection/mitigation approaches (RAG, citation-aware generation, atomic factuality evaluation, self-consistency, semantic entropy, chain-of-verification, and research-and-revision systems), concluding that no single technique eliminates hallucination and that a verification-centered, defense-in-depth architecture is needed for trustworthy scholarly AI.

## Citation Integrity Audit

[View Audit](citation-audit/Citation_Integrity_Audit.docx)

A ten-reference systematic sample of the AI-generated paper's 18-item bibliography was independently verified against DOI/arXiv/ACM/ACL records (first 3, last 3, and 4 evenly spaced references, to avoid cherry-picking suspicious-looking entries). **All ten sampled references were classified A — Verified** (publication exists; title, authors, year, venue, and identifier all match), for an authenticity score of **100/100**. The main integrity weakness found was not fabrication but completeness/traceability: two bibliography entries are uncited duplicates, and one source (RAGTruth) is discussed in the body text without an explicit in-text citation marker. Central lesson: a citation should never be trusted merely because it looks scholarly or carries a DOI — it must be checked to exist, and checked to actually support the claim it's attached to.

## Survey and Review Papers

See [`references/references.md`](references/references.md#survey-and-review-papers) — 4 papers establishing the intrinsic/extrinsic and factuality/faithfulness framing that this taxonomy builds on.

## Foundational Papers and Benchmarks

See [`references/references.md`](references/references.md#foundational-papers-and-benchmarks) — 5 papers, including TruthfulQA, HaluEval, and SelfAware.

## Detection Methods

See [`references/references.md`](references/references.md#detection-methods) — 5 papers, including FActScore, SelfCheckGPT, semantic entropy, Chain-of-Verification, and DoLa.

## Research Provenance / Citation-Aware Generation

See [`references/references.md`](references/references.md#research-provenance--citation-aware-generation) — ALCE and RARR.

## Retrieval-Augmented Generation and Grounding

See [`references/references.md`](references/references.md#retrieval-augmented-generation-and-grounding) — RAGTruth, Self-RAG, and FreshLLMs.

## Multimodal Hallucination

See [`references/references.md`](references/references.md#multimodal-hallucination) — Woodpecker.

## Datasets

See [`datasets/datasets.md`](datasets/datasets.md) — TruthfulQA, HaluEval, RAGTruth, and the FActScore knowledge source/annotations.

## Tools and Libraries

See [`tools/tools.md`](tools/tools.md) — Ragas, DeepEval, TruLens, Guardrails AI, and SelfCheckGPT-as-a-package.

## GitHub Implementations

See [`implementations/github-repositories.md`](implementations/github-repositories.md) — official code for FActScore, SelfCheckGPT, Self-RAG, DoLa, and Woodpecker.

## Tutorials and Learning Resources

See [`tutorials/tutorials.md`](tutorials/tutorials.md) — Anthropic's hallucination-reduction guidance plus the primary citation-verification sources (Google Scholar, Semantic Scholar, Crossref, arXiv) used throughout this audit.

## License

Repository content (README, audit summary, and original write-ups) is released under the [MIT License](LICENSE). Linked third-party papers, datasets, and code retain their own original licenses — see each source for details. No copyrighted third-party paper PDFs are redistributed in this repository; only the author's own AI-assisted paper and citation audit are included as files.

---

*Compiled as part of the "AI Tools for Research" course — GitHub Research Curation and Documentation activity.*
