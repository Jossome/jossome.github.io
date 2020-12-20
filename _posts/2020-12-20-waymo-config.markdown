---
title: "Installing Waymo open dataset"
layout: post
date: 2020-12-20 16:17
tag: misc
image: https://koppl.in/indigo/assets/images/jekyll-logo-light-solid.png
headerImage: false
projects: true
hidden: false # don't count this post in blog pagination
description: "How to correctly configure waymo dataset installation."
category: blog
author: Joss
externalLink: false
---
# Installing Waymo-open-dataset

## Some notes on using `bazel`
- Before building, do `export TEST_TMPDIR=/tmp/bazel` to avoid runing it on NFS.

## Misc
Some useful commands when running on cluster.
- `module avail`, `module add gcc-8.3.0`
- `lsload -gpuload`

## More docs
please refer to [my doc](https://github.com/Jossome/Waymo-open-dataset-document) as a supplement to the official tutorial.
