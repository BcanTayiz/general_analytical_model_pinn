# Taylor-Embedded Symbolic Physics-Informed Neural Networks (TES-PINNs)

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Python 3.10+](https://img.shields.io/badge/python-3.10%252B-blue.svg)](https://www.python.org/)
[![PyTorch](https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?style=flat&to=PyTorch&logo=PyTorch&logoColor=white)](https://pytorch.org/)

Official repository for the research paper: **"Taylor-Embedded Symbolic Physics-Informed Neural Networks (TES-PINNs): Drift-Free Discovery of Interpretable Dynamical Systems"**.

---

## Overview

Physics-Informed Neural Networks (PINNs) provide a powerful framework for modeling physical systems, but traditional architectures suffer from:
1. **Spectral bias** (difficulty in capturing high-frequency dynamics).
2. **Cumulative rollout drift** over long temporal horizons.
3. **Black-box opacity** lacking scientific interpretability.

**TES-PINNs** resolve these bottlenecks by integrating:
- **Randomized Fourier Feature Mappings** to overcome spectral bias.
- **Recursive Higher-Order Taylor Integration** to stabilize long-term trajectories and eliminate drift.
- **Direct Symbolic Translation & SINDy Filtering** to extract parsimonious, closed-form ordinary differential equations (ODEs) via SymPy.

---

## Repository Structure

```text
├── LICENSE.txt
├── README.md
├── method/
│   ├── code.ipynb
│   ├── article/
│   │   ├── article.pdf
├── tutorial/
│   ├── intro.ipynb
│   ├── polynomial-augmented neural networks.ipynb
│   ├── taylor_exp.ipynb
```