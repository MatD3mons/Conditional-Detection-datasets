# Conditional Detection - Retail Product Checkout Dataset
The Retail Product Checkout (RPC) dataset for Conditional Detection and transform it into YOLOv8 annotation format, you can follow these steps:

## Overview
for the One Shot Object Detection challenge:
* 200 classes -> split -> 160 base classes & 40 novel classes
* Train (train): 20,958 images
* Valid-base (valid): 8,982 images
* Valid-novel (test): 21,561 images

## Installation

#### Kaggle Authenticate
* Go to your Kaggle account settings and create a new API token.
* This will download a kaggle.json file. Move this file to ~/.kaggle/.

#### Download the Retail Product Checkout (RPC) dataset
```
kaggle datasets download diyer22/retail-product-checkout-dataset
```
```
unzip retail-product-checkout-dataset
```
#### Images/Annotations Processing 
Open and run the [Processing.ipynb](Processing_RPC.ipynb)

## Reference

* https://www.kaggle.com/datasets/diyer22/retail-product-checkout-dataset

* https://github.com/tongyuhome/rpc 

* https://rpc-dataset.github.io/

* https://arxiv.org/abs/1901.07249

#### Citations for the RPC authors

```
@article{wei_rpc_2022,
	title = {{RPC}: a large-scale and fine-grained retail product checkout dataset},
	volume = {65},
	issn = {1869-1919},
	url = {https://doi.org/10.1007/s11432-022-3513-y},
	doi = {10.1007/s11432-022-3513-y},
	number = {9},
	journal = {Science China Information Sciences},
	author = {Wei, Xiu-Shen and Cui, Quan and Yang, Lei and Wang, Peng and Liu, Lingqiao and Yang, Jian},
	month = aug,
	year = {2022},
	pages = {197101},
}
```

```
@misc{wei2019rpc,
      title={RPC: A Large-Scale Retail Product Checkout Dataset}, 
      author={Xiu-Shen Wei and Quan Cui and Lei Yang and Peng Wang and Lingqiao Liu},
      year={2019},
      eprint={1901.07249},
      archivePrefix={arXiv},
      primaryClass={id='cs.CV' full_name='Computer Vision and Pattern Recognition' is_active=True alt_name=None in_archive='cs' is_general=False description='Covers image processing, computer vision, pattern recognition, and scene understanding. Roughly includes material in ACM Subject Classes I.2.10, I.4, and I.5.'}
}
```
