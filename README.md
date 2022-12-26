# Birds-Classification
![image](https://user-images.githubusercontent.com/109751694/209489396-5c73c6a0-6c01-44fe-be02-03dd88499564.png)


# Overview
This project uses ResNet101 to categorise photos of 200 different species of birds. In this project, studies were conducted using both the unfrozen one-to-one comparisons and the frozen version of ResNet.

# DataSet
Name : Caltech-UCSD Birds-200-2011
link to download :Download
Discribtion :CUB-200-2011 is an extended version of CUB-200 [7], a challenging dataset of 200 bird species. The extended version roughly doubles the number of images per category and adds new part localization annotations. All images are annotated with bounding boxes, part locations, and at- tribute labels. Images and annotations were filtered by mul- tiple users of Mechanical Turk. We introduce benchmarks and baseline experiments for multi-class categorization and part localization.

To run this project you should download the dataset and put the files in the folder 'CUB_200_2011'

# Methods
## Preprocessing
To enable the model to concentrate on the attributes of the birds themselves rather than the background, I preprocessed the photos to isolate just the faces of the birds and remove the background.
Scaling and resizing were also used.

## Modeling 
Resnet version 101, which has 101 layers, and adding more layers to the original 101 layers to create a new, good architecture.
Try training the entire model from scratch as well as adding some more layers.
### Freezed model

![image](https://user-images.githubusercontent.com/109751694/209489639-dcc095bb-454f-45d0-a462-6dd53f35cdb8.png)
### Unfreezed model
![image](https://user-images.githubusercontent.com/109751694/209489653-47487de7-da84-404b-a199-0ddd4c6f32d7.png)

From these results the freezed model is qiut better as the unfreezed model wasnt able to converge.

## Plot With TSNE
![image](https://user-images.githubusercontent.com/109751694/209489853-cbdff505-e30c-4dea-9c6d-ba0d0e2ae176.png)

