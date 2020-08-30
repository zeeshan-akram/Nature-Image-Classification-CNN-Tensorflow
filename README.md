# Nature Image Classification: Project Overview
I created this model to classify aeroplane, car, cat, dog, flower, fruit, motorbike and person images. Did this project on Kaggle virtual machine on GPU.
* Data from Kaggle.com [Natural Images](https://www.kaggle.com/prasunroy/natural-images).
* Get files and perform labeling.
* Perform Preprocessing images augmentation.
* Model creation and training.
* Visualize loss and accuracy of model.
## Code and Resources Used
**Python Version:** 3.7 <br>
**Packages:** numpy, pandas, tensorflow, keras, matplotlib, efficientnet, sklearn, seaborn, re, math, cv2, PIL, os.<br>
## Get files and perform labeling
In this section retrive images paths and perform labeling. After that convert labels into binary labels. <br>
**e.g** converting from 0,1,2,3 to [1, 0, 0, 0, 0, 0, 0, 0], [0, 1, 0, 0, 0, 0, 0, 0], [0, 0, 1, 0, 0, 0, 0, 0], [0, 0, 0, 1, 0, 0, 0, 0].<br>
**Visualizing:**<br>
Airplane
![loading or Error](https://github.com/zeeshan-akram/Nature-Image-Classification-CNN-Tensorflow/blob/master/airplane.png)
Car
![loading or Error](https://github.com/zeeshan-akram/Nature-Image-Classification-CNN-Tensorflow/blob/master/car.png)
Cat
![loading or Error](https://github.com/zeeshan-akram/Nature-Image-Classification-CNN-Tensorflow/blob/master/cat.png)
Dog
![loading or Error](https://github.com/zeeshan-akram/Nature-Image-Classification-CNN-Tensorflow/blob/master/dog.png)
Flower
![loading or Error](https://github.com/zeeshan-akram/Nature-Image-Classification-CNN-Tensorflow/blob/master/flower.png)
Fruit
![loading or Error](https://github.com/zeeshan-akram/Nature-Image-Classification-CNN-Tensorflow/blob/master/fruit.png)
Motorbike
![loading or Error](https://github.com/zeeshan-akram/Nature-Image-Classification-CNN-Tensorflow/blob/master/motorbike.png)
People
![loading or Error](https://github.com/zeeshan-akram/Nature-Image-Classification-CNN-Tensorflow/blob/master/people.png)
## Preprocessing
In this step I retrive images from their paths and convert those images data into tensors. I also perform image augmentation.
Image Augmentations:
* Rotation.
* Shear.
* Zoom.
* Shifting.
* Random Brightness.
* Random Flip Left Right.<br>
![loading or Error](https://github.com/zeeshan-akram/Nature-Image-Classification-CNN-Tensorflow/blob/master/aug.png)
## Modeling
Create CNN model. Where relu activation function used for hidden layers and for output layer softmax activation function used. Compile model with adam optimizer, categorical_accuracy loss and categorical_accuracy, accuracy metrics. <br>
The layers I used are. <br>
* Conv2D
* MaxPool2D
* BatchNormalization
* Dropout
* Flatten
* Dense
## Model History
After training and validating model. Model have slightly high accuracy in validation rather than training.<br>
![loading or Error](https://github.com/zeeshan-akram/Nature-Image-Classification-CNN-Tensorflow/blob/master/model-history.png)
