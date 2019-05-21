# BASNet
Code for paper '[*BASNet: Boundary-Aware Salient Object Detection*](https://webdocs.cs.ualberta.ca/~xuebin/BASNet.pdf)', [Xuebin Qin](https://webdocs.cs.ualberta.ca/~xuebin/), Zichen Zhang, Chenyang Huang(http://webdocs.cs.ualberta.ca/~chuang8/), Chao Gao, Masood Dehghan and Martin Jagersand. [(supplementary)](https://webdocs.cs.ualberta.ca/~xuebin/BASNet-supp.pdf)  

__Contact__: xuebin[at]ualberta[dot]ca

## Required libraries

Python 3.6  
numpy 1.15.2  
scikit-image 0.14.0  
PIL 5.2.0  
PyTorch 0.4.0  
torchvision 0.2.1  
glob  

The SSIM loss is adapted from [pytorch-ssim](https://github.com/Po-Hsun-Su/pytorch-ssim/blob/master/pytorch_ssim/__init__.py).  

## Usage
1. Clone this repo
```
git clone https://github.com/NathanUA/BASNet.git
```
2. Download the pre-trained model [basnet.pth](https://drive.google.com/file/d/1qeKYOTLIOeSJGqIhFJOEch48tPyzrsZx/view?usp=sharing) and put it into the dirctory 'saved_models/basnet_bsi/'

3.  Cd to the directory 'BASNet', run the training and inference process by command: ```python basnet_test.py```
and ```python basnet_train.py``` respectively.  

 We also provide the predicted [saliency maps](https://drive.google.com/file/d/1K9y9HpupXT0RJ4U4OizJ_Uk5byUyCupK/view?usp=sharing) for datasets SOD, ECSSD, DUT-OMRON, PASCAL-S, HKU-IS and DUTS-TE.

## Architecture

![BASNet architecture](figures/architecture.png)


## Quantitative Comparison

![Quantitative Comparison](figures/quan.png)

## Qualitative Comparison

![Qualitative Comparison](figures/qual.png)

## Citation
```
@InProceedings{Qin_2019,
  author = {Qin, Xuebin and Zhang, Zichen and Huang, Chenyang and Gao, Chao and Dehghan, Masood and Jagersand, Martin},
  title = {BASNet: Boundary Aware Salient Object Detection},
  year = {2019}
}
```
