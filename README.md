# Object-Detection using EfficientDet-D2 architecture

## Intution
I have used SOTA to detect the persons and cars instead of the popular choice of YOLO V3. So the intution is that I would freeze the entire network and just retrain the last two layers by changing the classes as person & car. EfficientDet-D2 is the final architecture.

### Folder Structure
![image](https://user-images.githubusercontent.com/48932266/129469546-f6e739a2-29c4-4563-a648-52d6bb72ba47.png)

#### Loss Function and Metrics
Epochs completed : 10 [Due to limited GPU availability]

Hardware: Single GPU, Google Colab

Loss Function: Focal Loss

Metrics: AP

##### NOTE
All code is picked from google's automl repository for efficientdet : https://github.com/google/automl/tree/master/efficientdet

Use Objdet.ipynb file in the colab to replicate results.

To check the result of detection, check the results folder. These images were not used for training and were part of the test set.

In case you need to infer the model on a custom image. Scripts > infer_single_image.py


