#### OCR
I have taken custom weights file from github
link : https://drive.google.com/file/d/1EUPtbtdF0bjRtNjGv436vDY28EN5DXDH/view

Add the above custom.weights file in the data folder.
Run this command after that : python save_model.py --weights ./data/custom.weights --output ./checkpoints/custom-416 --input_size 416 --model yolov4 


PREDICTION :

PLACE THE IMAGE YOU WANT TO PREDICT IN THE data/images FOLDER AND RUN THE BELOW COMMAND WITH RESPECTIVE IMAGE NAME
command : python detect.py --weights ./checkpoints/custom-416 --size 416 --model yolov4 --images ./data/images/car2.jpg --plate

