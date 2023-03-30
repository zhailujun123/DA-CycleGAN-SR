# Introduction

This repo contains an unofficial implementation of [pseudo-sr](https://openaccess.thecvf.com/content_CVPR_2020/papers/Maeda_Unpaired_Image_Super-Resolution_Using_Pseudo-Supervision_CVPR_2020_paper.pdf).

![main image](./misc/figure.PNG)

Download the dataset from [here](https://github.com/jingyang2017/Face-and-Image-super-resolution).

# Usage

First, configure the yaml file which is located at `configs/faces.yaml`. Set the root folder of face dataset to `DATA.FOLDER`.

To train:
python3 train.py configs/faces.yaml
```
CUDA_VISIBLE_DEVICES=2,3 python train.py configs/faces.yaml --port 12121
```

The `--port` option is only required for multi-gpu training.
You can use a number between 49152 and 65535 for the port number. 

# Reproducibility

TBA

# Reference

Maeda, Shunta. "Unpaired Image Super-Resolution using Pseudo-Supervision." Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition. 2020.
