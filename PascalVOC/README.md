# Conditional-Detection---PASCAL-VOC
The Pascal VOC dataset for Conditional Detection and transform it into YOLOv8 annotation format, you can follow these steps:

## Overview
for the One Shot Object Detection challenge:
* 20 classes -> split -> 16 base classes & 4 novel classes
* Train (train): X images
* Valid-base (valid): X images
* Valid-novel (test): X images

```python
train_class_names = ['pottedplant', 'sofa', 'tvmonitor', 'car', 'bottle', 'boat', 'chair', 'person', 'bus', 'train', 'horse', 'bicycle', 'dog', 'bird', 'motorbike', 'diningtable']
test_class_names = ['cow', 'sheep', 'cat', 'aeroplane']
```


## Installation

#### Images/Annotations Processing 
Open and run the [Processing.ipynb](Processing.ipynb)

## Reference

* https://docs.ultralytics.com/fr/datasets/detect/voc/#dataset-yaml

* https://doi.org/10.1016/j.neucom.2020.04.092

* https://github.com/AICyberTeam/OSCD-datasets/tree/master/Pascal-OSCD

* http://host.robots.ox.ac.uk/pascal/VOC/ 

#### Citations for the PascalVOC authors

```
@Article{Everingham10,
   author = "Everingham, M. and Van~Gool, L. and Williams, C. K. I. and Winn, J. and Zisserman, A.",
   title = "The Pascal Visual Object Classes (VOC) Challenge",
   journal = "International Journal of Computer Vision",
   volume = "88",
   year = "2010",
   number = "2",
   month = jun,
   pages = "303--338",
} 

@article{fu_oscd_2021,
	title = {{OSCD}: {A} one-shot conditional object detection framework},
	volume = {425},
	issn = {0925-2312},
	shorttitle = {{OSCD}},
	url = {https://www.sciencedirect.com/science/article/pii/S0925231220306779},
	doi = {10.1016/j.neucom.2020.04.092},
	abstract = {The current advances in object detection depend on large-scale datasets to get good performance. However, there may not always be sufficient samples in many scenarios, resulting in the performance degradation of the current deep learning based object detection models. To overcome this problem, we propose a novel one-shot conditional detection framework (OSCD). Given a support image of the target object and a query image as input, OSCD can detect all objects belonging to the target object category in the query image. Specifically, OSCD is composed of a Siamese network and a two-stage detection model. In each stage of the two-stage detection pipeline, a feature fusion module and a learnable metric module are designed for effective conditional detection respectively. Once trained, OSCD can detect objects of both seen and unseen classes without further training, which also has advantages including class-agnostic, training-free for unseen classes, and without catastrophic forgetting. Experiments show that the proposed approach achieves state-of-the-art performance on the proposed datasets based on Fashion-MNIST and Pascal VOC.},
	language = {en},
	urldate = {2023-01-23},
	journal = {Neurocomputing},
	author = {Fu, Kun and Zhang, Tengfei and Zhang, Yue and Sun, Xian},
	month = feb,
	year = {2021},
	keywords = {Object detection, One-shot},
	pages = {243--255},
	file = {ScienceDirect Snapshot:C\:\\Users\\User\\Zotero\\storage\\5GSSJEBY\\S0925231220306779.html:text/html},
}

```