# image-deblurring-neural-nets
Several architectures of neural networks used for image deblurring (more especifically: residual CNNs, GANs and a proposed mixture of experts). Implementation with TensorFlow and Keras.

## 256colors: 
Experiments with images presenting up to 256 different gradations of color (B&W or RGB).

## 8colors: 
Experiments with images presenting only 8 different gradations of gray (only B&W).

## mixture_of_experts:
Proposed mixture of trained CNNs for the restoration of images presenting up to 256 different gradations of gray (only B&W).

#### Model of degradation used for the images (Gaussian Blur):
The degradation of the images is simulated by a gaussian point spread function (PSF), that has as parameters the value of standard deviation (sigma) and the size of filter (with higher values for sigma and broader sizes of filter, worse the degradation).

#### Measure of similarity between images (SSIM Index):
The SSIM index is used to measure the similarity between the restorations achieved and the original images without degradation. The SSIM index is contained in the interval [-1, 1] and returns 1 when both images are identical. This index takes in account characteristics from the human visual system (see https://ece.uwaterloo.ca/~z70wang/publications/ssim.pdf). At this repository, it is proposed a loss function for neural networks based on the SSIM index.

#### TensorFlow version: 2.0.0

##### These notebooks were made for an undergraduate research project concerning "Image restoration with machine learning techniques". The research was done by Guilherme A. Lizarzaburu (guilherme.a.lizarzaburu@gmail.com) with support from Fundação de Amparo à Pesquisa do Estado de São Paulo (FAPESP) and Universidade de São Paulo (USP).
