<img width="896" height="560" alt="image" src="https://github.com/user-attachments/assets/ecbc9a53-3291-4034-8bfe-2583913325c1" />
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

and;

      python train_STPLS3D.py

For inference, change the log file's path to be produced under the results folder 

[(https://github.com/onurcbayrak/LCA-KPConv/blob/main/test_models.py#L53) and 

[(https://github.com/onurcbayrak/LCA-KPConv/blob/main/test_models.py#L96)

      python test_models.py

# An overview of the proposed LCA-KPConv architecture:
LCA-KPConv architecture obtains the highest classification scores in 3 benchmark datasets, as of August 2025. 

<img width="800" height="250" alt="image" src="https://github.com/user-attachments/assets/32b1c261-e776-4f20-8ece-c38a1494dd57" />
<img width="512" height="487" alt="image" src="https://github.com/user-attachments/assets/86b2bf17-72fa-47db-91f2-754ba6efb3f5" />


# Results - STPLS3D

<img width="896" height="560" alt="image" src="https://github.com/user-attachments/assets/2a3e0fef-e96f-4391-9cd5-77c61ce29885" />

# Results - Hessigheim3D

<img width="989" height="646" alt="image" src="https://github.com/user-attachments/assets/8f9bac53-0f36-4b0e-af73-eca9051db1a9" />


# Results - Toronto3D

<img width="858" height="566" alt="image" src="https://github.com/user-attachments/assets/c9d5156e-ea62-4d59-86e3-9ddd68bdd460" />


