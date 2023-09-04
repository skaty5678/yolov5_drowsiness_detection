# Real-Time drowsiness Detection with YOLOv5 and PyTorch

Identification of objects in an image considered a common assignment for the human brain, though not so trivial for a machine. Identification and localization of objects in photos is a computer vision task called ‘object detection’. One of the most popular algorithms to date for real-time object detection is YOLO (You Only Look Once).

In this project, we performed drowsiness detection to check whether a person is awake or drowsy, using the latest YOLOv5 implementation developed by Ultralytics.

## Prerequisites

- PyTorch
- Torchvision
- Torchaudio
- OpenCV
- Matplotlib
- Numpy
- ipywidgets
- PyQt5
- lxml

## Installation

1. Install the required dependencies by running the following command:

    !pip3 install torch torchvision torchaudio


    !pip install opencv-python matplotlib numpy ipywidgets


    !pip install pyqt5==5.15.2 lxml


2. Clone the YOLOv5 repository by running:
 
    !git clone https://github.com/ultralytics/yolov5

3. Navigate to the cloned directory:

    cd yolov5

4. Install the requirements for YOLOv5:

    !pip install -r requirements.txt


5. Clone the labelImg repository for image labeling:

    !git clone https://github.com/tzutalin/labelImg.git


## Usage

1. Collect Images:
- Connect a webcam to your computer.
- Run the code to capture images for the specified labels ("awake" and "drowsy").
- Images will be saved in the "data/images" directory.

2. Label Images:
- Open the labelImg tool to label the collected images as "awake" or "drowsy".
- Save the labeled annotations as XML files.

3. Train the YOLOv5 Model:
- Run the training script with the specified parameters (image size, batch size, epochs, data configuration, weights, etc.).
- The model will be trained on the labeled images using the YOLOv5 architecture.

4. Load the Trained Model:
- Load the trained model weights for inference.
- Perform object detection on images or video streams.

