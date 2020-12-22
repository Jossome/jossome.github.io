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

# Leaderboard
## Detection
- 2D detection: only visual camera is allowed.
- 3D detection: all sensors are allowed.
- Metric:
    - AP/L2 means AP for Level-2 difficulty. This AP is calculated on both L1 and L2 labels.
    - If the code we use doesn't specify or filter the difficulty level, then we should compare the L2 AP with our trained models.
    - I highly suspect that submissions on leaderboards are prediction on all cameras, while I'm only predicting on the front view.

# YOLO on Waymo
Using YOLOv4 on Waymo.
- Cannot find a reliable PyTorch repo right now. First try mmdet::yolov4 branch; Second, the personal repo mmdet-yolov4; Third, Wong's implementation since he is one of the contributors of the darknet repo; Fourth, the c implementation.
- May need to adjust the anchor settings. Try to understand how this works. Or may not.

# Misc
Some useful commands when running on cluster.
- `module avail`, `module add gcc-8.3.0`
- `lsload -gpuload`

# More docs
please refer to [my doc](https://github.com/Jossome/Waymo-open-dataset-document) as a supplement to the official tutorial.
