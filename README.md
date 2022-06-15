# Ultralytics Yolov5 drowsiness detection
Identification of objects in an image considered a common assignment for the human brain, though not so trivial for a machine. Identification and localization of objects in photos is a computer vision task called ‘object detection’. One of the most popular algorithms to date for real-time object detection is YOLO (You Only Look Once).

In this project, will performed an end-to-end object detection, to be precise drowsiness detection, project to see whether a person is awake or drowsy, using the latest YOLOv5 implementation developed by Ultralytics.

## Steps involved in the process
### 1. Install and import dependencies
Install pytorch(used to load the yolo model and make detections) and some other required libraries

clone the ultralytics yolov5 repository from github then install the requirements.txt file 


### 2. Load Model
load the pretrained ultralytics model from torch hub and use the baseline model yolov5s


### 3. Make detections
Make initial detections.

### 4. Real time detections
 Use opencv to access our webcam and check for real time detections.

### 5. Collecting images and labelling them using labelimg
After having the initial looks and feel of the yolov5 time to kickstart the drowsiness detection from scratch i.e to train a custom yolo model.

First we collect some(20 in our case) images for two classes i.e. awake or drowsy, using the opencv.

then we git clone the labelImg repository from github and install the requirements.txt

Then proceed to label the captured images (awake or drowsy) using labelImg.

### 6. Train the model
Now that we have the labelled images and the pretained yolov5s model we will custom train our model specific to our need.
Train the model for 500 epochs with a batch size of 16. accuracy close to 99.95 %.

### 7. Save and load model
At last we load our trained custom model and see the performance of our model in real time.
