# Intelexica_flask-yolov5
Two Programs Merged

yolov5 faceDetection, 
flask server

So the idea is you run the flask server (main.py)_ and go the web page with the ip address
There will be a upload button . You will upload a Picture and then it will process the image and return the detected Image with bounding boxes.
Currently Weights used are yolov5


For only Converting the weights or detecting image.

#Detect Image:
python detect.py --source data/images --weights yolov5s.pt --conf 0.25

#Convet pt to onnx:
set PYTHONPATH="$PWD" && python models/export.py --weights yolov5s.pt --img 640 --batch 1

#Convert pt to tflite:
python tf.py --weights weights/yolov5s.pt --cfg models/yolov5s.yaml --img 640


Weights: https://drive.google.com/drive/folders/1jaRtyjd_IFec9i86bi4ZMPXWWrTK-8kD?usp=sharing
Place them weights/...
