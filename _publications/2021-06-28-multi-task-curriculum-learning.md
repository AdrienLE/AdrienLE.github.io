---
title: "Multi-task curriculum learning in a complex, visual, hard-exploration domain: Minecraft"
collection: publications
permalink: /publication/2021-06-28-multi-task-curriculum-learning
excerpt: 'An important challenge in reinforcement learning is training agents that can solve a wide variety of tasks. If tasks depend on each other (e.g. needing to learn to walk before learning to run), curriculum learning can speed up learning by focusing on the next best task to learn. We explore curriculum learning in a complex, visual domain with many hard exploration challenges: Minecraft.'
date: 2021-06-28
venue: 'arXiv'
paperurl: 'https://arxiv.org/pdf/2106.14876.pdf'
authors: 'Ingmar Kanitscheider, Joost Huizinga, David Farhi, William Hebgen Guss, Brandon Houghton, Raul Sampedro, Peter Zhokhov, Bowen Baker, <span class="me">Adrien Ecoffet</span>, Jie Tang, Oleg Klimov, Jeff Clune'
---
An important challenge in reinforcement learning is training agents that can solve a wide variety of tasks. If tasks depend on each other (e.g. needing to learn to walk before learning to run), curriculum learning can speed up learning by focusing on the next best task to learn. We explore curriculum learning in a complex, visual domain with many hard exploration challenges: Minecraft. We find that learning progress (defined as a change in success probability of a task) is a reliable measure of learnability for automatically constructing an effective curriculum. We introduce a learning-progress based curriculum and test it on a complex reinforcement learning problem (called "Simon Says") where an agent is instructed to obtain a desired goal item. Many of the required skills depend on each other. Experiments demonstrate that: (1) a within-episode exploration bonus for obtaining new items improves performance, (2) dynamically adjusting this bonus across training such that it only applies to items the agent cannot reliably obtain yet further increases performance, (3) the learning-progress based curriculum elegantly follows the learning curve of the agent, and (4) when the learning-progress based curriculum is combined with the dynamic exploration bonus it learns much more efficiently and obtains far higher performance than uniform baselines. These results suggest that combining intra-episode and across-training exploration bonuses with learning progress creates a promising method for automated curriculum generation, which may substantially increase our ability to train more capable, generally intelligent agents.

[Download paper here](https://arxiv.org/pdf/2106.14876.pdf)

You can cite this work using the BibTeX from Google Scholar, which should be as follows:
```
@inproceedings{ecoffet2021reinforcement,
  title={Reinforcement learning under moral uncertainty},
  author={Ecoffet, Adrien and Lehman, Joel},
  booktitle={International Conference on Machine Learning},
  pages={2926--2936},
  year={2021},
  organization={PMLR}
}
```