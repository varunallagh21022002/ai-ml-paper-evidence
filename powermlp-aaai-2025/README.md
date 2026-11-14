# PowerMLP — small-scale adaptation

**Citation:** Ruichen Qiu, Yibo Miao, Shiwen Wang, and Yifan Zhu, “PowerMLP: An Efficient Version of KAN,” *Proceedings of the AAAI Conference on Artificial Intelligence* 39(19), 20069–20076 (2025). DOI: https://doi.org/10.1609/aaai.v39i19.34210.

**Original paper:** https://doi.org/10.1609/aaai.v39i19.34210
**Notebook:** [GitHub](powermlp_adaptation.ipynb) · [Colab](https://colab.research.google.com/github/varunallagh21022002/ai-ml-paper-evidence/blob/main/powermlp-aaai-2025/powermlp_adaptation.ipynb)

## Status
**Executed locally after a gradient-correctness fix, with saved `results.json`, but not a reproduction.** The notebook implements the published adapted layer formula `z = α b(x) + ReLU_k(Wx + γ)`, with `b(x)=x/(1+e^-x)` and a final affine layer. Its forward pass uses `b(x)` and its analytic backpropagation includes the SiLU derivative; central finite differences check all parameters and inputs before training. It compares the result with a two-hidden-layer ReLU MLP on a deterministic one-dimensional regression function.

## Reproduction
Run all cells in Colab. No private data or credentials are required; the notebook generates its synthetic data and writes held-out RMSE, MAE, and fit time to `results.json`.

## Substitutions and limits
The implementation is a small NumPy adaptation of the published formula, not the authors’ full architecture, KAN implementation, theoretical analysis, or benchmark suite. The timing comparison is local and should not be generalized to the paper’s reported speed claim.
