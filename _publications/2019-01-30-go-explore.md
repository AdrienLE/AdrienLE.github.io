---
title: "Go-explore: a new approach for hard-exploration problems"
collection: publications
permalink: /publication/2019-01-30-go-explore
excerpt: 'Introduces Go-Explore, an exploration algorithm capable of solving the grand-challenge hard-exploration Atari games Montezuma′s Revenge and Pitfall.'
date: 2019-01-30
venue: 'arXiv'
paperurl: 'https://arxiv.org/pdf/1901.10995.pdf'
authors: '<span class="me">Adrien Ecoffet</span>, Joost Huizinga, Joel Lehman, Kenneth O. Stanley, Jeff Clune'
---
A grand challenge in reinforcement learning is intelligent exploration, especially when rewards are sparse or deceptive. Two Atari games serve as benchmarks for such hard-exploration domains: Montezuma's Revenge and Pitfall. On both games, current RL algorithms perform poorly, even those with intrinsic motivation, which is the dominant method to improve performance on hard-exploration domains. To address this shortfall, we introduce a new algorithm called Go-Explore. It exploits the following principles: (1) remember previously visited states, (2) first return to a promising state (without exploration), then explore from it, and (3) solve simulated environments through any available means (including by introducing determinism), then robustify via imitation learning. The combined effect of these principles is a dramatic performance improvement on hard-exploration problems. On Montezuma's Revenge, Go-Explore scores a mean of over 43k points, almost 4 times the previous state of the art. Go-Explore can also harness human-provided domain knowledge and, when augmented with it, scores a mean of over 650k points on Montezuma's Revenge. Its max performance of nearly 18 million surpasses the human world record, meeting even the strictest definition of "superhuman" performance. On Pitfall, Go-Explore with domain knowledge is the first algorithm to score above zero. Its mean score of almost 60k points exceeds expert human performance. Because Go-Explore produces high-performing demonstrations automatically and cheaply, it also outperforms imitation learning work where humans provide solution demonstrations. Go-Explore opens up many new research directions into improving it and weaving its insights into current RL algorithms. It may also enable progress on previously unsolvable hard-exploration problems in many domains, especially those that harness a simulator during training (e.g. robotics).

[Download paper here](https://arxiv.org/pdf/1901.10995.pdf)

If you wish to cite the Go-Explore algorithm in general as opposed to something specific mentioned in this particular version, you should probably cite [First return then explore](publications/2020-05-14-first-return-then-explore) instead. If you really wish to cite this version, you can use the BibTeX from Google Scholar, which should be as follows:
```
@article{ecoffet2019go,
  title={Go-explore: a new approach for hard-exploration problems},
  author={Ecoffet, Adrien and Huizinga, Joost and Lehman, Joel and Stanley, Kenneth O and Clune, Jeff},
  journal={arXiv preprint arXiv:1901.10995},
  year={2019}
}
```