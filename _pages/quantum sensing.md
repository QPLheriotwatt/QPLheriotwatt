---
title: "Quantum Photonics Laboratory - Quantum Sensing"
layout: textlay
excerpt: "Quantum Photonics Laboratory -- Quantum Sensing"
sitemap: false
permalink: research//quantum-sensing/
---

# Quantum Sensing
### Introduction
We utilise single electron spins associated to a defect in diamond, the nitrogen-vacancy (NV) centre, as a tiny nanoscale quantum sensor, and apply it to investigate interesting problems in condensed matter physics and biology. We operate and manage the Heriot-Watt’s “Nanoscale quantum sensing facility” (link to the page), hosting the world’s first commercial low-temperature scanning quantum sensor, and we deploy it to study magnetism, spin waves, superconductivity in 2D van der Waals materials and their heterostructures. As part of the UK “[Quantum sensing hub for biomedical research](https://www.qbiomed.org/)”, we deploy spin-based quantum sensors to detect small quantities of molecules relevant for health-care, with the goal of enabling novel biomedical research tools and early disease detection. The operator of our quantum sensors is enhanced by AI and machine learning techniques, which make their operation fast, automated and robust, as required by deployment in different fields.

![]({{ site.url }}{{ site.baseurl }}/images/slider/scanningtip.png){: style="width: 50%; display: block; margin: 0 auto;"}

**Real-time adaptive optimisation and machine learning.** One of the main bottlenecks for NV magnetometry is the data acquisition time: especially for long dynamical decoupling sequences with high spectral selectivity, required in nanoscale magnetic resonance, the signal acquisition timescales become prohibitively long. Our solution is to add **self-optimisation** capabilities to our sensor, developing Bayesian algorithms that enable optimising measurement settings in real-time based on previous outcomes. The settings are updated using simple heuristics or, in more complex multi-parameter cases, by policies developed through model-aware reinforcement learning. We implement these type of protocols using real-time microcontrollers, FPGAs and programmable arbitrary waveform generators (see MJ Arshad et al, Physical Review Applied (2024) for a description of our adaptive quantum sensing setup).
In addition, we are developing automated learning algorithms to extract information from the environment. This is particularly important in nanoscale magnetic resonance, where the single-electron sensor detects simultaneously signals from multiple individual nuclear spins that need to be isolated and identified. This research is carried out in collaboration with the groups of Erik Gauger (quantum theory) and Yoann Altmann (applied statistics).

![]({{ site.url }}{{ site.baseurl }}/images/researchpic/learning_models_for_quantum_system_2.png){: style="width: 60%; display: block; margin: 0 auto;"}


**Quantum sensing of complex quantum materials.** One of our major efforts is to directly image currents and magnetic fields geerated by spin and charge transport in quantum materials. Doing so enables a unique window into the world of condensed matter physics in which collective electron and spin excitations are both fundementally intersting and technologically applicable. For example, many quantum materials derive their properties from reduction of dimensionality, which has shown electron confinement and increased interactions in two dimensions. Such discoveries at the interface of semiconductors has enabled high-mobility field effect transistors.
Our research focuses on exploring coupling spin/magnetic order in novel magnetic thin films and ‘van der Waals’ heterostructures including magnetic textures, spin waves, and Moiré superlattices. To do we we have recently set-up a [Nanoscale Quantum Sensing facility]({{ site.url }}{{ site.baseurl }}/facilities/nanoscale_quantum_sensing), including the first commercial scanning spin-based quantum sensor operating between 1.8-300K.


**Quantum sensing in bio-chemistry.** We are very interested in applying spin-based quantum sensing to study interesting processes in surface chemistry and biology. If interested, you can for example read the Roadmap on Nanoscale Magnetic Resonance Imaging we co-authored with other leading international groups in this exciting field. We are working on this topic as part of the newly-established “UK Quantum Hub for Biomedicla Research” (Q-BIOMED). Stay tuned for more information about this work!

Our quantum sensing activities are highlighted below:

**Quantum for Healthcare**
Link to the corresponding page

**Quantum Learning Systems** - [Link]({{ site.url }}{{ site.baseurl }}/research/quantum-learning)

**2D Materials** - [Link]({{ site.url }}{{ site.baseurl }}/research/quantum-materials)



