# GitHub Implementations

Official research-code repositories for methods discussed in the paper. Each was checked for an active repository, clear documentation, and a direct link back to its paper (per the selection criteria in the assignment instructions).

- **FActScore** — [github.com/shmsw25/FActScore](https://github.com/shmsw25/FActScore)
  Official implementation of Min et al. (2023). Computes atomic-fact-level factual precision for long-form generations; installable via `pip install factscore`. Actively maintained with open issues/PRs.

- **SelfCheckGPT** — [github.com/potsawee/selfcheckgpt](https://github.com/potsawee/selfcheckgpt)
  Official implementation of Manakul et al. (2023). Provides BERTScore, QA-based (MQAG), n-gram, NLI, and LLM-prompting variants of the self-consistency check, plus the `wiki_bio_gpt3_hallucination` dataset.

- **Self-RAG** — [github.com/AkariAsai/self-rag](https://github.com/AkariAsai/self-rag)
  Official implementation of Asai et al. (2023/2024). Includes training code, the retrieval corpus setup, and evaluation scripts (integrating with the ALCE benchmark) for the adaptive-retrieval, self-critique framework.

- **DoLa** — [github.com/voidism/DoLa](https://github.com/voidism/DoLa)
  Official implementation of Chuang et al. (ICLR 2024). A decoding-time factuality intervention that requires no retrieval or fine-tuning — useful as a lightweight baseline to compare against retrieval-based mitigation.

- **Woodpecker** — [github.com/BradyFU/Woodpecker](https://github.com/BradyFU/Woodpecker)
  Official implementation of Yin et al. (2023/2024). Training-free, five-stage hallucination-correction pipeline for multimodal (vision-language) LLM outputs, evaluated on the POPE benchmark.

Related benchmark/tooling repositories also worth knowing (referenced from the papers above but not primary "implementations" in their own right):
- [github.com/RUCAIBox/HaluEval](https://github.com/RUCAIBox/HaluEval) — benchmark generation and evaluation code for Li et al. (2023).
- [github.com/princeton-nlp/ALCE](https://github.com/princeton-nlp/ALCE) — citation-quality evaluation harness for Gao et al. (2023), used by Self-RAG's own evaluation scripts.
