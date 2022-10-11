Projects from the course SF2955 Computer-intensive Methods for Mathematical Statistics @KTH, 2021

# Project 1: "Sequential Monte Carlo-based mobility tracking in cellular networks"

In this project, we needed to track a target (whose movement is described by a Markov-chain, c.f. HA1) via RSSI (*received signal
strength indication*) measurements from stations of a cellular network. Think of it this way: You want to track the movements of a Tesla, but there's massive fog, and the only data you have are the RSSI measurements that the car is measuring from the network.

# Exercises:

1. Convince oneself that 
$$\{\left(\tilde{\mathbf{X}_{n}}, \mathbf{Y}_{n}\right)\}_{n \in \mathbb{N}}$$
forms a hidden Markov model, where $\tilde{\mathbf{X}_{n}}$ is the hidden state that governs the dynamics of the target, and $\mathbf{Y}_{n}$ are the RSSI measurements.

2. Estimate the expected positions of the target using Sequential Monte Carlo methods:
  1. Sequential Importance Sampling (SIS): this leads to *sample degeneracy*
  2. Sequential Importance Resampling (SIR): before mutation, resample the particles according to their normlized weights.

3. Perform approximate maximum-likelihood estimation of the variance of the Gaussian noise from a different set of RSSI data.
