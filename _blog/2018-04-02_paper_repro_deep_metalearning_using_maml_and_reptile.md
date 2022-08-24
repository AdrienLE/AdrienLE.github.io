---
title: "Paper repro: Deep Metalearning using “MAML” and “Reptile”"
collection: blog
permalink: /blog/2018-04-02_paper_repro_deep_metalearning_using_maml_and_reptile
excerpt: "In this post I reproduce two papers in the field of metalearning: MAML and the similar Reptile."
date: 2018-04-02
paperurl: 'https://medium.com/towards-data-science/paper-repro-deep-metalearning-using-maml-and-reptile-fd1df1cc81b0'
authors: '<span class="me">Adrien Ecoffet</span>'
---
In this post I reproduce two papers in the field of metalearning: MAML and the similar Reptile. 

The goal of both of these papers is to solve the K-shot learning problem. In K-shot learning, we need to train a neural network to generalize based on a very small number of examples (often on the order of 10 or so) instead of the often thousands of examples we see in datasets like ImageNet.

The metalearning approach of both Reptile and MAML is to come up with an initialization for neural networks that is easily generalizable to similar tasks. This is different to “Learning to Learn by Gradient Descent by Gradient Descent” in which we weren’t learning an initialization but rather an optimizer.


[View full post here](https://medium.com/towards-data-science/paper-repro-deep-metalearning-using-maml-and-reptile-fd1df1cc81b0)

In the event you would want to cite this blog post, you could use this template:
```
@electronic{ecoffet2018paper_repro_deep_metalearning_using_maml_and_reptile,
  title={Paper repro: Deep Metalearning using “MAML” and “Reptile”},
  author={Ecoffet, Adrien},
  url = {https://medium.com/towards-data-science/paper-repro-deep-metalearning-using-maml-and-reptile-fd1df1cc81b0},
  year={2018}
}
```