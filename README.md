# Mobilenet-Edge-TPU

This repository contains a PyTorch pretrained model of the EdgeTPU-DeepLab model, originally developed in TensorFlow. The EdgeTPU-DeepLab model is a deep learning model for semantic segmentation, specifically designed to run on Edge TPUs.

For more information on the original EdgeTPU-DeepLab model and the MobileNet Edge TPU model, please refer to the following resources:

- [EdgeTPU-DeepLab Model Zoo](https://github.com/tensorflow/models/blob/master/research/deeplab/g3doc/model_zoo.md)
- [MobileNet Edge TPU](https://github.com/tensorflow/models/tree/master/research/slim/nets/mobilenet)


## Model Conversion

The TensorFlow pretrained EdgeTPU-DeepLab has been converted to a PyTorch format for easier integration into PyTorch-based projects. The converted model file can be found at `torch_mobilenet_edgetpu/mobilenet_edgetpu.pth`.

**Note:** This pretrained model only contains the backbone part of the model and does not include the decoder. It is intended for subsequent model training. Additionally, the pretrained model does not contain logits as they are usually replaced with the required class numbers.
