# VehicleCounter-Yolov3
 This project aims to count every vehicle (motorcycle, bus, car, cycle, truck, train) detected in the input video using YOLOv3 object-detection algorithm.
- Link for better understanding : https://drive.google.com/file/d/18w0FSWB-bczSRPti_EPHo25qfM0s6KSm/view?usp=sharing
## Prerequisites
* Linux distro or MacOS or Windows(Tested on Ubuntu 18.04)
* A street video file to run the vehicle counting 
* The pre-trained yolov3 weight file should be downloaded by following these steps:
```
cd yolo-coco
wget https://pjreddie.com/media/files/yolov3.weights
``` 

## Dependencies for using CPU for computations
* Python3 (Tested on Python 3.6.9)
```
sudo apt-get upgrade python3
```
* Pip3
```
sudo apt-get install python3-pip
```
* OpenCV 3.4 or above(Tested on OpenCV 3.4.2.17)
```
pip3 install opencv-python==3.4.2.17
```
* Imutils 
```
pip3 install imutils
```
* Scipy
```
pip3 install scipy
```

Examples: 
* Running with defaults
```
python3 yolo_video.py --input inputVideos/highway.mp4 --output outputVideos/highwayOut.avi --yolo yolo-coco 
```
* Specifying confidence
```
python3 yolo_video.py --input inputVideos/highway.mp4 --output outputVideos/highwayOut.avi --yolo yolo-coco --confidence 0.3
```
## Reference
* https://www.pyimagesearch.com/2018/11/12/yolo-object-detection-with-opencv/ 
