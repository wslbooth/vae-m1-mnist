# Semi-Supervised Learning on MNIST with a Variational Autoencoder (M1 Model)

This repository contains a clean, reproducible implementation of the M1 semi-supervised VAE model from Kingma et al. (2014), “Semi-Supervised Learning with Deep Generative Models”.
All code is written in a Google Colab notebook, and experiments are performed on the MNIST dataset.

## Project Goal

Evaluate whether a VAE used as a latent feature extractor improves classification accuracy compared to a baseline classifier.

## Current Results

Baseline classifier: ~86% max test accuracy

M1 model (VAE + classifier): ~88% max test accuracy

Improvement demonstrates that the VAE learns useful discriminative latent features

## Contents

notebooks/ — Main Colab notebook with complete implementation

Implementation of:

- Variational Autoencoder (encoder + decoder)

- Classifier trained on learned latent space

- Training loops, loss functions, KL term, and evaluation metrics

- Experiment results and plots

## References

Kingma, D. P., Rezende, D. J., Mohamed, S., & Welling, M. (2014).
Semi-Supervised Learning with Deep Generative Models.
NeurIPS 27.
https://arxiv.org/abs/1406.5298

Kingma, D. P., & Welling, M. (2014).
Auto-Encoding Variational Bayes.
arXiv:1312.6114.
https://arxiv.org/abs/1312.6114

Doersch, C. (2016).
Tutorial on Variational Autoencoders.
https://arxiv.org/abs/1606.05908

## Status

Actively being developed.

Planned additions:
- Hyperparameter sweeps
- Latent space visualization
- β-VAE experiments
- Fashion-MNIST comparison
