# Project Description
This project utilizes deep learning techniques for the classification, detection, and recognition of various marine animals. By leveraging state-of-the-art AI models, it aims to contribute to initiatives in fishing, endangered animal protection, tracking, and analysis.

## Project Goals
Image Classification: Identify the marine animal in a given image.
Object Detection: Localize different instances of the same species within a single image.
Few-Shot Learning (Siamese Network): Recognize specific instances of certain sea animals, with a focus on whales.
## Dataset Description
The dataset for this project is available in this repository. It consists of five main classes: fish, jelly, shark, tuna, and whale. The dataset is organized into three main folders corresponding to the tasks of classification, detection, and few-shot learning.

#### Classification Folder

Structure: Divided into train and validation (val) subsets. Each subset contains five subfolders, one for each class.
Notes:
The first four folders (fish, jelly, shark, and tuna) include .txt files with detection annotations, which should be ignored for the classification task.
The classes are imbalanced and include images with lighting variations.
#### Detection Folder

Structure: Divided into train and val subsets. Contains only four classes: fish, jelly, shark, and tuna.
Annotations:
Each image has a corresponding annotation file with the same name as the image.
Example: The object detection annotations for image “323.jpg” can be found in “323.txt” in the same folder.
Each .txt file contains one or more lines, each corresponding to an object in the image, with six values: width, height, xmin, ymin, xmax, ymax.
Note: The width and height refer to the image dimensions, not the object's.
#### Few-Shot Learning Folder

Structure: Divided into train and val subsets, with each subset containing several subfolders named after whale IDs.
Notes:
Each whale ID has approximately 7-12 instances.
There are 50 whale IDs in the train set and 17 whale IDs in the val set.
Whales in the val set are different from those in the train set.
### Additional Bonus (Completed)
Applied image segmentation on the whale class to separate the whale tail from the background.
Measured the length of the whale tail using image processing algorithms.
