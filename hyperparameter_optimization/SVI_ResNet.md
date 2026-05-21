# Optimal hyperparameters for ResNet-18 SVI-BNN training

| Hyperparameter | Dirty-MNIST | CIFAR-10 | CINIC-10 |
|---|---:|---:|---:|
| Optimizer | Adam | Adam | Adam |
| Max KL factor ($\alpha_{\text{max}}$) | $1.69 \times 10^{-4}$ | $7.007 \times 10^{-4}$ | $8.38 \times 10^{-5}$ |
| Learning rate | $1.13 \times 10^{-3}$ | $2.883 \times 10^{-4}$ | $6.73 \times 10^{-5}$ |
| Epochs (SVI / deterministic pre-training) | 50 / 0 | 50 / 400 | 50 / 400 |
| **Gaussian prior parameters:** |  |  |  |
| σ (first layer) | 0.0078 | 0.0536 | 0.1677 |
| σ (last layer) | 0.0124 | 0.9096 | 0.0607 |
| σ (intermediate layers) | 1.918 | 0.6533 | 0.2284 |
| μ (all layers) | 0.0 | 0.0 | 0.0 |
| Posterior initial σ | $5.45 \times 10^{-6}$ | $7.85 \times 10^{-6}$ | $3.04 \times 10^{-6}$ |
| Posterior initial μ | 0.016 (uniform distribution) | pre-trained | pre-trained |
