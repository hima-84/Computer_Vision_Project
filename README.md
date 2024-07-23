# Computer_Vision_Project
## Project Overview 
This project aims to leverage deep learning techniques for the classification, detection, and recognition of various marine animals. By utilizing state-of-the-art AI models, this project contributes to efforts in fishing, endangered animal protection, tracking, and analysis.

### Project Objectives:
Image Classification: Identify the marine animal in a given image.
Object Detection: Localize different instances of the same species within a single image.
Few-Shot Learning (Siamese Network): Recognize specific instances of a certain sea animal, focusing on whales.

### Dataset Description
The project dataset can be found also in this Repository.

The dataset consists of five main classes: fish, jelly, shark, tuna, and whale. It is organized into three main folders corresponding to the three tasks: classification, detection, and few-shot learning.

1. Classification Folder
Structure:
Separated into train and val subsets.
Contains five subfolders, each representing one of the five classes.
Each subfolder contains images corresponding to that class.
Notes:
The first four folders (fish, jelly, shark, and tuna) contain .txt files with detection annotations. These .txt files should be ignored for the classification task.
The classes are unbalanced and include images with lighting variations.
2. Detection Folder
Structure:
Separated into train and val subsets.
Contains only four classes: fish, jelly, shark, and tuna.
Each image has a corresponding annotation file with the same name as the image.
Annotations:
Example: The object detection annotations for image “323.jpg” can be found in “323.txt” in the same folder.
Each .txt file contains 1 or more lines, each corresponding to an object in the image.
Each line in a .txt file has 6 values: width, height, xmin, ymin, xmax, ymax.
Note: The width and height refer to the image dimensions, not the object's.
3. Few-Shot Learning Folder
Structure:
Separated into train and val subsets.
Each subset is divided into several subfolders, with each folder named after a whale ID.
Notes:
Each whale ID has approximately 7-12 instances.
There are 50 whale IDs in the train set and 17 whale IDs in the val set.
Whales in the val set are different from those in the train set.
