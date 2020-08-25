# Nature Image Classification: Project Overview
I created this model to classify airplane, car, cat, dog, flower, fruit, motorbike and person images. Did this project on Kaggle virtual machine on GPU.
* Data from [Natural Images](https://www.kaggle.com/prasunroy/natural-images).
* Get files and perform labeling.
* Perform Preprocessing images augmentation.
* Model creation and training.
* Visualize loss and accuracy of model.
## Code and Resources Used
**Python Version:** 3.7 <br>
**Packages:** numpy, pandas, tensorflow, keras, matplotlib, efficientnet, sklearn, seaborn, re, math, cv2, PIL, os.<br>
## Preprocessing
In this step I retrive images from their paths and convert those images data into tensors. I also perform image augmentation.
Image Augmentations:
* Rotation.
* Shear.
* Zoom.
* Shifting.
* Random Brightness.
* Random Flip Left Right.
