# Paper 3 — collaborating models adaptation

**Citation:** Peng Chen and Bang Wang, “On Collaborating Small and Large Models For Few-shot Intent Detection,” Findings of EMNLP 2025, 13937–13953.

**Original paper:** https://aclanthology.org/2025.findings-emnlp.749/
**Notebook:** [GitHub](paper_3_collaborating_models_adaptation.ipynb) · [Colab](https://colab.research.google.com/github/varunallagh21022002/ai-ml-paper-evidence/blob/main/paper-3-collaborating-models/paper_3_collaborating_models_adaptation.ipynb)

## Status
**Preliminary concept demonstration — unexecuted and not a paper implementation.** The notebook contains an unexecuted Colab path with a few-shot small classifier and `google/flan-t5-small` as an explicit LLM refinement step. The old concept-demo `results.json` is intentionally omitted because it is unrelated to this notebook path. No verified results are published for this paper.

## Reproduction
Run all cells in Colab. It downloads public Banking77 files, trains the small candidate model, routes low-confidence cases to the public instruction LLM, and should be extended with held-out metrics before saving verified outputs.

## Substitutions and limits
The Colab path still omits the paper’s self-supervised LLM augmentation, multi-round reasoning, enriched intent descriptions, and OOS detection. It does not claim the paper’s BANKING77, CLINC150, or HWU64 results.
