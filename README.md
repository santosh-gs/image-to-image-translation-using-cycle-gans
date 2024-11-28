# Image to Image Translation using CycleGANs

Main Paper: [Unpaired Image-to-Image Translation using Cycle-Consistent Adversarial Networks](https://arxiv.org/abs/1703.10593v7)

### horse <--> zebra

<p align="center">
  <img src="https://github.com/santosh-gs/image-to-image-translation-using-cycle-gans/blob/main/images/hose2zebra.png?raw=true" width="49%" />
  <img src="https://github.com/santosh-gs/image-to-image-translation-using-cycle-gans/blob/main/images/zebra2horse.png?raw=true" width="49%" />
</p>

### Training Framework

<p align="center">
  <img src="https://github.com/santosh-gs/image-to-image-translation-using-cycle-gans/blob/main/images/cyclegan_training_framework.png?raw=true" width="98%" />
</p>

Figure Credit: [MainPaper](https://arxiv.org/abs/1703.10593v7)

### Requirements
Tested Environment Setup:
* Python 3.9.13
* PyTorch 1.4.0
* torchvision 0.5.0
* Dominate 2.4.0
* Visdom >= 0.1.8.8
* Weights and Biases (wandb)