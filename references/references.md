# Curated Research Papers

All papers below were checked for **existence, correct title/authors/year, and a valid persistent identifier (DOI/arXiv ID)** against publisher pages, ACL Anthology, arXiv, ACM DL, or Nature, following the verification procedure in [`citation-audit/`](../citation-audit/). Sixteen of these are the works cited in the AI-assisted paper itself (see the audit results); four more (marked ✳) were added and independently verified while building this collection, to broaden coverage of detection/mitigation methods and multimodal hallucination.

---

## Survey and Review Papers

- **Survey of Hallucination in Natural Language Generation**
  Z. Ji, N. Lee, R. Frieske, T. Yu, D. Su, Y. Xu, E. Ishii, Y. Bang, A. Madotto, P. Fung — 2023, *ACM Computing Surveys*, vol. 55, no. 12, Article 248
  [DOI: 10.1145/3571730](https://doi.org/10.1145/3571730)
  The foundational survey distinguishing intrinsic vs. extrinsic hallucination in NLG; the conceptual starting point for LLM-specific taxonomies.

- **Siren's Song in the AI Ocean: A Survey on Hallucination in Large Language Models**
  Y. Zhang, Y. Li, L. Cui, D. Cai, L. Liu, T. Fu, X. Huang, E. Zhao, Y. Zhang, Y. Chen, L. Wang, A. T. Luu, W. Bi, F. Shi, S. Shi — 2023, arXiv:2309.01219
  [arXiv:2309.01219](https://arxiv.org/abs/2309.01219)
  Characterizes hallucination as divergence from user input, prior context, and world knowledge.

- **A Survey on Hallucination in Large Language Models: Principles, Taxonomy, Challenges, and Open Questions**
  X. Huang et al. — 2025, *ACM Transactions on Information Systems*, Article 42
  [DOI: 10.1145/3703155](https://doi.org/10.1145/3703155)
  Organizes LLM hallucination into factuality vs. faithfulness hallucination; the most comprehensive recent taxonomy.

- **Factuality of Large Language Models: A Survey**
  Y. Wang, M. Wang, M. A. Manzoor, F. Liu, G. Georgiev, R. J. Das, P. Nakov — 2024, *Proceedings of EMNLP 2024*, pp. 19519–19529
  [arXiv:2402.02420](https://arxiv.org/abs/2402.02420)
  Distinguishes factuality, hallucination, relevance, and trustworthiness as separate evaluation axes.

## Foundational Papers and Benchmarks

- **TruthfulQA: Measuring How Models Mimic Human Falsehoods**
  S. Lin, J. Hilton, O. Evans — 2022, *ACL 2022*, pp. 3214–3252
  [DOI: 10.18653/v1/2022.acl-long.229](https://doi.org/10.18653/v1/2022.acl-long.229) · [arXiv:2109.07958](https://arxiv.org/abs/2109.07958)
  Shows LLMs can reproduce common human misconceptions rather than mere training-pattern likelihood.

- **HaluEval: A Large-Scale Hallucination Evaluation Benchmark for Large Language Models**
  J. Li, X. Cheng, X. Zhao, J.-Y. Nie, J.-R. Wen — 2023, *EMNLP 2023*, pp. 6449–6464
  [DOI: 10.18653/v1/2023.emnlp-main.397](https://doi.org/10.18653/v1/2023.emnlp-main.397)
  35K-example benchmark showing LLMs both generate and fail to recognize hallucinated content.

- **Language Models (Mostly) Know What They Know**
  S. Kadavath et al. — 2022, arXiv:2207.05221
  [arXiv:2207.05221](https://arxiv.org/abs/2207.05221)
  Shows LLMs have partial, imperfectly calibrated ability to predict whether their own answers are correct.

- **Do Large Language Models Know What They Don't Know?** ✳
  Z. Yin, Q. Sun, Q. Guo, J. Wu, X. Qiu, X. Huang — 2023, *Findings of ACL 2023*
  [arXiv:2305.18153](https://arxiv.org/abs/2305.18153)
  Introduces the SelfAware dataset (1,032 unanswerable + 2,337 answerable questions) to measure a model's self-knowledge boundary.

- **Lost in the Middle: How Language Models Use Long Contexts**
  N. F. Liu, K. Lin, J. Hewitt, A. Paranjape, M. Bevilacqua, F. Petroni, P. Liang — 2024, *Transactions of the ACL*, vol. 12, pp. 157–173
  [DOI: 10.1162/tacl_a_00638](https://doi.org/10.1162/tacl_a_00638) · [arXiv:2307.03172](https://arxiv.org/abs/2307.03172)
  Demonstrates the U-shaped performance drop when relevant evidence sits in the middle of a long context — relevant to why "just add more context" doesn't solve grounding.

## Detection Methods

- **FActScore: Fine-grained Atomic Evaluation of Factual Precision in Long Form Text Generation**
  S. Min, K. Krishna, X. Lyu, M. Lewis, W.-t. Yih, P. Koh, M. Iyyer, L. Zettlemoyer, H. Hajishirzi — 2023, *EMNLP 2023*, pp. 12076–12100
  [DOI: 10.18653/v1/2023.emnlp-main.741](https://doi.org/10.18653/v1/2023.emnlp-main.741)
  Decomposes long-form text into atomic facts and scores the supported fraction — the basis of claim-level (not document-level) factuality evaluation.

- **SelfCheckGPT: Zero-Resource Black-Box Hallucination Detection for Generative Large Language Models**
  P. Manakul, A. Liusie, M. J. F. Gales — 2023, *EMNLP 2023*, pp. 9004–9017
  [DOI: 10.18653/v1/2023.emnlp-main.557](https://doi.org/10.18653/v1/2023.emnlp-main.557) · [arXiv:2303.08896](https://arxiv.org/abs/2303.08896)
  Detects hallucination via self-consistency across sampled generations, without needing model internals or an external database.

- **Detecting Hallucinations in Large Language Models Using Semantic Entropy**
  S. Farquhar, J. Kossen, L. Kuhn, Y. Gal — 2024, *Nature*
  [DOI: 10.1038/s41586-024-07421-0](https://doi.org/10.1038/s41586-024-07421-0)
  Measures uncertainty over semantic-equivalence classes rather than token probabilities to flag unreliable outputs.

- **Chain-of-Verification Reduces Hallucination in Large Language Models**
  S. Dhuliawala, M. Komeili, J. Xu, R. Raileanu, X. Li, A. Celikyilmaz, J. Weston — 2023, arXiv:2309.11495
  [arXiv:2309.11495](https://arxiv.org/abs/2309.11495)
  Model drafts an answer, generates verification questions, answers them independently, then revises — a self-verification pipeline.

- **DoLa: Decoding by Contrasting Layers Improves Factuality in Large Language Models** ✳
  Y.-S. Chuang et al. — 2024, *ICLR 2024*
  [arXiv:2309.03883](https://arxiv.org/abs/2309.03883)
  A decoding-time method that contrasts logits from early vs. late transformer layers to surface more factual predictions, with no retrieval or fine-tuning required.

## Research Provenance / Citation-Aware Generation

- **Enabling Large Language Models to Generate Text with Citations (ALCE)**
  T. Gao, H. Yen, J. Yu, D. Chen — 2023, *EMNLP 2023*, pp. 6465–6488
  [DOI: 10.18653/v1/2023.emnlp-main.398](https://doi.org/10.18653/v1/2023.emnlp-main.398)
  Benchmark and framework evaluating LLM-generated citations on fluency, correctness, and citation quality — not just citation presence.

- **RARR: Researching and Revising What Language Models Say, Using Language Models**
  L. Gao, Z. Dai, P. Pasupat, A. Chen, A. T. Chaganty, Y. Fan, V. Y. Zhao, N. Lao, H. Lee, D.-C. Juan, K. Guu — 2023, *ACL 2023*, pp. 16477–16508
  [DOI: 10.18653/v1/2023.acl-long.910](https://doi.org/10.18653/v1/2023.acl-long.910)
  Post-generation research-and-revision system that finds attribution for existing claims and revises unsupported content.

## Retrieval-Augmented Generation and Grounding

- **RAGTruth: A Hallucination Corpus for Developing Trustworthy Retrieval-Augmented Language Models**
  C. Niu, Y. Wu, J. Zhu, S. Xu, K. Shum, R. Zhong, J. Song, T. Zhang — 2024, *ACL 2024*, vol. 1, pp. 10862–10878
  [DOI: 10.18653/v1/2024.acl-long.585](https://doi.org/10.18653/v1/2024.acl-long.585)
  ~18,000 manually annotated RAG responses showing that retrieval augmentation does **not** eliminate hallucination.

- **Self-RAG: Learning to Retrieve, Generate, and Critique through Self-Reflection** ✳
  A. Asai, Z. Wu, Y. Wang, A. Sil, H. Hajishirzi — 2023/2024, *ICLR 2024*
  [arXiv:2310.11511](https://arxiv.org/abs/2310.11511)
  Trains a model to adaptively decide when to retrieve and to critique its own generations with reflection tokens, rather than retrieving indiscriminately.

- **FreshLLMs: Refreshing Large Language Models with Search Engine Augmentation**
  T. Vu, M. Iyyer, X. Wang, N. Constant, J. Wei, J. Wei, C. Tar, Y.-H. Sung, D. Zhou, Q. Le, T. Luong — 2024, *Findings of ACL 2024*, pp. 13697–13720
  [DOI: 10.18653/v1/2024.findings-acl.813](https://doi.org/10.18653/v1/2024.findings-acl.813)
  Introduces the FreshQA benchmark for fast-changing and false-premise questions, and shows search augmentation improves temporal accuracy.

## Multimodal Hallucination

- **Woodpecker: Hallucination Correction for Multimodal Large Language Models** ✳
  S. Yin, C. Fu, S. Zhao, T. Xu, H. Wang, D. Sui, Y. Shen, K. Li, X. Sun, E. Chen — 2023/2024, *Science China Information Sciences*, 67(12):220105
  [arXiv:2310.16045](https://arxiv.org/abs/2310.16045)
  A training-free, five-stage pipeline (concept extraction → question formulation → visual knowledge validation → claim generation → correction) for fixing hallucinated text in vision-language model outputs.

---

**Total: 20 verified papers**, covering surveys/taxonomies (4), foundational work and benchmarks (5), detection methods (5), citation-aware generation (2), RAG/grounding (3), and multimodal hallucination (1).

See [`../citation-audit/`](../citation-audit/) for the systematic 10-reference authenticity/metadata audit performed on the AI-generated source paper — all ten sampled references (including six of the works listed above) were classified **A (Verified)**, for an authenticity score of 100/100.
