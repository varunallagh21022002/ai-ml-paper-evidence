# Paper 4 — DDAIR adaptation

**Citation:** Galo Castillo-López, Alexis Lombard, Nasredine Semmar, and Gaël de Chalendar, “How DDAIR you? Disambiguated Data Augmentation for Intent Recognition,” EACL 2026 Short Papers, 274–286. Official record: https://aclanthology.org/2026.eacl-short.20/.

**Original paper:** https://aclanthology.org/2026.eacl-short.20/
**Notebook:** [GitHub](paper_4_ddair_adaptation.ipynb) · [Colab](https://colab.research.google.com/github/varunallagh21022002/ai-ml-paper-evidence/blob/main/paper-4-ddair/paper_4_ddair_adaptation.ipynb)

## Status
**Executed locally with saved `results.json`, but not a reproduction.** It creates deterministic lexical substitutions and retains augmented utterances only when their TF-IDF similarity to the source class centroid exceeds the strongest competing centroid by a fixed margin.

## Reproduction
Run all cells in Colab. The notebook downloads public Banking77 files and writes the split, threshold, kept augmentation count, and held-out metrics.

## Substitutions and limits
This is not the DDAIR sentence-embedding/regeneration pipeline. It substitutes hand-coded lexical replacements and TF-IDF centroid-margin filtering for DDAIR's embedding comparison and regeneration process, and does not reproduce its datasets, ambiguity analyses, or results.
