# LCA-KPConv

This repository contains the implementation of Kernel Point Convolution with Local Contextual Attention mechanism in PyTorch.

The code has been tested on 
CUDA 11.3, Python 3.7.16, and torch 1.11.0

# Installation  
For installation, please refer to https://github.com/HuguesTHOMAS/KPConv-PyTorch/blob/master/INSTALL.md

Trained models and prediction results are available at https://drive.google.com/drive/folders/1oapSEidRO8DWbKJPot3Woxi6LxXWHUmu


Currently, this repository only contains the code with the selected parameters for the STPLS3D dataset.
The code for Hessigheim3D and Toronto3D datasets will be released after the peer-review process

To reproduce the results on STPLS3D, 
Replace the folder path (Line 84):

https://github.com/onurcbayrak/LCA-KPConv/blob/main/datasets/STPLS3D.py#L84

      self.path = r"E:STPLS3D" -> self.path=r"YOUR_PATH"

and;

      python train_STPLS3D.py

For inference, change the log file's path to be produced under the results folder 

[(https://github.com/onurcbayrak/LCA-KPConv/blob/main/test_models.py#L53) and 

[(https://github.com/onurcbayrak/LCA-KPConv/blob/main/test_models.py#L96)

      python test_models.py

# An overview of the proposed LCA-KPConv architecture:
LCA-KPConv architecture obtains the highest classification scores in 3 benchmark datasets, as of August 2025. 

<img width="800" height="250" alt="image" src="https://github.com/user-attachments/assets/15917012-eabe-466d-8a9a-fa7f2cc99feb" />

# Results - STPLS3D

<img width="788" height="600" alt="image" src="https://github.com/user-attachments/assets/b77acce5-ec1c-42e5-ac07-b02f3ca46f28" />
<img width="512" height="487" alt="image" src="https://github.com/user-attachments/assets/86b2bf17-72fa-47db-91f2-754ba6efb3f5" />

# Results - Hessigheim3D

<img width="800" height="1000" alt="image" src="https://github.com/user-attachments/assets/4ecd1f19-846d-4b6e-8e0d-1818c99c18da" />
<img width="575" height="539" alt="image" src="https://github.com/user-attachments/assets/ac4d57b5-f1ac-493f-845a-63c4b54612d1" />

# Results - Toronto3D

<img width="671" height="443" alt="image" src="https://github.com/user-attachments/assets/2300b76b-38d7-48e4-88a7-e77cc38615b7" />
<img width="723" height="320" alt="image" src="https://github.com/user-attachments/assets/3c802417-b55e-44a8-bb3e-c9e0d8ba2594" />


