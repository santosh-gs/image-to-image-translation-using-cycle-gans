# Image to Image Translation using CycleGANs

Main Paper: [Unpaired Image-to-Image Translation using Cycle-Consistent Adversarial Networks](https://arxiv.org/abs/1703.10593v7)

### Training Framework

<p align="center">
  <img src="https://github.com/santosh-gs/image-to-image-translation-using-cycle-gans/blob/main/images/cyclegan_training_framework.png?raw=true" width="98%" />
</p>

Figure Credit: [Main Paper](https://arxiv.org/abs/1703.10593v7)

(a) The CycleGAN model consists of two mapping functions, G: X → Y and F: Y → X, along with corresponding adversarial discriminators D_Y and D_X. The discriminator D_Y trains G to generate outputs that resemble domain Y, while D_X does the same for F with respect to domain X. To regularize these mappings, the model employs two cycle-consistency losses, ensuring that translating from one domain to another and then back reconstructs the original input. 
(b) The forward cycle-consistency loss ensures that x → G(x) → F(G(x)) ≈ x, while (c) the backward cycle-consistency loss ensures that y → F(y) → G(F(y)) ≈ y.

### horse <--> zebra

<p align="center">
  <img src="https://github.com/santosh-gs/image-to-image-translation-using-cycle-gans/blob/main/images/hose2zebra.png?raw=true" width="49%" />
  <img src="https://github.com/santosh-gs/image-to-image-translation-using-cycle-gans/blob/main/images/zebra2horse.png?raw=true" width="49%" />
</p>

### monet <--> photo

<p align="center">
  <img src="https://github.com/santosh-gs/image-to-image-translation-using-cycle-gans/blob/main/images/monet2photo.png?raw=true" width="49%" />
  <img src="https://github.com/santosh-gs/image-to-image-translation-using-cycle-gans/blob/main/images/photo2monet.png?raw=true" width="49%" />
</p>

### Requirements
Tested Environment Setup:
* Python 3.9.13
* PyTorch 1.4.0
* torchvision 0.5.0
* Dominate 2.4.0
* Visdoms 0.1.8.8
* Weights and Biases (wandb)