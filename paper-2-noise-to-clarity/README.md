# Paper 2 — From Noise to Clarity adaptation

**Citation:** Junbao Huang et al., “From Noise to Clarity: Filtering Real and LLM-Generated Samples for Enhanced Intent Detection,” Findings of EMNLP 2025, 21736–21746.

**Original paper:** https://aclanthology.org/2025.findings-emnlp.1186/
**Notebook:** [GitHub](paper_2_noise_to_clarity_adaptation.ipynb) · [Colab](https://colab.research.google.com/github/varunallagh21022002/ai-ml-paper-evidence/blob/main/paper-2-noise-to-clarity/paper_2_noise_to_clarity_adaptation.ipynb)

## Status
**Executed locally with saved `results.json`, but not a reproduction.** It uses a compact 10-class Banking77 subset and substitutes deterministic corrupted utterances for LLM-generated samples by deleting a word and vowel. A TF-IDF similarity-to-class-centroid score substitutes for the paper's filtering machinery before training.

## Reproduction
Run all cells in Colab. The notebook downloads the public Banking77 train/test CSV files and writes the actual metrics and filtering threshold to `results.json`.

## Substitutions and limits
This does not reproduce the paper's LLM-generated data, topic modeling, quality labels, datasets, or reported results. Synthetic corruption and centroid filtering are transparent substitutions for noisy samples and quality assessment; the official test set remains untouched.
