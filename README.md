# MobileNetV2-for-Disaster-Classification
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://drive.google.com/file/d/1rvrT2SJOzbDsQ6bYu1JqH_GbeLnSHxsd/view?usp=sharing) </br>

This jupyter notebook is to train a lightweight MobileNetV2 model for disaster classification using the [Crisis Image Benchmark Datasets (CrisisIBD)](https://crisisnlp.qcri.org/crisis-image-datasets-asonam20)

## Training Procedures

I train a MobileNetV2 for Disaster Classification using the procedures as described in the [paper](https://arxiv.org/pdf/2104.04184.pdf). </br>
The notable difference is I use weaker augmentations for my training. </br>
From my experiments, fine-tuning MobileNetV2 (pre-trained on ImageNet) is often less steady if the augmentations are too strong.

## Results

The benchmark values are extracted from Table 11 of the paper. </br>
I only compare with the MobileNetV2 results in the paper, as I only intend to train a MobileNetV2 with performance as close as the one described in the paper. </br>

| Model               | Acc.  | Prec. | Recall| F1    |
|---------------------|-------|-------|-------|-------|
| MobileNetV2 (paper) | 0.785 | 0.781 | 0.785 | 0.782 |
| MobileNetV2 (mine)  | 0.776 | 0.787 | 0.776 | 0.781 |

## Future Updates

- [x] Train a Multi-Task Model for Disaster Classification and Victim Detection
- [ ] Use other CNNs (such as EfficientNet)

Priority is given for first task, as it is part of my research project. </br>
Feel free to contribute ya :)
