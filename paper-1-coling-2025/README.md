# Paper 1 — COLING 2025 adaptation

**Citation:** Maia Aguirre et al., “Fine-Tuning Medium-Scale LLMs for Joint Intent Classification and Slot Filling: A Data-Efficient and Cost-Effective Solution for SMEs,” COLING Industry Track 2025, 251–262.

**Original paper:** https://aclanthology.org/2025.coling-industry.21/
**Notebook:** [GitHub](paper_1_coling_2025_adaptation.ipynb) · [Colab](https://colab.research.google.com/github/varunallagh21022002/ai-ml-paper-evidence/blob/main/paper-1-coling-2025/paper_1_coling_2025_adaptation.ipynb)

## Status
**Preliminary concept demonstration — unexecuted and not a paper implementation.** The notebook contains an unexecuted Colab path using MASSIVE, a small BERT encoder, intent and BIO slot heads, and LoRA adapters. The old concept-demo `results.json` is intentionally omitted because it is unrelated to this notebook path. No verified results are published for this paper.

## Reproduction
Open the notebook in Colab and run all cells. It installs the model dependencies, loads a small English MASSIVE split, prepares joint intent/slot labels, and defines the LoRA model path. Add and save a successful training/evaluation run before treating it as implemented.

## Limitations
The Colab path still needs a completed training loop, intent accuracy, slot entity-F1, and saved run metadata. It does not claim Llama-3-8B, the paper’s data scale, or the authors’ results.
