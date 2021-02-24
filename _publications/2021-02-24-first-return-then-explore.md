---
title: "First return, then explore"
collection: publications
permalink: /publication/2021-02-24-first-return-then-explore
excerpt: 'The definite version of the Go-Explore algorithm. On top of the results from the original pre-print, it introduces a dynamic representation that supports all Atari games, a variant in which the exploration phase can be performed in stochastic environments, and demonstrates Go-Explore working in a robotics environment.'
date: 2021-02-24
venue: 'Nature'
paperurl: 'https://www.nature.com/articles/s41586-020-03157-9.epdf?sharing_token=fVSAoXFGOipXiv03jaRGFtRgN0jAjWel9jnR3ZoTv0M2nmoar2g6_K5n8IBFPE90s2PCF4tYuP4UnEffP83tohRanjcxryz9Usln4Rw7idY6ufIsQYVgwwD0B8UgE7JYzmgOuMdgNqvVMg7GsfFiI2ZBi9PjjmJtJGEDwzRPFWc%3D'
authors: '<span class="me">Adrien Ecoffet</span>, Joost Huizinga, Joel Lehman, Kenneth O. Stanley, Jeff Clune'
---
Reinforcement learning promises to solve complex sequential-decision problems autonomously by specifying a high-level reward function only. However, reinforcement learning algorithms struggle when, as is often the case, simple and intuitive rewards provide sparse1 and deceptive2 feedback. Avoiding these pitfalls requires a thorough exploration of the environment, but creating algorithms that can do so remains one of the central challenges of the field. Here we hypothesize that the main impediment to effective exploration originates from algorithms forgetting how to reach previously visited states (detachment) and failing to first return to a state before exploring from it (derailment). We introduce Go-Explore, a family of algorithms that addresses these two challenges directly through the simple principles of explicitly ‘remembering’ promising states and returning to such states before intentionally exploring. Go-Explore solves all previously unsolved Atari games and surpasses the state of the art on all hard-exploration games1, with orders-of-magnitude improvements on the grand challenges of Montezuma’s Revenge and Pitfall. We also demonstrate the practical potential of Go-Explore on a sparse-reward pick-and-place robotics task. Additionally, we show that adding a goal-conditioned policy can further improve Go-Explore’s exploration efficiency and enable it to handle stochasticity throughout training. The substantial performance gains from Go-Explore suggest that the simple principles of remembering states, returning to them, and exploring from them are a powerful and general approach to exploration—an insight that may prove critical to the creation of truly intelligent learning agents.

[Link to paper here](https://www.nature.com/articles/s41586-020-03157-9.epdf?sharing_token=fVSAoXFGOipXiv03jaRGFtRgN0jAjWel9jnR3ZoTv0M2nmoar2g6_K5n8IBFPE90s2PCF4tYuP4UnEffP83tohRanjcxryz9Usln4Rw7idY6ufIsQYVgwwD0B8UgE7JYzmgOuMdgNqvVMg7GsfFiI2ZBi9PjjmJtJGEDwzRPFWc%3D)

You can cite this work using the following BibTeX:
```
@Article{Ecoffet2021,
  author={Ecoffet, Adrien and Huizinga, Joost and Lehman, Joel and Stanley, Kenneth O. and Clune, Jeff},
  title={First return, then explore},
  journal={Nature},
  year={2021},
  month={Feb},
  day={01},
  volume={590},
  number={7847},
  pages={580-586},
  issn={1476-4687},
  doi={10.1038/s41586-020-03157-9},
  url={https://doi.org/10.1038/s41586-020-03157-9}
}
```