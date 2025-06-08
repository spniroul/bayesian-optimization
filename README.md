# Bayesian Optimization: A Gentle Introduction with Applications

This project provides an accessible yet mathematically grounded introduction to **Bayesian Optimization (BO)**—a powerful method for optimizing expensive black-box functions. The project culminates in a hands-on application: tuning hyperparameters of a neural network on the MNIST dataset using the `bayes_opt` Python library.

## 📌 Project Overview

Bayesian Optimization is particularly useful in scenarios where the objective function is expensive to evaluate or lacks derivatives. It works by building a probabilistic surrogate model (e.g., Gaussian Process) and selecting promising evaluation points through acquisition functions that balance **exploration** and **exploitation**.

This project explores:
- Theoretical foundations of Bayesian Optimization
- Gaussian Process regression and kernel selection
- Acquisition functions (Expected Improvement)
- Application to neural network hyperparameter tuning

## 🧠 Key Concepts

- **Surrogate Modeling:** Use of Gaussian Processes (GPs) to model the objective function and quantify uncertainty.
- **Acquisition Functions:** Heuristics like Expected Improvement to decide where to sample next.
- **Exploration vs. Exploitation:** Strategic trade-off for efficient convergence.

## 🔧 Implementation

We applied Bayesian Optimization to tune the following hyperparameters of an MLP classifier from `scikit-learn`:
- **Phase 1:** Learning rate and alpha (L2 regularization)
- **Phase 2:** Added hidden layer size to the tuning process

### Results

| Phase | Optimized Parameters                                     | Accuracy |
|-------|----------------------------------------------------------|----------|
| 1     | Alpha = 0.008, Learning Rate = 0.077                     | 94.6%    |
| 2     | Alpha = 0.075, Learning Rate = 0.005, Hidden Layer Size = 116 | 95.7%    |

The results show clear performance improvement through strategic hyperparameter tuning.


## 🤝 Authors and Contributions

- **Hubert Witkos** – Theoretical foundations (Gaussian Processes, Acquisition Functions)
- **Yuqian Wang** – Literature review and project introduction
- **Soujan Niroula** – Neural network tuning and Python implementation
- **Yongliang Yu** – Assisted with implementation and experiments

## 🤖 Use of AI

- Used for LaTeX formatting, Python code debugging, and synthesizing basic theoretical references.

## 📘 References

- Frazier, P.I. (2018). *A tutorial on Bayesian Optimization*. [arXiv:1807.02811](https://arxiv.org/abs/1807.02811)  
- Shahriari et al. (2016). *Taking the human out of the loop: A review of Bayesian Optimization.*  
- Snoek et al. (2012). *Practical Bayesian Optimization of Machine Learning Algorithms.*


