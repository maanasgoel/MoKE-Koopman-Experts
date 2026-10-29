# MoKE: A Mixture of Koopman Experts for Nonlinear Dynamical Systems

Koopman operator theory gives a linear view of nonlinear dynamics, but a single global operator struggles with systems that have several equilibria and switch between regimes. MoKE learns a set of local Koopman operators, one per regime, and a gating network that blends them for smooth transitions.

## Evaluation

Tested on the Duffing oscillator, Van der Pol oscillator, Lorenz attractor, and double pendulum against VAR, extended DMD, and single-operator Koopman autoencoders. With 3 to 4 experts, MoKE had the best accuracy within the training horizon and never diverged on long rollouts of 500 to 1,000 steps, while eDMD diverged on 15 to 16% of Duffing and double-pendulum trajectories.

## Paper and code

- Paper: [MoKE_Paper.pdf](MoKE_Paper.pdf)
- Code: [pujiacheng/ESE5380_MoKE-on-non-linear-dynamical-system](https://github.com/pujiacheng/ESE5380_MoKE-on-non-linear-dynamical-system)
