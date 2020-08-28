# image-deblurring-neural-nets
Several architectures of neural networks used for image deblurring (more especifically residual CNNs, GANs and a proposed mixture of experts).

## 256colors: 
Experiments over images with 256 gradations of color (B&W or RGB).

## 8colors: 
Experiments over images with 8 gradations of gray (only B&W).

## mixture_of_experts:
Proposed mixture of trained CNNs for the restoration of images with 256 gradations of gray (only B&W).

#### Model of degradation used for the images (Gaussian Blur):
The degradation of the images was simulated by a gaussian point spread function (that have sigma and the dimension of the filter as parameters - with higher values for sigma and broader dimensions for the filter, worse the degradation).

#### Measure of similarity between images (SSIM Index):
The SSIM index was used to measure the similarity between the restoratios achieved and the original images without degradation. The SSIM index is contained in the interval [-1, 1] and returns 1 when both images are identical. This index takes in account characteriscs from the human visual system (see https://ece.uwaterloo.ca/~z70wang/publications/ssim.pdf).

#### Tensorflow version: 2.0.0

##### These notebooks were made for an undergraduate research project concerning "Image restoration with machine learning techniques". The file RelatorioFinal.pdf is the report (in portuguese) of such project. This research was made with support from Universidade de São Paulo (USP) and Fundação de Amparo à Pesquisa do Estado de São Paulo (FAPESP).
