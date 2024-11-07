# MultiHarmonic-NoiseDrowning-Qubits
Implementation of Multi-Harmonic Controlled Noise Drowning with Subharmonic Driving (MHCND-SD) to enhance qubit stability using Qiskit.

## Overview
This repository demonstrates the Multi-Harmonic Controlled Noise Drowning with Subharmonic Driving (MHCND-SD) methodology for enhancing qubit stability in quantum computing, implemented in Qiskit.

MHCND-SD combines controlled noise drowning with subharmonic driving frequencies to mitigate high-frequency environmental noise, thereby extending qubit coherence times. This approach offers a scalable, energy-efficient alternative to traditional quantum error correction methods.

## Project Contents
- **notebooks/**: Contains Jupyter Notebooks with code implementing the MHCND-SD approach in Qiskit.
- **paper/**: Holds the original research paper for this project, titled "Multi-Harmonic Subharmonic Driving and Controlled Noise Drowning for Enhanced Qubit Stability."
- **images/**: Contains visualizations, including the plot of state probabilities over time under MHCND-SD.

## Abstract
The MHCND-SD method enhances qubit coherence by introducing controlled noise and multi-harmonic subharmonic driving. This approach reduces sensitivity to environmental noise and provides a robust buffer against decoherence. Simulations in Qiskit validate the MHCND-SD approach, showing its potential to enhance qubit stability.

## Simulation Code Example
The following example initializes qubit frequencies and sets up subharmonic driving frequencies as used in the MHCND-SD methodology:

```python
# Initialize qubit frequencies and subharmonic driving frequencies
omega_q1 = 2 * np.pi * 5.0  # Qubit 1 frequency (5 GHz)
omega_d1 = omega_q1 / 2     # First harmonic (1/2) for both qubits
omega_d2 = omega_q1 / 3     # Second harmonic (1/3)
omega_d3 = omega_q1 / 4     # Third harmonic (1/4)

# Amplitudes for each harmonic
A_d1 = 0.05 * omega_q1      # Amplitude for first harmonic
A_d2 = 0.05 * omega_q1      # Amplitude for second harmonic
A_d3 = 0.05 * omega_q1      # Amplitude for third harmonic
```

## Results
The plot below shows the state probabilities over time under the MHCND-SD protocol with stochastic noise:

![image|500](https://github.com/user-attachments/assets/52c716ee-ef1c-477d-88fb-50c578f05e6f)
<span style="color: white;">*Figure 1: State probabilities of the 2-qubit system simulated over 500 ns under MHCND-SD protocol with stochastic noise.*</span>

## References
1. S. E. Nigg, H. Paik, B. Vlastakis, G. Kirchmair, S. Shankar, L. Frunzio, M. H. Devoret, and R. J. Schoelkopf, "Fast superconducting qubit control with sub-harmonic drives," *arXiv preprint arXiv:2306.10162*, 2023. [Online]. Available: https://arxiv.org/abs/2306.10162

2. J. Schirk, M. Singh, L. Södergren, E. Dionis, D. Sugny, M. Werninghaus, K. Liegener, C. M. F. Schneider, and S. Filipp, "Protected Fluxonium Control with Sub-harmonic Parametric Driving," *arXiv preprint arXiv:2410.00495*, 2024. [Online]. Available: https://arxiv.org/abs/2410.00495

3. J. P. Santos, L. C. Céleri, G. T. Landi, and M. Paternostro, "Reservoir engineering for maximally efficient quantum engines," *Phys. Rev. Res.*, vol. 2, p. 043419, 2020. [Online]. Available: https://link.aps.org/doi/10.1103/PhysRevResearch.2.043419

4. K. Fujii and K. Nakajima, "Quantum reservoir computing: a reservoir approach toward quantum machine learning on near-term quantum devices," *arXiv preprint arXiv:2011.04890*, 2020. [Online]. Available: https://arxiv.org/abs/2011.04890

5. T. O. MacLean, T. F. O'Brien, P. S. Żuchowski, and D. Jaksch, "Quantum Reservoir Computing Using Arrays of Rydberg Atoms," *PRX Quantum*, vol. 3, p. 030325, 2022. [Online]. Available: https://link.aps.org/doi/10.1103/PRXQuantum.3.030325

## Contact
For any questions, please reach out to [Your Contact Info].
