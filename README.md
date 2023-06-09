# Crowd-Counting using scale-adaptive Convolutional Neural Network


Implementation of the Paper: [Crowd counting via scale-adaptive convolutional neural network](https://arxiv.org/abs/1711.04433)

## Overview

This repository contains python implementation of the paper Crowd counting via scale-adaptive convolutional neural network by the Lu Zhang, Miaojing Shi, Qiaobo Chen. 

The paper introduces a novel approach to The main objective of the paper is to address the challenge of accurately estimating the number of pedestrians in crowd images, considering the scale and perspective changes that commonly occur. The paper proposes a novel approach called Scale-Adaptive CNN (SaCNN) architecture, which uses a backbone with fixed small receptive fields. The SaCNN extracts feature maps from multiple layers and adapts them to have the same output size, which are then combined to generate the final density map. The number of people in the crowd is computed by integrating the density map.

Additionally, the paper introduces a relative count loss along with the density map loss to enhance the network's generalization on crowd scenes with few pedestrians. This is particularly important as existing approaches often struggle in accurately counting sparse crowds.

To validate the proposed SaCNN architecture and loss function, the authors conduct extensive experiments on multiple datasets, including ShanghaiTech and a newly collected dataset called SmartCity. The experimental results demonstrate significant improvements of SaCNN over the state-of-the-art methods in accurately counting pedestrians in crowd images. 

This README provides an overview of the implementation and instructions for running the code.

## Dependencies

The following dependencies are required to run the code:

- Python (version 3.7)
- TensorFlow(1.x)
- NumPy
- Pandas

## Usage

The Code can be run by executing main.ipnyb

## Contributing

Contributions to this repository are welcome! If you encounter any issues or have suggestions for improvements, please feel free to open an issue or submit a pull request.

## Citation

```@article{zhang17sacnn,
Author = {Lu Zhang*, Miaojing Shi* and Qiaobo Chen},
Title = {Crowd Counting Via Sacle-adaptive Convolutional Neural Network},
booktitle= = {IEEE Winter Conference on Applications of Computer Vision (WACV)},
Year = {2018}
}
