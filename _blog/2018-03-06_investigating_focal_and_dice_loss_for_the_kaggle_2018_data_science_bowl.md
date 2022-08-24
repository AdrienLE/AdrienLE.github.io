---
title: "Investigating Focal and Dice Loss for the Kaggle 2018 Data Science Bowl"
collection: blog
permalink: /blog/2018-03-06_investigating_focal_and_dice_loss_for_the_kaggle_2018_data_science_bowl
excerpt: "This post details my experiments and implementations with three important loss functions for the Kaggle 2018 data science bowl, and compares their effects on a simplified implementation of U-Net."
date: 2018-03-06
paperurl: 'https://medium.com/becoming-human/investigating-focal-and-dice-loss-for-the-kaggle-2018-data-science-bowl-65fb9af4f36c'
authors: '<span class="me">Adrien Ecoffet</span>'
---
This post details my experiments and implementations with three important loss functions for the Kaggle 2018 data science bowl, and compares their effects on a simplified implementation of U-Net.

The loss functions I investigate are binary cross entropy (referred to as “nll” in the notebook because my initial version used the related NLLLoss instead of BCE), the soft-dice loss (introduced in “V-Net: Fully Convolutional Neural Networks for Volumetric Medical Image Segmentation” and generally considered to be useful for segmentation problems), and the focal loss.




[View full post here](https://medium.com/becoming-human/investigating-focal-and-dice-loss-for-the-kaggle-2018-data-science-bowl-65fb9af4f36c)

In the event you would want to cite this blog post, you could use this template:
```
@electronic{ecoffet2018investigating_focal_and_dice_loss_for_the_kaggle_2018_data_science_bowl,
  title={Investigating Focal and Dice Loss for the Kaggle 2018 Data Science Bowl},
  author={Ecoffet, Adrien},
  url = {https://medium.com/becoming-human/investigating-focal-and-dice-loss-for-the-kaggle-2018-data-science-bowl-65fb9af4f36c},
  year={2018}
}
```