# Conditional-Detection---Grozi-3.2k-Dataset
The Grozi-3.2k dataset for Conditional Detection and transform it into YOLOv8 annotation format, you can follow these steps:

## Overview
for the One Shot Object Detection challenge:
* 1063 classes -> split -> 879 base classes & 185 novel classes
* Train (train): 596 images
* Valid-base (valid): 60 images
* Valid-novel (test): 84 images
* dairy: 12 images - 166 classes 
* paste: 91 images - 259 classes

## Installation

#### Install library python
```
pip install -r requirement.txt
```
#### Images/Annotations Processing 
Open and run the [Processing.ipynb](Processing.ipynb)

## Reference

* https://onlinelibrary.wiley.com/doi/10.1155/2020/8875910

* https://github.com/aosokin/os2d

* https://github.com/tobiagru/ObjectDetectionGroceryProducts/blob/master/README.md

#### Citations for the RPC authors

```
@article{wei_deep_2020,
	title = {Deep {Learning} for {Retail} {Product} {Recognition}: {Challenges} and {Techniques}},
	volume = {2020},
	issn = {1687-5265},
	shorttitle = {Deep {Learning} for {Retail} {Product} {Recognition}},
	url = {https://www.hindawi.com/journals/cin/2020/8875910/},
	doi = {10.1155/2020/8875910},
	abstract = {Taking time to identify expected products and waiting for the checkout in a retail store are common scenes we all encounter in our daily lives. The realization of automatic product recognition has great significance for both economic and social progress because it is more reliable than manual operation and time-saving. Product recognition via images is a challenging task in the field of computer vision. It receives increasing consideration due to the great application prospect, such as automatic checkout, stock tracking, planogram compliance, and visually impaired assistance. In recent years, deep learning enjoys a flourishing evolution with tremendous achievements in image classification and object detection. This article aims to present a comprehensive literature review of recent research on deep learning-based retail product recognition. More specifically, this paper reviews the key challenges of deep learning for retail product recognition and discusses potential techniques that can be helpful for the research of the topic. Next, we provide the details of public datasets which could be used for deep learning. Finally, we conclude the current progress and point new perspectives to the research of related fields.},
	language = {en},
	urldate = {2023-01-24},
	journal = {Computational Intelligence and Neuroscience},
	author = {Wei, Yuchen and Tran, Son and Xu, Shuxiang and Kang, Byeong and Springer, Matthew},
	month = nov,
	year = {2020},
	note = {Publisher: Hindawi},
	pages = {e8875910},
	file = {Full Text PDF:C\:\\Users\\User\\Zotero\\storage\\YW34DJXR\\Wei et al. - 2020 - Deep Learning for Retail Product Recognition Chal.pdf:application/pdf},
}

```

```
@inproceedings{osokin_os2d_2020,
	address = {Cham},
	series = {Lecture {Notes} in {Computer} {Science}},
	title = {{OS2D}: {One}-{Stage} {One}-{Shot} {Object} {Detection} by {Matching} {Anchor} {Features}},
	isbn = {978-3-030-58555-6},
	shorttitle = {{OS2D}},
	doi = {10.1007/978-3-030-58555-6_38},
	abstract = {In this paper, we consider the task of one-shot object detection, which consists in detecting objects defined by a single demonstration. Differently from the standard object detection, the classes of objects used for training and testing do not overlap. We build the one-stage system that performs localization and recognition jointly. We use dense correlation matching of learned local features to find correspondences, a feed-forward geometric transformation model to align features and bilinear resampling of the correlation tensor to compute the detection score of the aligned features. All the components are differentiable, which allows end-to-end training. Experimental evaluation on several challenging domains (retail products, 3D objects, buildings and logos) shows that our method can detect unseen classes (e.g., toothpaste when trained on groceries) and outperforms several baselines by a significant margin. Our code is available online: https://github.com/aosokin/os2d.},
	language = {en},
	booktitle = {Computer {Vision} – {ECCV} 2020},
	publisher = {Springer International Publishing},
	author = {Osokin, Anton and Sumin, Denis and Lomakin, Vasily},
	editor = {Vedaldi, Andrea and Bischof, Horst and Brox, Thomas and Frahm, Jan-Michael},
	year = {2020},
	keywords = {Object detection, Few-shot learning, One-shot detection},
	pages = {635--652},
	file = {Version soumise:C\:\\Users\\User\\Zotero\\storage\\85VUMGRV\\Osokin et al. - 2020 - OS2D One-Stage One-Shot Object Detection by Match.pdf:application/pdf},
}

```