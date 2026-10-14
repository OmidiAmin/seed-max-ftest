This is a simple demo of Successive Empirical Excess risk Difference MAXimization (SEED-MAX)
and SEED-MAX-F-test methods for pruning random convolutional features of MINIROCKET method.

Please cite this code as

`
@article{seedmax2025random,
  author = {Omidi, Mohammad Amin and Seyfe, Babak and Valaee, Shahrokh},
  title  = {Random Feature Pruning for Multi-Class Classification},
  journal={arXiv preprint},
  year={2026},
  url = {https://arxiv.org/abs/2610.15101}
}
`


---

**🚀 Demo Code: Random Feature Pruning for Multi-Class Time-Series Classification**

Training accurate classifiers on time-series datasets with *limited labeled samples* remains a fundamental challenge—particularly for data-hungry deep learning models. In low-sample regimes, DL architectures often fail to learn sufficiently informative representations.

A highly effective alternative is to **generate a large pool of random convolutional features** and train a **regularized linear classifier** on top of them. This paradigm—exemplified by ROCKET and MiniROCKET—has consistently achieved *state-of-the-art accuracy* on diverse time-series benchmarks.

However, most of these randomly generated features are **highly redundant**.

🔍 **Our contribution:**
We introduce a *highly efficient feature pruning pipeline* that **automatically removes over 90% of redundant random features**, while *almost entirely preserving classification accuracy*—and significantly accelerating inference.

### 🧠 SEED-MAX-F-Test in a nutshell:

1. Pre-train a linear classifier on all random features
2. Rank features by their regression weights
3. Detect a **change point** in the weight spectrum
4. Prune low-impact features beyond the change point
5. Apply an **F-test** for further statistical refinement

The result: **faster models, fewer features, same accuracy.**

📌 Code available here:
[https://github.com/OmidiAmin/seed-max-ftest](https://github.com/OmidiAmin/seed-max-ftest)

👉 If you work on time-series learning, feature engineering, or efficient ML pipelines—this is for you.

