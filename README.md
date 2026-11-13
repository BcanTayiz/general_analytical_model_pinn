# Generalized Structure-Preserving Analytical Embedded PINNs

This repository provides a generalized framework for modeling nonlinear dynamical systems by embedding known analytical equations directly into neural network architectures while treating physical coefficients as learnable parameters. This approach bridges purely data-driven black-box models with mechanistic physics, eliminating long-term rollout drift and achieving robust extrapolation and inverse parameter discovery.

---

## 🚀 Key Features

* **Structure-Preserving Embedding**: Constrains the hypothesis space to valid physical templates rather than unconstrained function approximation.
* **Inverse Parameter Identification**: Optimizes physical coefficients (e.g., damping, stiffness, limit-cycle parameters) directly via gradient descent.
* **Multi-System Support**: Easily extensible across various nonlinear systems including the **Duffing Oscillator** and the **Van der Pol Limit-Cycle Oscillator**.
* **Rigorous Evaluation**: Implements chronological train/test splitting to validate long-term future-state extrapolation capability.

---

## 📊 Benchmark Results

| System | Training $R^2$ | Test Extrapolation $R^2$ | True Parameters | Learned Parameters |
| :--- | :---: | :---: | :--- | :--- |
| **Duffing Oscillator** | $0.9959$ | $0.9671$ | $\delta=0.2, \alpha=-1.0, \beta=1.0$ | $\delta=0.2175, \alpha=-1.0000, \beta=0.9993$ |
| **Van der Pol Oscillator** | $0.9912$ | $0.8377$ | $\mu=1.5000$ | $\mu=1.4975$ |
---

## 🛠️ Installation & Requirements

Ensure you have Python 3.8+ and PyTorch installed along with standard scientific libraries:

```bash
pip install torch numpy scipy matplotlib
```

---

## 📂 Repository Structure


There is final code and final article pdf in **method** folder \
You may find different attempts  in **tutorial** folder where I created tests or different methods\



---

## 📄 Citation

If you use this framework or code in your research, please cite our paper draft:

```bibtex
@software{analytical_embedded_pinns2026,
  title={A Generalized Structure-Preserving Analytical Embedded Framework for Nonlinear Dynamical Systems},
  author={Barış Can Tayiz},
  year={2026},
  publisher={Zenodo},
  doi={10.5281/zenodo.24182618},
  url={https://doi.org/10.5281/zenodo.24182618}
}

```