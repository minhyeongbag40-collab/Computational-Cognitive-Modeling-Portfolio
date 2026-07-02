Bayesian Models of Cognition


# Bayesian Observer Model

## Research Question

How do prior beliefs and sensory uncertainty influence binary perceptual decisions?

## Overview

This project implements a simple Bayesian observer model for binary categorization.
The observer receives noisy sensory evidence and combines it with prior beliefs to
infer the most likely latent category.

The project investigates how changes in sensory noise, category separation, and
prior probability affect posterior beliefs and decision boundaries.

## Model

Let C denote a latent category and x denote noisy sensory evidence.

C ~ Bernoulli(pi)

x | C = 0 ~ Normal(mu_0, sigma^2)

x | C = 1 ~ Normal(mu_1, sigma^2)

The posterior probability is computed using Bayes' rule:

P(C | x) ∝ P(x | C)P(C)

## Current Progress

- [ ] Implement the generative model
- [ ] Compute posterior probabilities
- [ ] Visualize likelihoods and decision boundaries
- [ ] Analyze the effects of prior probability
- [ ] Analyze the effects of sensory noise
- [ ] Perform parameter recovery
- [ ] Compare with a non-Bayesian baseline model

## Tools

- Python
- NumPy
- SciPy
- Matplotlib
- Jupyter Notebook
