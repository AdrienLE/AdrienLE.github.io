---
title: "Video PreTraining (VPT): Learning to Act by Watching Unlabeled Online Videos"
collection: publications
permalink: /publication/2022-06-23-video-pretraining
excerpt: 'We show that with a small amount of labeled data we can train an inverse dynamics model accurate enough to label a huge unlabeled source of online data -- here, online videos of people playing Minecraft -- from which we can then train a general behavioral prior. '
date: 2022-06-23
venue: 'arXiv'
paperurl: 'https://arxiv.org/pdf/2206.11795.pdf'
authors: 'Bowen Baker, Ilge Akkaya, Peter Zhokhov, Joost Huizinga, Jie Tang, <span class="me">Adrien Ecoffet</span>, Brandon Houghton, Raul Sampedro, Jeff Clune'
---
Pretraining on noisy, internet-scale datasets has been heavily studied as a technique for training models with broad, general capabilities for text, images, and other modalities. However, for many sequential decision domains such as robotics, video games, and computer use, publicly available data does not contain the labels required to train behavioral priors in the same way. We extend the internet-scale pretraining paradigm to sequential decision domains through semi-supervised imitation learning wherein agents learn to act by watching online unlabeled videos. Specifically, we show that with a small amount of labeled data we can train an inverse dynamics model accurate enough to label a huge unlabeled source of online data -- here, online videos of people playing Minecraft -- from which we can then train a general behavioral prior. Despite using the native human interface (mouse and keyboard at 20Hz), we show that this behavioral prior has nontrivial zero-shot capabilities and that it can be fine-tuned, with both imitation learning and reinforcement learning, to hard-exploration tasks that are impossible to learn from scratch via reinforcement learning. For many tasks our models exhibit human-level performance, and we are the first to report computer agents that can craft diamond tools, which can take proficient humans upwards of 20 minutes (24,000 environment actions) of gameplay to accomplish.

[Download paper here](https://arxiv.org/pdf/2206.11795.pdf)

You can cite this work using the BibTeX from Google Scholar, which should be as follows:
```
@article{baker2022video,
  title={Video PreTraining (VPT): Learning to Act by Watching Unlabeled Online Videos},
  author={Baker, Bowen and Akkaya, Ilge and Zhokhov, Peter and Huizinga, Joost and Tang, Jie and Ecoffet, Adrien and Houghton, Brandon and Sampedro, Raul and Clune, Jeff},
  journal={arXiv preprint arXiv:2206.11795},
  year={2022}
}
```