# Custom-Mask-detector-using-tensorflow-1.x
https://github.com/tensorflow/models/blob/v1.13.0/research/object_detection/g3doc/detection_model_zoo.md

1. Open google colab
2. upload the tfod1. training.ipynb file on colab 
3. remember that the model folder v1.13.0 should be present in the tfod1.x folder.
4. now upload the dataset given in the github repo which contains images as train and test in zip format in the models -> research folder 
5. move the utils sub file folder from models utils to google drive research folder 
6. Nw go to the TFOD1.x file in google dirve then go to models then reseearch then go to training than faster rcnn config and change the required changes .ie,

num_classes = 2
line 107  - PATH TO BE CONFIGURED = faster_rcnn
line 113 - num_steps = 10000
line 122 = input_path : train.record
line 124 = label_map_path: "training/labelmap.pbtxt"
line 136: input_path: "test.record"
line 138 : label_map_path: "training/labelmap.pbtxt"

Now in research folder there is a folder slim move the deployment and nets folder from slim to research main 


5. then run this TFOD1_x_training.ipynb file from starting to end



