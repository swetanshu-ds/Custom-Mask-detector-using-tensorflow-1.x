# Custom-Mask-detector-using-tensorflow-1.x
https://github.com/tensorflow/models/blob/v1.13.0/research/object_detection/g3doc/detection_model_zoo.md

1. Open google colab
2. upload the tfod1. training.ipynb file on colab 
3. remember that the model folder v1.13.0 should be present in the tfod1.x folder.
4. now upload the dataset.zip on the google drive within the TFOD1.x models research folder  given in the github repo which contains images as train and test in                       zip format in the models -> research folder 
5. move the utils sub file folder from models utils to google drive research folder 
6. Now go to the TFOD1.x file in google dirve then go to models then reseearch then go to training than faster rcnn config and change the required changes .ie,

7. num_classes = 2
8. line 107  - PATH TO BE CONFIGURED = faster_rcnn
9. line 113 - num_steps = 10000
10. line 122 = input_path : train.record
11. line 124 = label_map_path: "training/labelmap.pbtxt"
12. line 136: input_path: "test.record"
13. line 138 : label_map_path: "training/labelmap.pbtxt"

14. Now in research folder there is a folder slim move the deployment and nets folder from slim to research main 

15. Time to start training -

16. For this train.py file should be moved to research folder from legacy inside object_detection folder.

17 The training will take so much time.

18. Now go to research object_detection folder and move the export_inference_graph.py file to the research folder
19. Convert Checkpoints to Frozen Inference Graph - run the  code of .ipynb file below this

20 . Inferenceing with our trained model
21. Go to research object_detection and then to object_detection_tutorial.ipynb and open it in google colab.
22. 
