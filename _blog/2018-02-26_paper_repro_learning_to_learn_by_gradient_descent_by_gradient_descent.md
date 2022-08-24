---
title: "Paper repro: “Learning to Learn by Gradient Descent by Gradient Descent”"
collection: blog
permalink: /blog/2018-02-26_paper_repro_learning_to_learn_by_gradient_descent_by_gradient_descent
excerpt: "This is a reproduction of the metalearning paper “Learning to Learn by Gradient Descent by Gradient Descent”"
date: 2018-02-26
paperurl: 'https://medium.com/becoming-human/paper-repro-learning-to-learn-by-gradient-descent-by-gradient-descent-6e504cc1c0de'
authors: '<span class="me">Adrien Ecoffet</span>'
---
This is a reproduction of the paper “Learning to Learn by Gradient Descent by Gradient Descent”. 

Learning to learn is a very exciting topic for a host of reasons, not least of which is the fact that we know that the type of backpropagation currently done in neural networks is implausible as an mechanism that the brain is actually likely to use: there is no Adam optimizer nor automatic differentiation in the brain! Something else has to be doing the optimization of our brain’s neural network, and most likely that something else is itself a neural network!

The paper we are looking at today is thus trying to replace the optimizers normally used for neural networks (eg Adam, RMSprop, SGD etc.) by a recurrent neural network: after all, gradient descent is fundamentally a sequence of updates (from the output layer of the neural net back to the input), in between which a state must be stored. We can think of an optimizer as a mini-RNN. The idea in this paper is to actually train that RNN instead of using a generic algorithm like Adam/SGD/etc..




[View full post here](https://medium.com/becoming-human/paper-repro-learning-to-learn-by-gradient-descent-by-gradient-descent-6e504cc1c0de)

In the event you would want to cite this blog post, you could use this template:
```
@electronic{ecoffet2018paper_repro_learning_to_learn_by_gradient_descent_by_gradient_descent,
  title={Paper repro: “Learning to Learn by Gradient Descent by Gradient Descent”},
  author={Ecoffet, Adrien},
  url = {https://medium.com/becoming-human/paper-repro-learning-to-learn-by-gradient-descent-by-gradient-descent-6e504cc1c0de},
  year={2018}
}
```