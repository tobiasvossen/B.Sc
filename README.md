# Bachelor thesis
- [B.Sc](https://github.com/tobiasvossen/B.Sc)
  - jupyter/ 
    - [colorization.ipynb](jupyter/colorization.ipynb) as [Jupyter Notebook](https://github.com/jupyter/notebook)
  - data/
    - Dataset examples
  - model/
    - Model summaries
    - [discriminator.h5](model/discriminator.h5) as discriminative model export
    - [generator.h5](model/generator.h5) as generative model export
  - deployment/
    - Colorized examples

## Title
Automatic colorization of gray-value images based on machine learning and deep generative neural networks

## Abstract
Generative models create - in contrast to object recognising discriminatory models – new content instead of just differentiating between well-known one. This reveals new possibilities of data synthesis, which are needed whenever it is not useful or even impossible to predict unknown content. The automatic colorization of gray-value images is a prime example for the use of a GAN (known as Generative Adversarial Network), which assigns as part of this work plausible color information to hueless patterns. Deep convolutional neural networks are used, which handle the colorization as a pixel-to-pixel transformation by the help of machine learning, with the result of historical black and white images being enhanced by a suitable color restoration.

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

## Acknowledgement
Implementation relies heavily on [TensorFlow](https://github.com/tensorflow/tensorflow) and [Keras](https://github.com/keras-team/keras)

Training process borrows from [TensorFlow Tutorial](https://www.tensorflow.org/tutorials/generative/pix2pix)

Hyperparameter search based on [TensorBoard Guide](https://www.tensorflow.org/tensorboard/hyperparameter_tuning_with_hparams)
