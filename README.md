# Object-Detection

This repository contains the object detection project for the AI course in your engineering semester. The project utilizes the YOLOv5 model for detecting objects in images, videos, and live streams.

Overview
YOLOv5 (You Only Look Once) is a state-of-the-art, real-time object detection model that can detect various objects in images and videos with high accuracy. This project demonstrates the usage of YOLOv5 for object detection on different media sources, including local videos, live camera feeds, and YouTube links.

Setup
Prerequisites
Make sure you have the following installed:

Python 3.7+
PyTorch
OpenCV
Other dependencies listed in requirements.txt
Installation
Clone the repository:

bash
Copy code
git clone https://github.com/yourusername/object-detection-yolov5.git
cd object-detection-yolov5
Install dependencies:

bash
Copy code
pip install -r requirements.txt
Download YOLOv5 weights:

Download the pre-trained weights from the official YOLOv5 repository or use custom-trained weights.

Running the Object Detection
1. Detect objects in an image:
go
Copy code
```bash
python detect.py
```
This command will use the default settings to detect objects in the provided image.

2. Detect objects in a live camera feed:
go
Copy code
```bash
python detect.py --source 0
```
This command will use your computer's default webcam to perform real-time object detection.

3. Detect objects in a video file:
go
Copy code
```bash
python detect.py --source vid.mp4
```
Replace vid.mp4 with the path to your video file. The model will process each frame in the video and display the detected objects.

4. Detect objects in a YouTube video:
go
Copy code
```bash
python detect.py --source 'link of yt video'
```
Replace 'link of yt video' with the actual URL of the YouTube video. This command will stream the video and perform object detection in real time.

Results
The detected objects will be shown in the output window with bounding boxes and labels. The results are saved in the runs/detect/exp directory by default.

Contributing
Feel free to contribute by submitting issues or pull requests. Ensure your code adheres to the project's style guidelines.

License
This project is licensed under the MIT License - see the LICENSE file for details.

Acknowledgments
YOLOv5 by Ultralytics
PyTorch
