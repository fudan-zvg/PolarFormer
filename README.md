# PolarFormer

This repository is an official implementation of  PolarFormer.

Our new Polar Transformer (PolarFormer), takes as input multi-camera 2D images for 3D object detection in the bird's-eye-view (BEV). Specifically, we design a cross-attention based Polar detection head and a multi-scale Polar representation learning strategy. We make best use of the Polar representation rasterized via attending to the corresponding image observation in a sequence-to-sequence fashion subject to the geometric constraints. The DD3D pretrained VoVNet (V2-99) and nuScenes pretrained ResNet101-DCN are adopted as backbone networks. We do not perform test-time augmentation and use a single model for inference.

## News
**2022.05.18**: PolarFormer achieves state-of-the-art performance among the published works (**57.2% NDS** and **49.3% mAP**) on nuScenes 3D Object Detection [Leaderboard](https://www.nuscenes.org/object-detection?externalData=all&mapData=no&modalities=Camera).

## Get Started

### Environment
This implementation is build upon  [detr3d](https://github.com/WangYueFt/detr3d/blob/main/README.md), please follow the steps in [install.md](./docs/install.md) to prepare the environment.

### Data
Please follow the official instructions of mmdetection3d to process the nuScenes dataset.(https://mmdetection3d.readthedocs.io/en/latest/datasets/nuscenes_det.html)



## Acknowledgement
Many thanks to the following open-source projects:
* [mmdetection3d](https://github.com/open-mmlab/mmdetection3d)
* [detr3d](https://github.com/WangYueFt/detr3d)