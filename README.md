# LCA-KPConv

This repository contains the implementation of Kernel Point Convolution with Local Contextual Attention mechanism in PyTorch.

The code has been tested on 
CUDA 11.3, Python 3.7.16, and torch 1.11.0

# Installation  
For installation, please refer to https://github.com/HuguesTHOMAS/KPConv-PyTorch/blob/master/INSTALL.md

Trained models and prediction results are available at https://drive.google.com/drive/folders/1oapSEidRO8DWbKJPot3Woxi6LxXWHUmu


Currently, this repository only contains the code with the selected parameters for the STPLS3D dataset.
The code for Hessigheim3D and Toronto3D datasets will be released after the journal paper completes the peer-review process

To reproduce the results on STPLS3D, 
Replace the folder path (Line 84):

https://github.com/onurcbayrak/LCA-KPConv/blob/main/datasets/STPLS3D.py#L84

      self.path = r"E:STPLS3D" -> self.path=r"YOUR_PATH"

and\l
      python train_STPLS3D.py

For inference, change the log file path at [(https://github.com/onurcbayrak/LCA-KPConv/blob/main/test_models.py#L53) and [(https://github.com/onurcbayrak/LCA-KPConv/blob/main/test_models.py#L96)

      python test_models.py


