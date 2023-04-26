# Drawing-and-analysis-of-bounding-boxes-for-object-detection-with-anchor-based-models
A repository for open-sourcing the datasets used in the paper "Drawing and analysis of bounding boxes for object detection with the anchor-based model" accepted in SCIA2023

* Author: Manav Madan (HFU)
* Task: Object detection for single-class objects
* Image_resolution: 416*416 px
* Label_fomat: yolo

## The Dataset structure
There are 2 main folders (Real and Artificial). 
* The "Real" folder contains the adapted chessboard dataset ("ChessBoard") used in the paper. The original dataset with its license is also provided as a zip file ('ChessPiecesOriginal.zip') and the licence is also available with the original sources. The dataset used for the paper is a single-class dataset of chess pieces. The dataset is divided into training ("train",276 images) and validation ("valid",30). Inside the sub folders, there are different folders for labels according to the experiment mentioned in the paper. Whereas images are kept in one folder as they do not change and only the labels change.
* The "Artificial" folder contains images for the synthetically generated dataset with circles as in binary images. The total number of generated images was 500 whereas in the "train" folder there are 475 and the "valid" folder has 25 images. The labels are kept in different folders according to the experiments mentioned in the paper. The images are divided into (one with noise and the other without)


## Citation
If you use these datasets in your work then please cite us using the following reference:
@InProceedings{10.1007/978-3-031-31435-3_24,
author="Madan, Manav
and Reich, Christoph
and Hassenpflug, Frank",
editor="Gade, Rikke
and Felsberg, Michael
and K{\"a}m{\"a}r{\"a}inen, Joni-Kristian",
title="Drawing and Analysis of Bounding Boxes for Object Detection with Anchor-Based Models",
booktitle="Image Analysis",
year="2023",
publisher="Springer Nature Switzerland",
address="Cham",
pages="359--373",
abstract="Supervised object detection models are trained to recognize certain objects. These models are classified into two types: single-stage detectors and two-stage detectors. The single-stage detectors just need one pass through the model to anticipate all the bounding boxes, whereas the two-stage detectors require to first estimate the image portions where the object could be located. Due to their speed and simplicity, single-stage anchor-based models are used in many industrial settings. Training such models require bounding boxes that describe the spatial location of an object, which are usually drawn by an expert. However, the question remains, how much area should be considered when drawing the bounding boxes? In this paper, we demonstrate the effects that the size and placement of a rectangular bounding box can have on the performance of the anchor-based models. For this, we first perform experiments on a synthetically generated binary dataset and then on a real-world object detection dataset. Our results show that fixing the size of the bounding boxes can help in improving the performance of the model in the case of single class object detection (approximately 50{\%} improvement in mAP@[.5:.95] for real world dataset). Furthermore, we also demonstrate how freely available tools can be combined for obtaining the best possible semi automated object labeling pipeline.",
isbn="978-3-031-31435-3"
}
