# RL-GAN-Net: Point Cloud Shape Completion with Reinforcement Learning

This project draws inspiration from the CVPR 2019 paper titled "RL-GAN-Net: A Reinforcement Learning Agent Controlled GAN Network for Real-Time Point Cloud Shape Completion." It aims to recreate and explore the concepts presented in the paper for personal learning and experimentation purposes.

## Requirements

The required packages for this project are listed in the `Requirement_Conda.txt` and `Requirements_pip.txt` files. You can choose to install only the necessary packages or clone the entire environment.

## Getting Started

Follow these steps to use the RL-GAN-Net:

1. Download the data from [https://github.com/optas/latent_3d_points](https://github.com/optas/latent_3d_points).
2. Process the data using `Processdata2.m` to obtain incomplete point clouds.
3. Train the autoencoder using `main.py` and save the model.
4. Generate Global Feature Vectors (GFV) using the pretrained autoencoder (AE) with `GFV.py` and store the data.
5. Train the Generative Adversarial Network (GAN) on the generated GFV data by going into the GAN folder and using `trainer.py`. Save the model.
6. Train the Reinforcement Learning (RL) agent by using the pre-trained GAN and AE with `trainRL.py`.
7. Test with incomplete data by running `testRL.py`.

## Citation

If you find this work useful for your projects, please consider citing our CVPR paper:

```
@InProceedings{Sarmad_2019_CVPR,
author = {Sarmad, Muhammad and Lee, Hyunjoo Jenny and Kim, Young Min},
title = {RL-GAN-Net: A Reinforcement Learning Agent Controlled GAN Network for Real-Time Point Cloud Shape Completion},
booktitle = {The IEEE Conference on Computer Vision and Pattern Recognition (CVPR)},
month = {June},
year = {2019}
}
```

The original implementation and data credits go to their respective authors. This information is presented here for personal understanding and educational purposes.