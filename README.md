# Vietnam-Identity-Card-Id-Name-DoB-Extraction
This repository includes Colab Notebook of code extracting Id, Name and Date of Birth from Vietnam Identity Card

The pipelines of the system are as follow:

![pipeline](https://github.com/user-attachments/assets/f5196157-720a-48c1-9909-bc1142acd494)

1. Using Yolov5 object detection to detect 4 corners of the ID card.
2. From detected corners, rotate and stretch the image to front-view. (With some image processing method, this step can handle with some missing corners cases (misisng 1, and 4 corners)
4. Using Yolov5 object detecton model to detect ID, Name and Date of Birth from the card.
5. With the ID, Name and DoB image, run them through VietOCR model to translate the words in the pictures into texts.

** Pre-trained weights: **

Corners Detections - [Google Drives](https://drive.google.com/file/d/1WedHEte2CJl2vWmc1zUALJjCJ6-HUJ5X/view?usp=sharing)

Info Extraction - [Google Drives](https://drive.google.com/file/d/1MWRUqOmGkMVFRcqfAQQ8PI7bF6pnPP1T/view?usp=sharing)

** Related Repos **

Info Translation (VietOCR): [VietOCR](https://github.com/pbcquoc/vietocr)

Yolov5: [YOLOv5](https://github.com/ultralytics/yolov5)
