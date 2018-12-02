---
title: "Disguise attack"
layout: post
date: 2018-05-01 12:00
tag: adversarial-machine-learning
image: https://koppl.in/indigo/assets/images/jekyll-logo-light-solid.png
headerImage: false
projects: true
hidden: true # don't count this post in blog pagination
description: "An adversarial attack based on one-pixel-attack by Su et al. (2017)."
category: project
author: Joss
externalLink: false
---
# Disguise Attack
An extreme attack base on the paper "One pixel attack for fooling deep neural networks".

## Demo
- Our results:
    - <img src="https://github.com/Jossome/one-pixel-attack-keras/blob/master/images/1.png" width="500" height="500">
- One-pixel-attack results:
    - <img src="https://github.com/Jossome/one-pixel-attack-keras/blob/master/images/one_pixel.png" width="500" height="500">

## What's new?
- Our adversarial pixel is harder or even impossible to find.
- Objective:
    - $$ L = e^{\gamma(C-1)} + \Delta $$, a soft manner.
    - where C stands for real class label, $\Delta$ stands for the difference between the pixel before and after attack.
    - $\gamma$ is a threshold to control the exponential growth rate.
- YUV color space:
    - https://en.wikipedia.org/wiki/YUV
    - The different $\Delta$ is calculated on YUV space instead of RGB space.

## TODO
- [x] Run on cifar10.
- [x] Run on basic leNet and ResNet.
- [ ] Regulation on $\Delta$.
- [ ] Run on more models.
- [ ] Run on imageNet.

