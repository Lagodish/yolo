Training YOLOv3 object detection.
We'll be training a YOLOv3 and YOLOv3-tiny (You Only Look Once) model. This specific model is a one-shot learner, meaning each image only passes through the network once to make a prediction, which allows the architecture to be very performant, viewing up to 60 frames per second in predicting against video feeds.

Convertation from Darknet to CoreML
Download YOLOv3 pretrained weights from YOLO website. Download both cfg and weights files.
Load Darknet weights to Keras model using Keras-YOLOv3 implementation.
After cloning above repo use this commend to load Darknet and save .h5:

python convert.py yolov3.cfg yolov3.weights model_data/yolo.h5
