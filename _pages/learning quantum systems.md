---
title: "Quantum Photonics Laboratory - Learning Quantum Systems"
layout: textlay
excerpt: "Quantum Photonics Laboratory -- Learning Quantum Systems"
sitemap: false
permalink: /research/learning-quantum-systems/
---

# Learning Quantum Systems
### Introduction

The development of efficient techniques for the characterization of quantum systems is crucial for the development of quantum technologies for communication, computing, sensing and simulation. As the complexity of quantum states and dynamics increases exponentially with their size, however, their full description becomes intractable and even approximations are often challenging.
Our group, in collaboration with thereotical quantum physicists ([Erik Gauger](https://qtt.eps.hw.ac.uk/)) and experts in statistical learning ([Yoann Altmann](https://yoannaltmann.weebly.com/)), develops novel automated tools to characterise quantum systems, learning the processes (and the associated rates) governing their dynamics. We are particularly interested in artificial intelligence methods that can ‘advise’ experimentalists on the optimal experiments to gain information on a system, for example to distinguish between alternative models that might explain the same datasets. The toolbox we develop is then applied in Quantum Sensing experiments. For a general overview of this research field, you can read our review on “[Learning Quantum Systems](https://www.nature.com/articles/s42254-022-00552-1)” (Nature Reviews Physics, 2023 – also available on arXiv).

**Learning models for unknown quantum systems.** We develop algorithms, utilising a variety of statistical tools such as Bayesian inference, neural networks, graybox models, to automate the extraction of physical models from experimental data in a reliable, robust, and interpretable form. This is an important challenge for both fundamental scientific discoveries and technological applications, for example to propose explanations for experimental data and suggest alternative interpretations that researchers may have not have originally envisioned. We apply these algorithms to a variety of physical systems, ranging from quantum optics to superconducting circuits.

![]({{ site.url }}{{ site.baseurl }}/images/researchpic/learning_models_for_quantum_system.png){: style="width: 75%; display: block; margin: 0 auto;"}


**Optimising quantum experiments and quantum sensors.** One of the main bottlenecks for quantum sensors, particularly those based on single particles, is the data acquisition time. A specific example are the long dynamical decoupling sequences, with high spectral selectivity, required to identify nuclear spins with a single electron spin quantum sensor ([nanoscale magnetic resonance](https://iopscience.iop.org/article/10.1088/1361-6528/ad4b23)), which require weeks of integration time!
Our solution is to add **self-optimisation** capabilities to our sensor, developing sequential Bayesian experiment design algorithms that enable optimising measurement settings in real-time based on previous outcomes. The settings are updated using simple heuristics or, in more complex multi-parameter cases, by policies developed through model-aware reinforcement learning. We implement these protocols using real-time microcontrollers, FPGAs and programmable arbitrary waveform generators (see MJ Arshad et al, Physical Review Applied (2024) for a description of our adaptive quantum sensing setup).
In addition, we are developing automated learning algorithms to extract information from the environment. This is particularly important in nanoscale magnetic resonance, where the single-electron sensor detects simultaneously signals from multiple individual nuclear spins that need to be isolated and identified. This research is carried out in collaboration with the groups of Erik Gauger (quantum theory) and Yoann Altmann (applied statistics).


![]({{ site.url }}{{ site.baseurl }}/images/researchpic/learning_models_for_quantum_system_2.png){: style="width: 50%; display: block; margin: 0 auto;"}


For more information on this work, please contact  Prof Cristian Bonato ([c.bonato'at'hw.ac.uk](mailto:c.bonato'at'hw.ac.uk))


