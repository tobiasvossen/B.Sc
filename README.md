# Bachelor thesis
- [B.Sc](https://github.com/tobiasvossen/B.Sc)
  - jupyter/ 
    - [colorisation.ipynb](jupyter/colorisation.ipynb) as [Jupyter Notebook](https://github.com/jupyter/notebook)
  - data/
    - Dataset examples
  - model/
    - Model summaries
    - [discriminator.h5](models/discriminator.h5) as discriminative model export
    - [generator.h5](models/generator.h5) as generative model export
  - deployment/
    - Colorised examples

## Title
Automatic colorisation of grey-value images based on machine learning and deep generative neural networks.

## Abstract
...

## Baseline
Based on [Pix2Pix](https://github.com/phillipi/pix2pix) by Isola et al. from [Image-to-Image Translation with Conditional Adversarial Networks](https://arxiv.org/abs/1611.07004)

## Data
Trained on [Places365](https://github.com/CSAILVision/places365) by Zhou et al. from [Places: A 10 million Image Database for Scene Recognition](https://www.researchgate.net/publication/318200394_Places_A_10_Million_Image_Database_for_Scene_Recognition)

## Model
- [Generative Adversarial Network](https://arxiv.org/abs/1406.2661)
  - Architecture
    - [U-Net](https://arxiv.org/abs/1505.04597) as Generator
    - [PatchGAN](https://arxiv.org/abs/1604.04382) as Discriminator
  - Loss
    - Binary crossentropy
    - L1 deviation

## Deployment
...

## Release
| Release | Date     |
| :-------|---------:|
| 1.0.0   | 31.01.20 | 
    
## Software
| Software          | Version  |
| :-----------------|---------:|
| CoLab             | 1.0.0    | 
| Keras             | 2.2.4    | 
| Python            | 3.6.9    |
| TensorBoard       | 2.1.0    |
| TensorFlow        | 2.1.0    |
| TensorFlow Addons | 0.6.0    |
