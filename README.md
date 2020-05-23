# Object-Detection
A Keras implementation of YOLOv3 (Tensorflow backend)
# Quick Start

    1.Download YOLOv3 weights from YOLO website(https://pjreddie.com/darknet/yolo/)
    2.Convert the Darknet YOLO model to a Keras model.
    3.Run YOLO detection.
    
If you want to use original pretrained weights for YOLOv3:
 1. wget https://pjreddie.com/media/files/darknet53.conv.74
 2. rename it as darknet53.weights
 3. python convert.py -w darknet53.cfg darknet53.weights model_data/darknet53_weights.h5
 4. use model_data/darknet53_weights.h5 in train.py
# Some issues to know
1.The test environment is

    Python 3.5.2
    Keras 2.1.5
    tensorflow 1.6.0
2.The speed is slower than Darknet. Replacing PIL with opencv may help a little.


