---
title: "Waymo open dataset"
layout: post
date: 2020-12-20 16:17
tag: waymo
image: https://koppl.in/indigo/assets/images/jekyll-logo-light-solid.png
headerImage: false
projects: true
hidden: false # don't count this post in blog pagination
description: "Something about working on waymo dataset."
category: blog
author: Joss
externalLink: false
---
# Installing
- Use either their [pre-compiled package](https://pypi.org/project/waymo-open-dataset-tf-2-2-0/) or [build from source](https://github.com/waymo-research/waymo-open-dataset/tree/master/pip_pkg_scripts).
- If you want to use the third-party tool, their current installation is a mess. Please refer to [this comment](https://github.com/waymo-research/waymo-open-dataset/issues/146#issuecomment-747871191) and [this issue](https://github.com/waymo-research/waymo-open-dataset/issues/236) as a temporary workaround.

# Misc
Some useful commands when running on cluster.
- `module avail`, `module add gcc-8.3.0`
- `lsload -gpuload`

# More docs
please refer to [my doc](https://github.com/Jossome/Waymo-open-dataset-document) as a supplement to the official tutorial.
