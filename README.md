# **Automated algorithmic bias analysis of Twitter saliency filter**

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1eZpt6KPtrlA2egvuTnyS31v3UqDJScCD?usp=sharing)

This repository hosts a Jupyter notebook that introduces a few broad concepts, to help further develop automated testing tools for detecting algorithmic bias in machine vision tools, such as saliency filters.

The tool evaluated here is the [Twitter saliency filter](https://github.com/twitter-research/image-crop-analysis).

[FairFace: the face attribute dataset that is balanced for gender, race and age](https://arxiv.org/abs/1908.04913v1); is used here to generate the random image pairs for performing the saliency filter tests.

Quantification of the statisitcal significance in differences between the carefully manipulated saliency filter outputs and the baseline saliency filter outputs, is performed using the [Wilcoxon signed rank test](https://en.wikipedia.org/wiki/Wilcoxon_signed-rank_test).
Twitter saliency filter algorithmic bias analysis using automated tools

### Additional requirements

* Valid Google account
* This notebook by default assumes that the user is working inside the original [Google Colab environment](https://colab.research.google.com/drive/1eZpt6KPtrlA2egvuTnyS31v3UqDJScCD?usp=sharing). To run locally or in other cloud environments, please make sure that the data dependencies are satisfied.
* Google Drive access to save the FairFace dataset and the experiment history

```
Parts of the code used in this notebook are copyright protected.
Copyright 2021 Twitter, Inc.
SPDX-License-Identifier: Apache-2.0
```

## Data download
Download the FairFace dataset **`fairface-img-margin125-trainval.zip`** file and the labels **`fairface_label_train.csv`** file from the official **[FairFace GitHub repo](https://github.com/joojs/fairface)**.
