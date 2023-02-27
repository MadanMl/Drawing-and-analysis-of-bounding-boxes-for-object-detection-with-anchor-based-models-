# Drawing-and-analysis-of-bounding-boxes-for-object-detection-with-anchor-based-models
A repository for open-sourcing the datasets used in the paper "Drawing and analysis of bounding boxes for object detection with the anchor-based model" accepted in SCIA2023

* Author: Manav Madan (HFU)
* Task: Object detection for single-class objects
* Image_resolution: 416*416 px
* Label_fomat: yolo

## The Dataset structure
There are 2 main folders (Real and Artificial). 
* The "Real" folder contains the adapted chessboard dataset with the license. It is a single-class dataset of chess pieces. The dataset is divided into training ("train",276 images) and validation ("valid",30). Inside the sub folders, there are different folders for labels according to the experiment mentioned in the paper. Whereas images are kept in one folder as they do not change and only the labels change.
* The "Artificial" folder contains images for the synthetically generated dataset with circles as in binary images. The total number of generated images was 500 whereas in the "train" folder there are 475 and the "valid" folder has 25 images. The labels are kept in different folders according to the experiments mentioned in the paper. The images are divided into (one with noise and the other without)


## Citation
If you use these datasets in your work then please cite us using the following reference: