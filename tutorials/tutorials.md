# Tutorials and Learning Resources

## Reducing hallucination in practice

- **Anthropic — "Reduce hallucinations" (Claude Docs)**
  [docs.claude.com/en/docs/test-and-evaluate/strengthen-guardrails/reduce-hallucinations](https://docs.claude.com/en/docs/test-and-evaluate/strengthen-guardrails/reduce-hallucinations)
  Official guidance on allowing a model to express uncertainty, grounding answers in direct quotes, and citation-based verification — practical counterparts to the "epistemic reliability" dimension in this paper's taxonomy.

- **Anthropic — Claude Prompt Engineering Interactive Tutorial, Ch. 8: "Avoiding Hallucinations"**
  [github.com/anthropics/courses](https://github.com/anthropics/courses) (`prompt_engineering_interactive_tutorial/Anthropic 1P/08_Avoiding_Hallucinations.ipynb`)
  Hands-on notebook walking through evidence-gathering and temperature-control techniques for reducing hallucination on long documents.

## Citation and reference verification

- **Google Scholar** — [scholar.google.com](https://scholar.google.com/)
  General-purpose scholarly search used to check whether a cited title/author/venue combination genuinely exists.

- **Semantic Scholar** — [semanticscholar.org](https://www.semanticscholar.org/)
  AI-powered literature search with structured metadata (authors, venue, citation graph) — useful for catching "Frankenstein" citations that combine real authors/venues with a nonexistent paper.

- **Crossref** — [crossref.org](https://www.crossref.org/) (DOI lookup)
  The authoritative registry for resolving whether a supplied DOI is valid and belongs to the claimed publication — the primary tool for detecting Type E (identifier mismatch) citation errors.

- **arXiv** — [arxiv.org](https://arxiv.org/)
  Canonical source for verifying preprint IDs, publication dates, and author lists for the many arXiv-only references in this field.

These four verification sources map directly onto the audit procedure documented in [`../citation-audit/`](../citation-audit/), Part G ("Citation Authenticity and Metadata Audit").
