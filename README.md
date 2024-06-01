# Classification of Wind Turbine Components based on Synthetic Image Analysis through Deep Learning for Computer Vision






## Description

The README file is meant to explain the structure of this repository, the codes, and their applications. This repository serves as an additional resource to facilitate the inspection of codes used for this thesis. The codes were written in Python and used in Google Colab, Blender, or Visual Studio Code, depending on the task.

## Synthetic Dataset Generation

The file names are ordered chronologically, starting with background generation, the output of which was 
used for image generation. Next, the pictures were resized. Finally, annotations had to be generated for 
each complexity separately, along with testing annotations.

### Background generation:
- **COMPOSITE BACKGROUND GENERATION (LOCAL).ipynb**: This script generates composite backgrounds for use in the high complexity dataset.

### Blender coding:
- **IMAGE GENERATION (BLENDER CODE).ipynb**: This Blender script, written in Python, is meant to be used within Blender for automated synthetic image generation. It provides several randomized parameters that can be modified to increase or decrease the diversity of generated images. It was used to generate three sets of pictures with low, medium, and high complexity.

### Image resizing:
- **IMAGE RESIZING (LOCAL).ipynb**: A script for image resizing (to save space due to large datasets), meant to be used locally in Visual Studio Code for fast folder manipulation.

### Annotations generation:
- **LOW COMPLEXITY ANNOTATIONS – GENERATION.ipynb**
- **MEDIUM COMPLEXITY ANNOTATIONS – GENERATION.ipynb**
- **HIGH COMPLEXITY ANNOTATIONS – GENERATION.ipynb**
- **TESTING ANNOTATIONS – GENERATION_LOW_MEDIUM.ipynb**
- These four codes generate annotation files in YOLO or .XML format for each complexity and testing dataset separately. Low and medium complexity datasets use thresholding with binary grayscaling to take advantage of white backgrounds for separating objects and extracting bounding boxes. The high complexity dataset uses constant bounding box annotations due to the complex background.

### Dataset preparation:
- **LOW COMPLEXITY DATASET PREPARATION.ipynb**
- **MEDIUM COMPLEXITY DATASET PREPARATION.ipynb**
- **HIGH COMPLEXITY DATASET PREPARATION.ipynb**
- These three codes were used to split (80/20 stratified splitting) and save the training and validation datasets on Google Drive for use during the experimental phase.

## Experiments

Each code represents a separate experiment using a chosen deep learning architecture trained on a dataset of varying complexity. The codes also contain final testing and results. The name denotes the experiment, the architecture used, and the level of complexity.

### Experiment 1:
- **EXPERIMENT 1 – YOLOv8l – LOW.ipynb**
- **EXPERIMENT 1 – YOLOv8l – MEDIUM.ipynb**
- **EXPERIMENT 1 – YOLOv8l – HIGH.ipynb**

### Experiment 2:
- **EXPERIMENT 2 – Faster RCNN – LOW.ipynb**
- **EXPERIMENT 2 – Faster RCNN – MEDIUM.ipynb**
- **EXPERIMENT 2 – Faster RCNN – HIGH.ipynb**

### Experiment 3:
- **EXPERIMENT 3 – SSD – LOW.ipynb**
- **EXPERIMENT 3 – SSD – MEDIUM.ipynb**
- **EXPERIMENT 3 – SSD – HIGH.ipynb**

