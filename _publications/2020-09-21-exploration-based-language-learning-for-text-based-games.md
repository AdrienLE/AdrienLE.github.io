---
title: "Exploration Based Language Learning for Text-Based Games"
collection: publications
permalink: /publication/2020-09-29-exploration-based-language-learning-for-text-based-games
excerpt: 'This work presents an exploration and imitation-learning-based agent capable of state-of-the-art performance in playing text-based computer games using the Go-Explore exploration algorithm.'
date: 2020-09-21
venue: 'IJCAI'
paperurl: 'https://www.ijcai.org/Proceedings/2020/0207.pdf'
authors: 'Andrea Madotto, Mahdi Namazifar, Joost Huizinga, Piero Molino, <span class="me">Adrien Ecoffet</span>, Huaixiu Zheng, Alexandros Papangelis, Dian Yu, Chandra Khatri, Gokhan Tur'
---
This work presents an exploration and imitation learning-based agent capable of state-of-the art performance in playing text-based computer games. These games are of interest as they can be seen as a test bed for language understanding, problem-solving, and language generation by artificial agents. Moreover, they provide a learning setting in which these skills can be acquired through interactions with an environment rather than using fixed corpora. One aspect that makes these games particularly challenging for learning agents is the combinatorially large action space. Existing methods for solving text-based games are limited to games that are either very simple or have an action space restricted to a predetermined set of admissible actions. In this work, we propose to use the exploration approach of Go-Explore \[Ecoffet et al., 2019\] for solving text-based games. More specifically, in an initial exploration phase, we first extract trajectories with high rewards, after which we train a policy to solve the game by imitating these trajectories. Our experiments show that this approach outperforms existing solutions in solving text-based games, and it is more sample efficient in terms of number of interactions with the environment. Moreover, we show that the learned policy can generalize better than existing solutions to unseen games without using any restriction on the action space.

[Download paper here](https://www.ijcai.org/Proceedings/2020/0207.pdf)

You can cite this work using the BibTeX from [IJCAI](https://www.ijcai.org/Proceedings/2020/207), which should be as follows:
```
@inproceedings{ijcai2020-207,
  title     = {Exploration Based Language Learning for Text-Based Games},
  author    = {Madotto, Andrea and Namazifar, Mahdi and Huizinga, Joost and Molino, Piero and Ecoffet, Adrien and Zheng, Huaixiu and Papangelis, Alexandros and Yu, Dian and Khatri, Chandra and Tur, Gokhan},
  booktitle = {Proceedings of the Twenty-Ninth International Joint Conference on
               Artificial Intelligence, {IJCAI-20}},
  publisher = {International Joint Conferences on Artificial Intelligence Organization},             
  editor    = {Christian Bessiere},	
  pages     = {1488--1494},
  year      = {2020},
  month     = {7},
  note      = {Main track}
  doi       = {10.24963/ijcai.2020/207},
  url       = {https://doi.org/10.24963/ijcai.2020/207},
}
```